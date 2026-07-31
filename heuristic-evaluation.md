---
name: heuristic-evaluation
description: >
  Perform a comprehensive UX heuristic evaluation on a design provided as an attached screenshot, a
  Figma file/frame link, or a live website URL (landing page, microsite, or any web page) using
  Nielsen's 10 Usability Heuristics plus extended heuristics for accessibility and visual design.
  Outputs an interactive dashboard with severity scores, issue tables, and prioritized
  recommendations. Trigger whenever a user provides any of these three input types (attached image,
  figma.com link, or http/https URL) and asks for "heuristic evaluation", "heuristic analysis",
  "usability audit", "UX audit", "heuristic review", "audit this website/page/site/microsite", or
  "audit this Figma file/frame" — even without the word "heuristic". Always use this skill (not
  design-critique) when the user mentions heuristics, usability evaluation, or a structured/scored
  UX audit.
---

# Heuristic Evaluation Skill

A rigorous, structured UX heuristic evaluation framework for any digital design artifact. Produces
a comprehensive interactive dashboard with per-heuristic scoring, severity-ranked issue tables,
and actionable fix recommendations.

---

## When to Use

Use this skill when:
- A design image is attached, OR a Figma link is shared, OR a website URL is shared — AND the user
  mentions: heuristic, usability audit, UX audit, evaluation, structured review, or scored analysis
- The user asks for heuristic analysis, heuristic evaluation, or a formal UX review of a screenshot,
  Figma frame, landing page, microsite, or any live web page
- The user wants a scored, systematic breakdown of UX issues (not just general design feedback)

If none of the three input types (image, Figma link, URL) is provided, ask the user to supply one
before proceeding.

---

## Input Sources

This skill accepts three input types. Identify which one applies, then follow the matching
acquisition path below **before** starting the Analysis Process. All three paths converge on the
same output: one or more evaluatable images/content passed into the standard 13-heuristic framework.

### Source A: Attached Screenshot / Mockup / Wireframe
Use the image directly as provided. No acquisition step needed. This is the baseline case the rest
of this skill was originally written for.

### Source B: Figma Link
Trigger on any `figma.com/design/...`, `figma.com/file/...`, or `figma.com/proto/...` URL.

1. Call `tool_search` (e.g. query "figma design context screenshot") to load the Figma MCP tools if
   not already loaded.
2. Use `Figma:get_screenshot` on the linked node/frame to get the visual artifact to evaluate.
3. Use `Figma:get_design_context` on the same node to pull structural context (component names,
   variant properties, text content) — this materially improves accuracy for H2 (Match with Real
   World), H4 (Consistency), and E2 (Visual Hierarchy), since you can cross-check labels and
   component reuse instead of guessing from pixels alone.
4. If the link points to a whole file rather than a specific frame, ask the user which frame/flow
   to audit rather than guessing — Figma files commonly contain many unrelated frames.
5. If the link is a `.../proto/...` prototype link, note in Step 1 (Orient & Identify Context) that
   interactive heuristics (H3, H9) can be assessed more confidently than from a static frame, and
   evaluate transitions/states if `get_design_context` surfaces them.

### Source C: Website URL
Trigger on any `http://` or `https://` URL that is not a Figma link.

1. Call `tool_search` (e.g. query "browser navigate screenshot") to load the browser tools if not
   already loaded.
2. Navigate to the URL.
3. **Viewport default: desktop only.** Only capture/evaluate a mobile viewport if the user explicitly
   asks for mobile, responsive, or multi-viewport review. If they do, resize the window to a mobile
   width (e.g. 390px) and repeat the capture/evaluation as a separate pass, then compare the two in
   the dashboard (see "Multi-Viewport Output" below).
4. **Full-page capture is the default for landing pages / microsites.** Scroll through the entire
   page and capture every section — do not stop at the first viewport ("above the fold") unless the
   user explicitly asks for above-the-fold only. Long pages should be captured as a sequence of
   section screenshots (hero, then each subsequent section in order) rather than one attempted
   mega-screenshot, since most capture tools have height limits and heuristics like H8 (Aesthetic &
   Minimalist Design) need to be judged per-section as well as holistically.
5. Optionally use a page-text extraction tool to cross-check copy/labels for H2, H6, H10 — useful
   when a section's content is dense (long-form text, pricing tables, FAQs).
6. Treat the full set of section screenshots as **one artifact** for scoring purposes (one set of
   13 heuristic scores for the page as a whole), but track *which section* each issue occurs in —
   the Issues Table's "Location" column should name the section (e.g. "Hero", "Pricing table",
   "Footer"), not just "the page".

### Multi-Viewport Output (only when mobile was explicitly requested)
When both desktop and mobile were captured, extend Panel 2 (Scorecard) with a second score column
per viewport, and add a short "Desktop vs Mobile" delta note per heuristic where scores diverge by
2+ points. Don't build two separate dashboards — one unified dashboard with both viewports keeps
cross-viewport consistency (H4) checkable at a glance.

---

## Visual Evidence Crops

For the highest-impact issues, attach a cropped image of the actual problem area next to the
finding instead of describing it in text alone. This is **not** applied to every issue — only to
issues that make it into the **Priority Fix List (Panel 5)** and any issue rated 🔴 Critical or
🟠 Major in the Issues Table (Panel 4). Applying it to every issue (which can number 20–30+ across
a full audit) bloats the dashboard's file size for little added value on low-severity items.

### Sourcing the crop by input type

- **Source B (Figma)**: Use the bounding box (`x`, `y`, `width`, `height`) returned by
  `get_design_context` for the specific node/layer the issue refers to. This gives a pixel-precise
  crop straight from structural data — no visual guessing required. Crop directly from that
  region of the frame image already retrieved via `get_screenshot`.
- **Source A (uploaded screenshot) / Source C (website URL)**: Crop is based on your own visual
  estimate of the problem region from the captured image. Since this is an estimate rather than a
  structural coordinate, **overlay a thin red bounding box** around the specific element in the
  crop so the reader can see exactly what's being flagged, not just "somewhere in this area."

### Processing

1. Use the bash tool with a Python image library (e.g. Pillow) to crop the relevant region from
   the source screenshot/frame image.
2. For Source A/C, draw the red bounding-box overlay before final crop.
3. Resize each crop to a max width of ~500–600px before encoding, to keep the dashboard's payload
   light.
4. Encode the resulting crop as base64 and embed it directly in the widget HTML as
   `<img src="data:image/png;base64,...">` — no external hosting or file links, so the dashboard
   stays fully self-contained per the existing implementation constraints.

### Placement in the dashboard

Add a **"Visual"** column to Panel 5 (Priority Fix List), showing a small thumbnail per fix. Make
the thumbnail clickable (or hoverable) to expand into a simple JS lightbox overlay showing the
full-size crop. Do not add thumbnails to the main Issues Table (Panel 4) by default — keep that
table text-only and reserve visuals for the Priority Fix List, unless the user explicitly asks for
visuals on every row.

If cropping isn't feasible for a given issue (e.g. the location spans multiple non-contiguous
areas, or the input source doesn't support it), fall back to text-only for that item rather than
skipping the fix recommendation entirely.

---

## Evaluation Framework

### Primary: Nielsen's 10 Usability Heuristics

| # | Heuristic | Key Questions |
|---|---|---|
| H1 | **Visibility of System Status** | Does the UI always inform users of what's going on? Loading states, progress, feedback? |
| H2 | **Match Between System & Real World** | Does the language/metaphor match user mental models? Jargon-free? |
| H3 | **User Control & Freedom** | Can users undo, redo, escape? Are exits clearly marked? |
| H4 | **Consistency & Standards** | Are patterns, labels, icons consistent? Does it follow platform conventions? |
| H5 | **Error Prevention** | Does the design prevent errors before they happen? Constraints, confirmation dialogs? |
| H6 | **Recognition Over Recall** | Is information visible/accessible? Are options shown, not memorized? |
| H7 | **Flexibility & Efficiency of Use** | Are there shortcuts for expert users? Accelerators? Customization? |
| H8 | **Aesthetic & Minimalist Design** | Is information minimal and relevant? No irrelevant/rarely-needed content? |
| H9 | **Help Recognize, Diagnose & Recover Errors** | Are error messages clear, plain-language, actionable? |
| H10 | **Help & Documentation** | Is help accessible? Is documentation searchable and task-focused? |

### Extended Heuristics

| # | Heuristic | Key Questions |
|---|---|---|
| E1 | **Accessibility & Inclusive Design** | WCAG compliance, color contrast, touch targets, screen reader support? |
| E2 | **Visual Hierarchy & Information Architecture** | Is content structured logically? Can users orient themselves quickly? |
| E3 | **Feedback & Affordance** | Do interactive elements look interactive? Do actions have clear affordances? |

---

## Scoring System

For each heuristic, assign:

**Score (0–10)**: 
- 9–10: Excellent — no issues found
- 7–8: Good — minor issues, non-blocking
- 5–6: Needs Work — notable issues affecting usability
- 3–4: Poor — significant problems impacting user experience
- 0–2: Critical — severe failures, must fix immediately

**Severity per Issue (1–4)** (Nielsen Severity Rating):
- 🔴 **4 — Usability Catastrophe**: Must fix before release
- 🟠 **3 — Major Usability Problem**: High priority to fix
- 🟡 **2 — Minor Usability Problem**: Low priority, fix if time permits
- 🟢 **1 — Cosmetic Problem**: Fix only if extra time
- ⚪ **0 — Not a usability problem**

---

## Analysis Process

### Step 1: Orient & Identify Context
Before evaluating, identify:
- What type of screen/flow is this? (onboarding, dashboard, form, landing page, microsite, etc.)
- Who is the likely target user?
- What is the primary user goal on this screen?
- What platform/device is it designed for?
- Which input source was used (screenshot / Figma link / website URL), which viewport(s) were
  captured, and whether the capture is full-page or above-the-fold — state this explicitly in the
  Executive Summary Bar so the reader knows the evaluation's scope.

### Step 2: Evaluate Each Heuristic
For each of the 13 heuristics (H1–H10 + E1–E3):
- Assign a score (0–10)
- List specific issues observed, each with:
  - Description of the problem
  - Where exactly it occurs
  - Severity rating (1–4)
  - Specific fix recommendation
- Note if the heuristic is not applicable (mark as N/A)

### Step 3: Calculate Summary Metrics
- **Overall Usability Score**: Weighted average of all heuristic scores
  - Core heuristics (H1–H10): 70% weight
  - Extended heuristics (E1–E3): 30% weight
- **Issue Count by Severity**: Count of 🔴 Critical / 🟠 Major / 🟡 Minor / 🟢 Cosmetic
- **Heuristics at Risk**: Any heuristic scoring below 5

### Step 4: Produce Dashboard Output (REQUIRED)

**Always output the results as an interactive HTML dashboard using the `show_widget` tool.**

The dashboard must include all sections below. See the Dashboard Template section for implementation.

---

## Dashboard Template

Build an interactive React/HTML dashboard with these panels:

### Panel 1: Executive Summary Bar
- Overall Usability Score (large number, color-coded: red <50, amber 50–70, green >70)
- Total issues found (broken down by severity)
- Design context identified (screen type, platform, user goal)
- Heuristics Passed / At Risk / Failed counts

### Panel 2: Heuristic Scorecard Table
Full-width table with columns:
| Heuristic | Score | Status | Issues Found | Top Issue |
Each row color-coded by score band. Clicking a row expands to show all issues for that heuristic.

### Panel 3: Severity Distribution Chart
Visual bar or donut chart showing:
- Count of Critical (🔴) / Major (🟠) / Minor (🟡) / Cosmetic (🟢) issues
- Total issue count

### Panel 4: Issues Table (sortable by severity)
All issues across all heuristics in one table:
| Severity | Heuristic | Issue | Location | Fix |
Default sorted by severity (Critical first). Allow filtering by heuristic.

### Panel 5: Priority Fix List
Top 5 highest-impact fixes, each with:
- Visual crop (thumbnail, click/hover to expand — see Visual Evidence Crops section)
- Issue description
- Heuristic violated
- Recommended fix
- Effort estimate (Low / Medium / High)

### Panel 6: Heuristic Radar/Spider Chart (optional but preferred)
Visual radar chart showing scores across all 13 heuristics — gives a clear pattern-at-a-glance.

---

## Dashboard Implementation Guide

Use `show_widget` with HTML+CSS+JS. Follow this structure:

```html
<!-- Use CSS variables for theming -->
<style>
  :root {
    --score-critical: #ef4444;
    --score-major: #f97316;
    --score-minor: #eab308;
    --score-cosmetic: #22c55e;
    --score-good: #3b82f6;
  }
</style>
```

**Key implementation notes:**
- Use inline JS for interactivity (tab switching, row expansion, filtering)
- Embed all data as JS variables at the top of the script — don't make API calls from within the widget
- Radar chart: use SVG with calculated polygon points — no external chart libraries needed
- Make the dashboard self-contained (no external dependencies)
- Use a clean, professional dark-or-light theme (match what feels right for the design type)
- Add a "Copy Report" button that copies a plain-text summary to clipboard
- Visual crops (Panel 5): embed as base64 data URIs generated per the Visual Evidence Crops section
  — never reference an external file path or URL, since the widget has no filesystem access at
  render time. A simple click-to-expand lightbox (an absolutely-positioned overlay div toggled by
  JS) is enough; no external lightbox library needed.

---

## Output Sequence

1. **Brief intro** (2–3 sentences): What design was analyzed, context identified
2. **`show_widget` call** with the full interactive dashboard
3. **Narrative summary** (after the widget): 3–5 sentences on the biggest findings and most critical fixes

Do NOT output the full analysis as a wall of text — the dashboard IS the primary output.
The narrative before/after the dashboard should be brief and contextual.

---

## Tone & Standards

- Be precise: reference specific elements, locations, and measurements where possible
- Be actionable: every issue must have a concrete fix recommendation
- Be proportionate: calibrate depth to the complexity of the design
- Apply WCAG 2.1 AA as the accessibility standard unless otherwise specified
- Reference established principles when citing issues (e.g., "violates H4 — Consistency & Standards")
- If a heuristic cannot be fully evaluated from a static image (e.g., H3, H9), note what can be
  assessed and flag what would need interactive testing

---

## Special Cases

**Wireframes / Low-fidelity**: Skip E1 (accessibility) and E2 visual scoring. Focus on H1–H10 structural heuristics.
**Mobile screens**: Apply mobile-specific standards (min 44×44px touch targets, thumb zone awareness).
**Complex flows / multiple screens**: Evaluate each screen, then summarize cross-screen consistency.
**Marketing / landing pages / microsites (full-page capture)**: Weight H2, H6, H8 more heavily
  (clarity, recognition, minimalism). Evaluate as one page-level score, but log issues per section
  in the Issues Table. Also explicitly check cross-section consistency (H4) — e.g. CTA button style,
  heading hierarchy, and spacing rhythm staying consistent from hero through footer — since
  inconsistency across sections is a common landing-page failure mode that a single-viewport review
  would miss.
**Live website audits (Source C)**: If the page requires a cookie/consent banner interaction to see
  real content, note this as an H1/H5 observation itself (does the banner block content, is dismissal
  obvious) rather than silently dismissing it and pretending it wasn't there.
**Forms**: Weight H5, H9 heavily (error prevention and recovery are critical in form flows).
