---
version: alpha
name: HOLDS
release: 4.0.0
status: stable
lastUpdated: 2026-10-15
tokenSource: ds-v4.json (Tokens Brücke DTCG export, 11 variable collections, generated
  2026-10-08). Components from the HOL Design System 2.0 Figma library (1gSTFbZHnohv4iJr9k51et),
  15 component pages read 2026-10-12. Document version 4.1 — see "Token Update Log (v4.1)".
name: Hukumonline (HOL) Design System
description: A legal-information platform that pairs an authoritative navy brand
  with a warm golden secondary accent. Typography stays grounded in Inter for
  body reading — long-form legal text demands high legibility at moderate sizes —
  while Nunito Sans carries display, heading, and button-label moments with
  confident weight. Surfaces are predominantly white with a light neutral border;
  depth is expressed through subtle brand-tinted shadows rather than heavy drop
  shadows. Every primary CTA runs in HOL navy, secondary moments in gold, and
  status signals use conventional semantic colors (green success, red danger,
  yellow warning, blue info).

# NOTE ON THE v4 TOKEN UPDATE: the colors block below is now a flat, 1:1 mirror of
# "Colors - Semantic" (path dots → dashes, e.g. surface.brand-primary.base →
# surface-brand-primary-base). The trailing comment on each line is the primitive
# it aliases. The "[unuse]" group in the source is intentionally excluded.
# Components further down reference the dotted source path directly
# (e.g. "{surface.brand-primary.base}"), so they stay traceable to Figma Variables.
colors:
  # ── Surface ─────────────────────────────────────────────────────
  surface-brand-primary-strong: "#05213e"           # blue.1100
  surface-brand-primary-base: "#003366"             # blue.1000
  surface-brand-primary-moderate: "#00458a"         # blue.900
  surface-brand-primary-mild: "#125190"             # blue.800
  surface-brand-primary-muted: "#0052a3"            # blue.700
  surface-brand-primary-subtle: "#2877c5"           # blue.600
  surface-brand-primary-soft: "#89bff4"             # blue.300
  surface-brand-primary-lighter: "#e0ecf9"          # blue.200
  surface-neutral-strong: "#162533"                 # neutral.500
  surface-neutral-base: "#2b4156"                   # neutral.400
  surface-neutral-muted: "#607a93"                  # neutral.300
  surface-neutral-subtle: "#8398ab"                 # neutral.200
  surface-neutral-soft: "#a8b8c7"                   # neutral.100
  surface-neutral-lighter: "#cfd9e2"                # neutral.75
  surface-neutral-lightest: "#f5f7f9"               # neutral.50
  surface-neutral-white: "#ffffff"                  # neutral.0
  surface-brand-secondary-base: "#f8ca0f"           # yellow.400
  surface-brand-secondary-subtle: "#ffe168"         # yellow.300
  surface-brand-secondary-soft: "#fff3c5"           # yellow.200
  surface-danger-base: "#dc381f"                    # red.600
  surface-danger-soft: "#ffeff0"                    # red.100
  surface-info-base: "#2877c5"                      # blue.600
  surface-info-soft: "#ebf6fc"                      # blue.100
  surface-success-base: "#00875a"                   # green.600
  surface-success-soft: "#eefdf6"                   # green.100
  surface-warning-base: "#daa520"                   # yellow.500
  surface-warning-soft: "#fff9e3"                   # yellow.100
  surface-accent-purple-strong: "#080d26"           # purple.1200
  surface-accent-purple-intense: "#1c0f3e"          # purple.1100
  surface-accent-purple-base: "#2c084e"             # purple.1000
  surface-accent-purple-moderate: "#2a2461"         # purple.900
  surface-accent-purple-mild: "#492ea1"             # purple.800
  surface-accent-purple-muted: "#7a2df1"            # purple.600
  surface-accent-purple-subtle: "#873de8"           # purple.500
  surface-accent-purple-soft: "#b314e4"             # purple.400
  surface-accent-purple-lighter: "#b361fc"          # purple.300
  surface-accent-indigo-strong: "#0c2373"           # indigo.1000
  surface-accent-indigo-base: "#391d8b"             # indigo.900
  surface-accent-indigo-moderate: "#3b27bb"         # indigo.700
  surface-accent-indigo-mild: "#4022fa"             # indigo.600
  surface-accent-indigo-muted: "#4f4ff5"            # indigo.500
  surface-accent-indigo-subtle: "#717de5"           # indigo.300
  surface-accent-indigo-soft: "#218eb9"             # indigo.200
  surface-accent-indigo-lighter: "#1cb1d1"          # indigo.100
  surface-overlay-inverse: "rgba(255, 255, 255, 0.3)"# neutral.0 @ 30%
  surface-overlay-inverse-soft: "rgba(255, 255, 255, 0.2)"# neutral.0 @ 20%
  surface-overlay-inverse-weak: "rgba(255, 255, 255, 0.1)"# neutral.0 @ 10%
  surface-overlay-soft: "rgba(245, 247, 249, 0.1)"  # neutral.50 @ 10%
  surface-overlay-contrast: "rgba(22, 37, 51, 0.2)" # neutral.500 @ 20%
  surface-overlay-default-weak: "rgba(5, 33, 62, 0.3)"# blue.1100 @ 30%
  surface-overlay-default: "rgba(5, 33, 62, 0.4)"   # blue.1100 @ 40%
  surface-overlay-info-weak: "rgba(40, 119, 197, 0.1)"# blue.600 @ 10%
  surface-overlay-info: "rgba(40, 119, 197, 0.3)"   # blue.600 @ 30%
  surface-overlay-danger: "rgba(220, 56, 31, 0.4)"  # red.600 @ 40%
  surface-overlay-danger-strong: "rgba(220, 56, 31, 0.6)"# red.600 @ 60%
  # ── Background ──────────────────────────────────────────────────
  background-danger: "#ffeff0"                      # red.100
  background-info: "#ebf6fc"                        # blue.100
  background-success: "#eefdf6"                     # green.100
  background-warning: "#fff9e3"                     # yellow.100
  background-neutral-strong: "#162533"              # neutral.500
  background-neutral-lighter: "#cfd9e2"             # neutral.75
  background-neutral-lightest: "#f5f7f9"            # neutral.50
  background-neutral-white: "#ffffff"               # neutral.0
  # ── Text ────────────────────────────────────────────────────────
  text-neutral-primary: "#2b4156"                   # neutral.400
  text-neutral-secondary: "#607a93"                 # neutral.300
  text-neutral-tertiary: "#8398ab"                  # neutral.200
  text-neutral-quaternary: "#a8b8c7"                # neutral.100
  text-neutral-muted: "#f5f7f9"                     # neutral.50
  text-neutral-inverse: "#ffffff"                   # neutral.0
  text-danger-strong: "#800000"                     # red.800
  text-danger-base: "#dc381f"                       # red.600
  text-warning-strong: "#6f4e37"                    # yellow.800
  text-info-strong: "#00458a"                       # blue.900
  text-info-base: "#2877c5"                         # blue.600
  text-success-strong: "#006040"                    # green.800
  text-success-base: "#00875a"                      # green.600
  text-brand-secondary-base: "#f8ca0f"              # yellow.400
  text-brand-secondary-moderate: "#daa520"          # yellow.500
  text-brand-secondary-strong: "#8d7101"            # yellow.700
  text-brand-primary-base: "#003366"                # blue.1000
  text-brand-primary-strong: "#05213e"              # blue.1100
  text-brand-primary-muted: "#0052a3"               # blue.700
  text-brand-primary-soft: "#89bff4"                # blue.300
  # ── Border ──────────────────────────────────────────────────────
  border-state-disabled: "#cfd9e2"                  # neutral.75
  border-state-active: "#2877c5"                    # blue.600
  border-state-interactive: "#0052a3"               # blue.700
  border-neutral-default: "#a8b8c7"                 # neutral.100
  border-neutral-strong: "#607a93"                  # neutral.300
  border-neutral-soft: "#f5f7f9"                    # neutral.50
  border-neutral-moderate: "#8398ab"                # neutral.200
  border-status-danger: "#dc381f"                   # red.600
  border-status-danger-strong: "#800000"            # red.800
  border-status-success: "#00875a"                  # green.600
  border-status-warning: "#daa520"                  # yellow.500
  border-inverse-inverse: "#ffffff"                 # neutral.0
  border-inverse-inverse-transparent: "rgba(255, 255, 255, 0)"# neutral.0 @ 0%
  border-inverse-inverse-weak: "rgba(255, 255, 255, 0.3)"# neutral.0 @ 30%
  border-brand-primary: "#003366"                   # blue.1000
  border-brand-primary-soft: "#e0ecf9"              # blue.200
  # ── Icon ────────────────────────────────────────────────────────
  icon-danger-strong: "#800000"                     # red.800
  icon-danger-base: "#dc381f"                       # red.600
  icon-info-base: "#2877c5"                         # blue.600
  icon-info-soft: "#ebf6fc"                         # blue.100
  icon-success-base: "#00875a"                      # green.600
  icon-warning-strong: "#daa520"                    # yellow.500
  icon-warning-base: "#f8ca0f"                      # yellow.400
  icon-neutral-base: "#2b4156"                      # neutral.400
  icon-neutral-muted: "#607a93"                     # neutral.300
  icon-neutral-subtle: "#8398ab"                    # neutral.200
  icon-neutral-soft: "#a8b8c7"                      # neutral.100
  icon-neutral-inverse: "#ffffff"                   # neutral.0
  icon-brand-primary-strong: "#05213e"              # blue.1100
  icon-brand-primary-base: "#003366"                # blue.1000
  icon-brand-primary-moderate: "#00458a"            # blue.900
  icon-brand-primary-muted: "#0052a3"               # blue.700
  icon-brand-primary-soft: "#89bff4"                # blue.300
  # ── Shadow tint (brand navy alpha) ──────────────────────────────
  shadow-extra-light: "rgba(0, 51, 102, 0.07)"      # blue.1000 @ 7%
  shadow-light: "rgba(0, 51, 102, 0.09)"            # blue.1000 @ 9%
  shadow-medium: "rgba(0, 51, 102, 0.12)"           # blue.1000 @ 12%
  shadow-heavy: "rgba(0, 51, 102, 0.16)"            # blue.1000 @ 16%

typography:
  # Mirrors "Typo - Semantic" (text.*) + "Label Button - Semantic" (button-label.*).
  # Values are the Desktop mode. Every entry carries a "# mobile →" comment with
  # the Mobile-mode size / line-height / letter-spacing resolved from the source.
  # Font weights are family-specific ramps (font.weight.nunito sans.* / inter.*).
  heading-1-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1100}"              # 50px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.1400}"          # 60px
    letterSpacing: "{letter-spacing.70}"              # 0.7px
    # mobile → 32px / 44px / ls 0.5px
  heading-1-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1100}"              # 50px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.1400}"          # 60px
    letterSpacing: "{letter-spacing.70}"              # 0.7px
    # mobile → 32px / 44px / ls 0.5px
  heading-1-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1100}"              # 50px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.1400}"          # 60px
    letterSpacing: "{letter-spacing.70}"              # 0.7px
    # mobile → 32px / 44px / ls 0.5px
  heading-2-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1000}"              # 42px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.1300}"          # 50px
    letterSpacing: "{letter-spacing.60}"              # 0.6px
    # mobile → 24px / 32px / ls 0.4px
  heading-2-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1000}"              # 42px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.1300}"          # 50px
    letterSpacing: "{letter-spacing.60}"              # 0.6px
    # mobile → 24px / 32px / ls 0.4px
  heading-2-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1000}"              # 42px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.1300}"          # 50px
    letterSpacing: "{letter-spacing.60}"              # 0.6px
    # mobile → 24px / 32px / ls 0.4px
  heading-3-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.900}"               # 35px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.1200}"          # 46px
    letterSpacing: "{letter-spacing.20}"              # 0.15px
    # mobile → 22px / 30px / ls 0px
  heading-3-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.900}"               # 35px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.1200}"          # 46px
    letterSpacing: "{letter-spacing.20}"              # 0.15px
    # mobile → 22px / 30px / ls 0px
  heading-3-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.900}"               # 35px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.1200}"          # 46px
    letterSpacing: "{letter-spacing.20}"              # 0.15px
    # mobile → 22px / 30px / ls 0px
  heading-4-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.800}"               # 29px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.1100}"          # 40px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 20px / 28px / ls 0px
  heading-4-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.800}"               # 29px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.1100}"          # 40px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 20px / 28px / ls 0px
  heading-4-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.800}"               # 29px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.1100}"          # 40px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 20px / 28px / ls 0px
  title-1-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.700}"               # 24px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.1000}"          # 36px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 18px / 26px / ls 0px
  title-1-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.700}"               # 24px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.1000}"          # 36px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 18px / 26px / ls 0px
  title-2-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.600}"               # 20px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.800}"           # 30px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 16px / 26px / ls 0px
  title-2-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.600}"               # 20px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.800}"           # 30px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 16px / 26px / ls 0px
  title-2-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.600}"               # 20px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.800}"           # 30px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 16px / 26px / ls 0px
  subtitle-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.800}"           # 30px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 16px / 26px / ls 0px
  subtitle-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.800}"           # 30px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 16px / 26px / ls 0px
  subtitle-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.800}"           # 30px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 16px / 26px / ls 0px
  body-1-bold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.inter.700}"             # 700 Bold
    lineHeight: "{line-height.desktop.700}"           # 28px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 16px / 26px / ls 0px
  body-1-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.700}"           # 28px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 16px / 26px / ls 0px
  body-1-medium:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.inter.500}"             # 500 Medium
    lineHeight: "{line-height.desktop.700}"           # 28px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 16px / 26px / ls 0px
  body-1-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.inter.400}"             # 400 Regular
    lineHeight: "{line-height.desktop.700}"           # 28px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 16px / 26px / ls 0px
  body-2-bold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.400}"               # 16px
    fontWeight: "{font.weight.inter.700}"             # 700 Bold
    lineHeight: "{line-height.desktop.600}"           # 26px
    letterSpacing: "{letter-spacing.30}"              # 0.25px
    # mobile → 14px / 24px / ls 0px
  body-2-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.400}"               # 16px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.600}"           # 26px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 14px / 24px / ls 0px
  body-2-medium:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.400}"               # 16px
    fontWeight: "{font.weight.inter.500}"             # 500 Medium
    lineHeight: "{line-height.desktop.600}"           # 26px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 14px / 24px / ls 0px
  body-2-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.400}"               # 16px
    fontWeight: "{font.weight.inter.400}"             # 400 Regular
    lineHeight: "{line-height.desktop.600}"           # 26px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 14px / 24px / ls 0px
  body-3-bold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.inter.700}"             # 700 Bold
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 12px / 20px / ls 0px
  body-3-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 12px / 20px / ls 0px
  body-3-medium:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.inter.500}"             # 500 Medium
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 12px / 20px / ls 0px
  body-3-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.inter.400}"             # 400 Regular
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 12px / 20px / ls 0px
  body-article-bold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.inter.700}"             # 700 Bold
    lineHeight: "{line-height.desktop.900}"           # 32px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 18px / 32px / ls 0.13px  (identical to desktop)
  body-article-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"               # 18px
    fontWeight: "{font.weight.inter.400}"             # 400 Regular
    lineHeight: "{line-height.desktop.900}"           # 32px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 18px / 32px / ls 0.13px  (identical to desktop)
  caption-medium:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.200}"               # 12px
    fontWeight: "{font.weight.inter.500}"             # 500 Medium
    lineHeight: "{line-height.desktop.300}"           # 20px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 10px / 16px / ls 0px
  caption-bold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.200}"               # 12px
    fontWeight: "{font.weight.inter.700}"             # 700 Bold
    lineHeight: "{line-height.desktop.300}"           # 20px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 10px / 16px / ls 0px
  caption-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.200}"               # 12px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.300}"           # 20px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 10px / 16px / ls 0px
  caption-regular:                       # source key is "caption.reguler" (typo in Figma) — normalised here
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.200}"               # 12px
    fontWeight: "{font.weight.inter.400}"             # 400 Regular
    lineHeight: "{line-height.desktop.300}"           # 20px
    letterSpacing: "{letter-spacing.0}"               # 0px
    # mobile → 12px / 16px / ls 0px
  small-extrabold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.100}"               # 10px
    fontWeight: "{font.weight.inter.800}"             # 800 Extra Bold
    lineHeight: "{line-height.desktop.100}"           # 16px
    letterSpacing: "{letter-spacing.20}"              # 0.15px
    # mobile → 9px / 14px / ls 0.13px
  small-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.100}"               # 10px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.100}"           # 16px
    letterSpacing: "{letter-spacing.20}"              # 0.15px
    # mobile → 9px / 14px / ls 0.13px
  extra-small-extrabold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.75}"                # 8px
    fontWeight: "{font.weight.inter.800}"             # 800 Extra Bold
    lineHeight: "{line-height.desktop.100}"           # 16px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 8px / 16px / ls 0.13px  (identical to desktop)
  extra-small-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.75}"                # 8px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.100}"           # 16px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 8px / 16px / ls 0.13px  (identical to desktop)
  2x-small-extrabold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.25}"                # 6px
    fontWeight: "{font.weight.inter.800}"             # 800 Extra Bold
    lineHeight: "{line-height.desktop.100}"           # 16px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 6px / 16px / ls 0.13px  (identical to desktop)
  2x-small-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.25}"                # 6px
    fontWeight: "{font.weight.inter.600}"             # 600 Semi Bold
    lineHeight: "{line-height.desktop.100}"           # 16px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 6px / 16px / ls 0.13px  (identical to desktop)
  label-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.nunito sans.800}"       # 800 Extra Bold
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 12px / 20px / ls 0.13px
  label-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 12px / 20px / ls 0.13px
  label-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.nunito sans.600}"       # 600 Semi Bold
    lineHeight: "{line-height.desktop.400}"           # 22px
    letterSpacing: "{letter-spacing.10}"              # 0.13px
    # mobile → 12px / 20px / ls 0.13px
  button-label-lg:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.400}"               # 16px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.500}"           # 24px
    letterSpacing: "{letter-spacing.40}"              # 0.4px
    # mobile → 16px / 24px / ls 0.4px  (identical to desktop)
  button-label-md:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.300}"               # 14px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.500}"           # 24px
    letterSpacing: "{letter-spacing.30}"              # 0.25px
    # mobile → 14px / 24px / ls 0.25px  (identical to desktop)
  button-label-sm:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.200}"               # 12px
    fontWeight: "{font.weight.nunito sans.700}"       # 700 Bold
    lineHeight: "{line-height.desktop.500}"           # 24px
    letterSpacing: "{letter-spacing.20}"              # 0.15px
    # mobile → 12px / 24px / ls 0.15px  (identical to desktop)
# Mirrors "Border - Semantic" border.radius.* 1:1 (so {rounded.X} == {border.radius.X}).
# v4 renumbered the scale again: a 3px step (xs) and a 10px step (2xl) were inserted,
# which pushed every step from 2xl upward one slot. Components below are remapped so
# they keep their previous pixel values.
rounded:
  2xs: "{border.radius.2xs}"    # 2px
  xs: "{border.radius.xs}"      # 3px   → new in v4
  sm: "{border.radius.sm}"      # 4px
  md: "{border.radius.md}"      # 5px
  lg: "{border.radius.lg}"      # 6px
  xl: "{border.radius.xl}"      # 8px
  2xl: "{border.radius.2xl}"    # 10px  → new in v4 (12px moved to 3xl)
  3xl: "{border.radius.3xl}"    # 12px  → was 2xl
  4xl: "{border.radius.4xl}"    # 16px  → was 3xl
  5xl: "{border.radius.5xl}"    # 24px  → was 4xl (chip round)
  6xl: "{border.radius.6xl}"    # 30px  → was 5xl
  7xl: "{border.radius.7xl}"    # 100px → was 6xl (label round, tab indicator, badge-dot-xl)
  full: "{border.radius.full}"  # 999px

# Mirrors the "Spacing - Semantic" step names 1:1. The source exposes the same
# scale three times — spacing.padding.*, spacing.gap.horizontal.*, and
# spacing.gap.vertical.* — with identical pixel values. In components below,
# padding properties map to spacing.padding.X and gap properties map to
# spacing.gap.{horizontal|vertical}.X; the alias here is the shared step.
spacing:
  2xs: "{spacing.padding.2xs}"  # 2px   → closes the long-standing 2px gap
  xs: "{spacing.padding.xs}"    # 4px
  sm: "{spacing.padding.sm}"    # 6px   → new in v4
  md: "{spacing.padding.md}"    # 8px
  lg: "{spacing.padding.lg}"    # 10px  → new in v4
  xl: "{spacing.padding.xl}"    # 12px
  2xl: "{spacing.padding.2xl}"  # 16px
  3xl: "{spacing.padding.3xl}"  # 20px  → new in v4
  4xl: "{spacing.padding.4xl}"  # 24px
  5xl: "{spacing.padding.5xl}"  # 32px
  6xl: "{spacing.padding.6xl}"  # 40px
  7xl: "{spacing.padding.7xl}"  # 48px
  8xl: "{spacing.padding.8xl}"  # 56px
  9xl: "{spacing.padding.9xl}"  # 64px
  max: "{spacing.padding.max}"  # 123px → purpose undocumented in source, see Known Gaps

# Border width (Border - Semantic). Values unchanged from the previous update;
# xl (3px) is new and has no consumer yet.
borderWidth:
  sm: "{border.width.sm}"       # 1px
  md: "{border.width.md}"       # 1.5px
  lg: "{border.width.lg}"       # 2px
  xl: "{border.width.xl}"       # 3px → new in v4

# Elevation (Elevation - Semantic x/y/blur/spread) — numeric values unchanged.
# Color uses the brand-navy alpha tints from Colors - Semantic shadow.*.
shadow:
  xs: "0px 1px 4px 1px {shadow.extra-light}"   # navy 7%
  sm: "1px 2px 12px 2px {shadow.light}"         # navy 9%
  md: "1px 6px 20px 4px {shadow.medium}"        # navy 12%
  lg: "1px 2px 40px 4px {shadow.heavy}"         # navy 16%
  xl: "2px 2px 56px 9px {shadow.heavy}"         # navy 16%

components:
  # Legend: "Δ" marks a resolved value that changed vs design.md v4 (visual change).
  # "⚠" marks a binding issue, missing state/token, or accessibility concern.
  # Radius values use ds-v4.json names; where Figma binds a different name it is noted (X1).

  # ─── BUTTON ───────────────────────────────────────────────────────────────
  # Source: Figma HOL Design System 2.0 › page "Button" (109:1553) › component set "New Button" (4873:1238)
  # Matrix: Style (Primary, Secondary, Outline, Text Icon, Light) × Size (Small, Medium, Large)
  #         × State (Default, Hover, Pressed, Disabled, Loading) × Icon (Off = label, On = icon-only)
  button-sm:
    height: 40px                                # no sizing token
    padding: "{spacing.md} {spacing.2xl}"       # 8px 16px
    gap: "{spacing.md}"                         # 8px → spacing.gap.horizontal.md
    label-typography: "{typography.button-label-sm}"
    iconSize: 20px
  button-md:
    height: 48px
    padding: "{spacing.xl} {spacing.4xl}"       # 12px 24px
    gap: "{spacing.md}"
    label-typography: "{typography.button-label-md}"
    iconSize: 20px
  button-lg:
    height: 56px
    padding: "{spacing.2xl} {spacing.4xl}"      # 16px 24px
    gap: "{spacing.md}"
    label-typography: "{typography.button-label-lg}"
    iconSize: 20px
  button-icon-only-sm:
    size: 40px
    padding: "{spacing.md}"                     # 8px ⚠ 8+20+8 = 36 ≠ 40 — padding token does not match the fixed size
  button-icon-only-md:
    size: 48px
    padding: "{spacing.xl}"                     # 12px → 12+20+12 = 48 ✓
  button-icon-only-lg:
    size: 56px
    padding: "{spacing.2xl}"                    # 16px → 16+20+16 = 52 ≠ 56 ⚠ (icon likely 24px here; confirm)
  button-border-radius: "{rounded.lg}"          # 6px
  button-max-characters: 25

  button-primary-default:
    backgroundColor: "{surface.brand-primary.base}"      # #003366
    labelColor: "{text.neutral.inverse}"
    iconColor: "{icon.neutral.inverse}"
  button-primary-hover:
    backgroundColor: "{surface.brand-primary.moderate}"  # #00458a  Δ was muted #0052a3
    labelColor: "{text.neutral.inverse}"
  button-primary-pressed:
    backgroundColor: "{surface.brand-primary.strong}"    # #05213e
    labelColor: "{text.neutral.inverse}"
  button-primary-disabled:
    backgroundColor: "{surface.neutral.soft}"            # #a8b8c7
    labelColor: "{text.neutral.secondary}"
  button-primary-loading:
    backgroundColor: "{surface.neutral.soft}"
    labelColor: "{text.neutral.secondary}"
    spinner: Spinner 20px, leading position (Button page component)

  button-secondary-default:
    backgroundColor: "{surface.brand-secondary.base}"    # #f8ca0f
    labelColor: "{text.brand-primary.base}"
  button-secondary-hover:
    backgroundColor: "{surface.brand-secondary.subtle}"  # #ffe168
    labelColor: "{text.brand-primary.base}"
  button-secondary-pressed:
    backgroundColor: "{surface.warning.base}"            # #daa520 — resolves former ⚠ undefined token, but borrows a status role; see notes
    labelColor: "{text.brand-primary.base}"              # 5.63:1
  button-secondary-disabled:
    backgroundColor: "{surface.neutral.soft}"
    labelColor: "{text.neutral.secondary}"

  button-outline-default:
    backgroundColor: "transparent"
    borderColor: "{border.state.interactive}"            # #0052a3
    borderWidth: "{border.width.sm}"                     # 1px  Δ was md 1.5px
    labelColor: "{text.brand-primary.base}"
  button-outline-hover:
    backgroundColor: "{surface.info.soft}"               # #ebf6fc  Δ was brand-primary.lighter #e0ecf9; info role on a brand component
    borderColor: "{border.state.interactive}"
    labelColor: "{text.brand-primary.base}"
  button-outline-pressed:
    backgroundColor: "{surface.brand-primary.soft}"      # #89bff4
    borderColor: "{border.state.interactive}"
    labelColor: "{text.brand-primary.base}"
  button-outline-disabled:
    backgroundColor: "{surface.neutral.lightest}"
    borderColor: "{border.neutral.default}"              # #a8b8c7  Δ was border.state.disabled #cfd9e2
    labelColor: "{text.neutral.secondary}"

  button-text-icon-default:                             # renamed from "tertiary" to match Figma
    backgroundColor: "transparent"
    labelColor: "{text.brand-primary.base}"
  button-text-icon-hover:
    backgroundColor: "transparent"
    labelColor: "{text.info.base}"                       # #2877c5  Δ was brand-primary.muted; info role on a brand component
  button-text-icon-pressed:
    backgroundColor: "transparent"
    labelColor: "{text.info.base}"
  button-text-icon-disabled:
    backgroundColor: "transparent"
    labelColor: "{text.neutral.secondary}"

  button-light-default:                                 # NEW style — for dark / navy surfaces
    backgroundColor: "transparent"
    borderColor: "{border.inverse.inverse-weak}"         # white @ 30%
    borderWidth: "{border.width.sm}"
    labelColor: "{text.neutral.inverse}"
  button-light-hover:
    backgroundColor: "{surface.overlay.inverse}"         # white @ 30%
    borderColor: "{border.inverse.inverse}"              # white
    labelColor: "{text.neutral.inverse}"
  button-light-pressed:
    backgroundColor: "{surface.overlay.default-weak}"    # navy-1100 @ 30%
    borderColor: "{border.inverse.inverse-weak}"
    labelColor: "{text.neutral.inverse}"
  button-light-disabled:
    backgroundColor: "transparent"
    borderColor: "{border.inverse.inverse-weak}"
    labelColor: "{text.neutral.tertiary}"

  # ─── INPUT & FORM ─────────────────────────────────────────────────────────
  # Source: Figma › page "Input & Form" (1436:12081) › component set "Input" (1672:13449)
  # Matrix: Type (Field, Text Area) × State (Default, Filled, Active, Failed, Success*, Disabled)
  #         * Success exists for Field only. Props: label, helperText, leftIcon (Field only), rightIcon.
  input:
    width: 256px                                # default; stretches to container
    gap-label-field-helper: "{spacing.xs}"      # 4px → spacing.gap.vertical.xs
    label-typography: "{typography.caption-medium}"
    labelColor: "{text.neutral.primary}"
    value-typography: "{typography.body-3-medium}"
    helper-typography: "{typography.caption-medium}"
    borderRadius: "{rounded.md}"                # 5px
    iconSize: 20px
    iconColor: "{icon.neutral.muted}"
  input-field:
    height: 48px                                # no sizing token
    paddingLeft: "{spacing.2xl}"                # 16px
    paddingRight: "{spacing.md}"                # 8px
    paddingVertical: "{spacing.md}"             # 8px
    gap: "{spacing.md}"                         # icon ↔ text
  input-textarea:
    minHeight: 82px                             # field box only
    padding: "{spacing.md}"                     # 8px all sides  Δ was 16px left
    gap: "{spacing.md}"
    trailingIcon: copy (top-right)

  input-default:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.state.disabled}"      # #cfd9e2  Δ was border.neutral.default #a8b8c7 ⚠ disabled role on an enabled state; 1.43:1 on white
    borderWidth: "{border.width.sm}"            # 1px  Δ was lg 2px
    valueColor: "{text.neutral.tertiary}"       # placeholder
    helperColor: "{text.neutral.secondary}"
  input-filled:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.state.disabled}"      # ⚠ same as default
    borderWidth: "{border.width.sm}"
    valueColor: "{text.neutral.primary}"
    helperColor: "{text.neutral.secondary}"
  input-active:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.state.active}"        # #2877c5
    borderWidth: "{border.width.md}"            # Field 1.5px · Text Area 1px ⚠ inconsistent
    valueColor: "{text.neutral.primary}"
    helperColor: "{text.neutral.secondary}"
  input-failed:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.status.danger}"
    borderWidth: "{border.width.md}"            # 1.5px
    trailingIcon: warning-circle
    iconColor: "{icon.danger.base}"
    valueColor: "{text.neutral.primary}"
    helperColor: "{text.danger.base}"
  input-success:                                # Field only
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.status.success}"
    borderWidth: "{border.width.md}"
    iconColor: "{icon.success.base}"            # ⚠ duplicate variant in Figma uses surface.success.base for the icon
    valueColor: "{text.neutral.primary}"
    helperColor: "{text.success.base}"
  input-disabled:
    backgroundColor: "{surface.neutral.lightest}"
    borderColor: "{border.state.disabled}"
    borderWidth: "{border.width.sm}"
    valueColor: "{text.neutral.tertiary}"
    helperColor: "{text.neutral.secondary}"

  # ─── CHECKBOX ─────────────────────────────────────────────────────────────
  # Source: Figma › page "Checkbox" (5294:1901) › "Checkbox" (5294:1903) + sub-component "Check" (5294:1928)
  # Matrix: Device (Desktop, Mobile) × Status (Default, Active, Disabled Default, Disabled Active)
  #         Check sub-component also has State=Indeterminate (not exposed on Checkbox).
  checkbox:
    height: 24px                                # Desktop; Mobile hugs content (20px)
    gap: "{spacing.md}"                         # 8px box ↔ label → spacing.gap.horizontal.md
    label-typography: "{typography.body-3-medium}"   # Desktop 14/22 · Mobile 12/20 (mode)
    hitArea: box + label                        # whole row is clickable
  checkbox-box:
    size: 16px
    borderRadius: "{rounded.sm}"                # 4px
    borderWidth: "{border.width.sm}"            # 1px
    checkIconSize: 16px

  checkbox-default:
    boxBackground: "{surface.neutral.white}"
    boxBorder: "{border.neutral.default}"       # #a8b8c7 ⚠ 2.03:1 on white (WCAG 1.4.11 needs 3:1)
    labelColor: "{text.neutral.primary}"
  checkbox-active:                              # checked
    boxBackground: "{surface.brand-primary.subtle}"   # #2877c5
    checkColor: "{icon.neutral.inverse}"
    labelColor: "{text.neutral.primary}"
  checkbox-indeterminate:                       # available on Check only
    boxBackground: "{surface.brand-primary.subtle}"
    dash: 8×2px, "{icon.neutral.inverse}", radius "{rounded.2xs}"
  checkbox-disabled-default:
    boxBackground: "{surface.neutral.lightest}"
    boxBorder: "{border.neutral.default}"
    labelColor: "{text.neutral.tertiary}"
  checkbox-disabled-active:
    boxBackground: "{surface.neutral.lightest}"
    boxBorder: "{border.neutral.default}"
    checkColor: "{icon.neutral.subtle}"         # #8398ab
    labelColor: "{text.neutral.tertiary}"

  # ─── RADIO ────────────────────────────────────────────────────────────────
  # Source: Figma › page "Radio" (5294:1947) › "Radio Button" (5294:1949) + sub-component "Radio" (136:1570)
  # Matrix: Device (Desktop, Mobile) × Status (Default, Active, Disabled Default, Disabled Active) — mirrors Checkbox
  radio:
    height: 24px                                # Desktop; Mobile hugs content
    gap: "{spacing.md}"                         # 8px control ↔ label
    label-typography: "{typography.body-3-medium}"   # Desktop 14/22 · Mobile 12/20 (mode)
    label-align: left                           # ⚠ Figma text is center-aligned; breaks multi-line wrapping
    hitArea: control + label
    selection: single per group
  radio-control:
    size: 16px
    borderRadius: "{rounded.full}"
    borderWidth: "{border.width.sm}"            # 1px

  radio-default:
    controlBackground: "{surface.neutral.white}"
    controlBorder: "{border.neutral.default}"   # #a8b8c7 ⚠ 2.03:1 (WCAG 1.4.11)
    labelColor: "{text.neutral.primary}"
  radio-active:
    controlBackground: "{surface.brand-primary.subtle}"   # #2877c5 ring
    dotColor: "{surface.neutral.white}"                   # inner dot (flattened vector) ⚠
    labelColor: "{text.neutral.primary}"
  radio-disabled-default:
    controlBackground: "{surface.neutral.lightest}"
    controlBorder: "{border.neutral.default}"
    labelColor: "{text.neutral.tertiary}"
  radio-disabled-active:
    controlBackground: "{surface.neutral.lightest}"
    controlBorder: "{border.neutral.default}"
    dotColor: "{surface.neutral.subtle}"                  # #8398ab
    labelColor: "{text.neutral.tertiary}"

  # ─── TOGGLE ───────────────────────────────────────────────────────────────
  # Source: Figma › page "Toggle" (5294:1851) › "Toggle" (5294:1853) + sub-component "Switch Toggle" (5294:1878)
  # Matrix: Status (On, Off, Disabled On, Disabled Off) × Device (Desktop, Mobile)
  #         ⚠ Mobile variants are named Status5–Status8 in Figma
  toggle:
    height: 24px
    gap: "{spacing.md}"                         # 8px switch ↔ label
    label-typography: "{typography.body-3-medium}"   # Desktop 14/22 · Mobile 12/20 (mode)
    hitArea: switch only                        # per Figma docs — label is not clickable ⚠ see notes
    behavior: immediate effect on press; no separate save action
  toggle-switch:
    size: 32 × 20px
    borderRadius: "{rounded.full}"
    handleColor: "{icon.neutral.inverse}"       # white
    construction: flattened vector ⚠ — track/handle not built from token-bound layers

  toggle-on:           { trackColor: "{surface.brand-primary.subtle}", labelColor: "{text.neutral.primary}" }   # #2877c5
  toggle-off:          { trackColor: "{surface.neutral.soft}",         labelColor: "{text.neutral.primary}" }   # #a8b8c7 — white handle on track 2.03:1 ⚠
  toggle-disabled-on:  { trackColor: "{surface.brand-primary.soft}",   labelColor: "{text.neutral.tertiary}" }  # #89bff4
  toggle-disabled-off: { trackColor: "{surface.neutral.lighter}",      labelColor: "{text.neutral.tertiary}" }  # #cfd9e2

  # ─── CHIP ─────────────────────────────────────────────────────────────────
  # Source: Figma › page "Chip" (766:8349) › component set "New Chip" (5049:626)
  # Matrix: Size (Small, Medium, Large) × State (Default, Hover, Active, Pressed, Disabled)
  #         × Corner (Rounded, Square) = 30 variants. Props: showLeftBadges, showRightBadges (16px icon).
  chip-sm:
    height: 26px
    padding: "{spacing.xs} {spacing.md}"        # 4px 8px ⚠ 4+20+4 = 28 > 26 (fixed height clips padding)
    typography: "{typography.caption-medium}"   # 12/20
    borderRadiusSquare: "{rounded.xs}"          # 3px  Δ was 5px for all sizes
  chip-md:
    height: 30px
    padding: "{spacing.xs} {spacing.md}"        # 4px 8px
    typography: "{typography.body-3-medium}"
    borderRadiusSquare: "{rounded.sm}"          # 4px  Δ was 5px
  chip-lg:
    height: 36px
    padding: "{spacing.xs} {spacing.xl}"        # 4px 12px
    typography: "{typography.body-3-medium}"
    borderRadiusSquare: "{rounded.md}"          # 5px
  chip-border-radius-round: "{rounded.5xl}"     # 24px — Figma binds border/radius/6xl (=24 in Figma; =30 in ds-v4.json) ⚠ token value mismatch
  chip-gap: "{spacing.md}"                      # icon ↔ label
  chip-iconSize: 16px
  chip-max-characters: 25

  chip-default:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.state.disabled}"      # #cfd9e2  Δ was border.neutral.default #a8b8c7 ⚠ disabled role on enabled state; 1.43:1
    borderWidth: "{border.width.sm}"            # 1px  Δ was 1.5px
    labelColor: "{text.neutral.primary}"
  chip-hover:
    backgroundColor: "{surface.brand-primary.lighter}"
    borderColor: "{border.state.interactive}"
    borderWidth: "{border.width.sm}"
    labelColor: "{text.neutral.primary}"
  chip-active:
    backgroundColor: "{surface.brand-primary.base}"
    labelColor: "{text.neutral.inverse}"
  chip-pressed:
    backgroundColor: "{surface.brand-primary.strong}"
    labelColor: "{text.neutral.inverse}"
  chip-disabled:
    backgroundColor: "{surface.neutral.lighter}"
    borderColor: "{border.neutral.default}"     # #a8b8c7  Δ was border.state.interactive (resolves earlier gap)
    borderWidth: "{border.width.sm}"
    labelColor: "{text.neutral.tertiary}"       # Δ was text.neutral.primary

  # ─── LABEL ────────────────────────────────────────────────────────────────
  # Source: Figma › page "Label" (6040:4277) › component set "Label" (6040:3944)
  # Matrix: Color (Dark, Light, Red, Green, Yellow, Blue) × Style (Default, Outline, Solid)
  #         × Type (Square, Round) = 36 variants. Props: text, showIcon (16px, leading).
  label:
    height: 24px
    padding: "{spacing.xs} {spacing.md}"        # 4px 8px  Δ vertical was 2px ⚠ 4+20+4 = 28 > 24
    gap: "{spacing.xs}"                         # 4px icon ↔ text → spacing.gap.horizontal.xs
    typography: "{typography.caption-medium}"
    iconSize: 16px
    borderRadiusSquare: "{rounded.sm}"          # 4px
    borderRadiusRound: "{rounded.7xl}"          # 100px — Figma binds border/radius/8xl, which does not exist in ds-v4.json ⚠
    borderWidthOutline: "{border.width.sm}"     # 1px
    width: hug                                  # ⚠ most variants are fixed at 48px (Square) / 52px (Round) in Figma
    max-characters: 25                          # guideline: 10–25

  label-dark-default:  { backgroundColor: "{surface.info.soft}", textColor: "{text.brand-primary.base}" }                 # Δ bg was brand-primary.lighter
  label-dark-outline:  { backgroundColor: "{surface.info.soft}", textColor: "{text.brand-primary.base}", borderColor: "{border.state.interactive}" }
  label-dark-solid:    { backgroundColor: "{surface.brand-primary.base}", textColor: "{text.neutral.inverse}" }

  label-light-default: { backgroundColor: "{surface.neutral.lightest}", textColor: "{text.brand-primary.base}" }
  label-light-outline: { backgroundColor: "{surface.neutral.lightest}", textColor: "{text.brand-primary.base}", borderColor: "{border.state.disabled}" }   # Δ was neutral.default
  label-light-solid:   { backgroundColor: "{surface.neutral.lighter}", textColor: "{text.neutral.primary}" }

  label-red-default:   { backgroundColor: "{surface.danger.soft}", textColor: "{text.danger.strong}" }
  label-red-outline:   { backgroundColor: "{surface.danger.soft}", textColor: "{text.danger.strong}", borderColor: "{border.status.danger}" }
  label-red-solid:     { backgroundColor: "{surface.danger.base}", textColor: "{text.neutral.inverse}" }

  label-green-default: { backgroundColor: "{surface.success.soft}", textColor: "{text.success.strong}" }
  label-green-outline: { backgroundColor: "{surface.success.soft}", textColor: "{text.success.strong}", borderColor: "{border.status.success}" }
  label-green-solid:   { backgroundColor: "{surface.success.base}", textColor: "{text.neutral.inverse}" }

  label-yellow-default: { backgroundColor: "{surface.warning.soft}", textColor: "{text.brand-secondary.strong}" }   # #8d7101  Δ was warning.strong #6f4e37 — resolves off-hue issue
  label-yellow-outline: { backgroundColor: "{surface.warning.soft}", textColor: "{text.brand-secondary.strong}", borderColor: "{border.status.warning}" }
  label-yellow-solid:   { backgroundColor: "{surface.warning.base}", textColor: "{text.neutral.inverse}" }          # ⚠ still 2.24:1

  label-blue-default:  { backgroundColor: "{surface.info.soft}", textColor: "{text.brand-primary.muted}" }          # Δ text was info.strong #00458a
  label-blue-outline:  { backgroundColor: "{surface.info.soft}", textColor: "{text.brand-primary.muted}", borderColor: "{border.state.active}" }   # resolves ⚠ border.status.info
  label-blue-solid:    { backgroundColor: "{surface.brand-primary.muted}", textColor: "{text.neutral.inverse}" }    # #0052a3  Δ was info.base #2877c5

  # ─── BADGES ───────────────────────────────────────────────────────────────
  # Source: Figma › page "Badges" (5486:3098) › component set "Badges" (2987:13883)
  # Matrix: Style (light, dark) × Type (Image, Text, Icon, Icon No Fill, dot) × Size (S, M, L, XL) = 40 variants
  badge:
    borderRadius: "{rounded.full}"              # Icon variants bind primitive radius/full instead of border/radius/full ⚠
    padding: "{spacing.xs}"                     # 4px (Text, Icon)
  badge-size:      { S: 16px, M: 20px, L: 32px, XL: 48px }   # ⚠ dark Text XL is 40px in Figma
  badge-light:     { backgroundColor: "{surface.neutral.lighter}", contentColor: "{text.brand-primary.base}" }
  badge-dark:      { backgroundColor: "{surface.brand-primary.base}", contentColor: "{text.neutral.inverse}" }

  badge-text:                                   # max 2 characters
    S:  "{typography.2x-small-semibold}"        # 6/16
    M:  "{typography.extra-small-semibold}"     # 8/16
    L:  "{typography.small-semibold}"           # 10/16
    XL: "{typography.body-2-semibold}"          # 16/26
  badge-icon:                                   # filled container
    iconSize: { S: 8px, M: 12px, L: 22px, XL: 30px }
  badge-icon-no-fill:                           # icon only, no container
    size: { S: 12px, M: 16px, L: 24px, XL: 40px }   # ⚠ off the 16/20/32/48 badge scale
    iconSize: { S: 12px, M: 16px, L: 24px, XL: 32px }
  badge-image:
    size: same as badge-size
    dark: separated from stacked avatars by a light ring (flattened in Figma; not token-bound) ⚠

  badge-dot:                                    # notification
    backgroundColor: "{surface.danger.base}"
    labelColor: "{text.neutral.inverse}"
    S:  { dot: 6px }                            # ⚠ flattened image — colour not bound to a token
    M:  { dot: 10px }                           # ⚠ flattened image
    L:  { size: 16px, typography: "{typography.extra-small-semibold}", maxChars: 2 }
    XL: { size: 32×20px, borderRadius: "{rounded.6xl}", typography: "{typography.small-semibold}", maxChars: 3 }   # "99+"; Figma binds border/radius/7xl (=30) ⚠
    dark: 1px "{border.inverse.inverse}" ring around the dot

  # ─── ALERT ────────────────────────────────────────────────────────────────
  # Source: Figma › page "Alert" (3343:2206) › component set "Alert" (3346:4327)
  # Matrix: State (Info, Warning, Failed, Success, Neutral) × Size (Medium = mobile, Large = desktop)
  # Props: showLeftIcon, showRightIcon (close), showDescription (Large), showButton (2 actions)
  alert:
    padding: "{spacing.2xl}"                    # 16px
    borderRadius: "{rounded.lg}"                # 6px
    borderWidth: "{border.width.sm}"            # 1px
    iconSize: 24px                              # leading status icon + trailing close (XCircle)
    gap-icon-content: "{spacing.md}"            # 8px
    gap-title-description: "{spacing.xs}"       # 4px
    gap-actions: "{spacing.2xl}"                # 16px between action buttons
    title-typography: "{typography.body-1-bold}"        # 18/28 desktop · 16/26 mobile
    description-typography: "{typography.body-3-medium}" # 14/22 desktop · 12/20 mobile
    descriptionColor: "{text.neutral.secondary}"
    closeIconColor: "{icon.neutral.subtle}"
    actions: button-sm text-icon (secondary action) + button-sm primary (primary action)
    max-characters: 100                         # title + description
    duration: 3–5s auto-dismiss unless persistent
    position: fixed, top-center of viewport
  alert-md:                                     # mobile
    width: 320px
    layout: vertical — header row (icon · title · close), description, actions right-aligned
  alert-lg:                                     # desktop
    width: 1120px                               # container width
    layout: horizontal — icon · title/description · actions · close
    gap: "{spacing.2xl}"

  alert-info:    { backgroundColor: "{surface.info.soft}",     borderColor: "{border.state.active}",    iconColor: "{icon.info.base}",       titleColor: "{text.info.strong}" }
  alert-success: { backgroundColor: "{surface.success.soft}",  borderColor: "{border.status.success}",  iconColor: "{icon.success.base}",    titleColor: "{text.success.strong}" }
  alert-warning: { backgroundColor: "{surface.warning.soft}",  borderColor: "{border.status.warning}",  iconColor: "{icon.warning.strong}",  titleColor: "{text.warning.strong}" }   # ⚠ title #6f4e37 off-hue; Label uses brand-secondary.strong
  alert-failed:  { backgroundColor: "{surface.danger.soft}",   borderColor: "{border.status.danger}",   iconColor: "{icon.danger.base}",     titleColor: "{text.danger.strong}" }
  alert-neutral: { backgroundColor: "{surface.neutral.lightest}", borderColor: "{border.neutral.default}", iconColor: "{icon.neutral.base}", titleColor: "{text.neutral.primary}" }

  # ─── TOOLTIP ──────────────────────────────────────────────────────────────
  # Source: Figma › page "Tooltip" (5153:360) › component set "Tooltip" (5158:961)
  # Matrix: Pointer (Up, Down, Left, Right) × Position (Left/Center/Right for Up·Down; Top/Center/Bottom for Left·Right)
  #         × Colour (Default, Dark, Light) = 36 variants. Prop: text.
  tooltip:
    padding: "{spacing.md} {spacing.xl}"        # 8px 12px
    borderRadius: "{rounded.md}"                # 5px
    typography: "{typography.caption-medium}"   # 12/20
    elevation: "1px 6px 20px 4px {shadow.light}"   # same hybrid as Back to Top ⚠
    pointer: 8.66 × 5.25px triangle             # flattened vector — colour not token-bound ⚠
    offset: 4px                                 # pointer tip ↔ target, desktop & mobile
    viewportPadding: 16px                       # max distance kept from viewport edge
    maxCharacters: 250                          # width hugs content; wrap beyond max width
    motion: fade + short slide from the target; optional delay before show
    placement: auto-flips to available space
  tooltip-default: { backgroundColor: "{surface.brand-primary.moderate}", textColor: "{text.neutral.inverse}" }   # #00458a, 9.47:1 — doc text still says "Info-500"
  tooltip-dark:    { backgroundColor: "{surface.neutral.strong}",         textColor: "{text.neutral.inverse}" }   # #162533 — for light backgrounds
  tooltip-light:   { backgroundColor: "{surface.neutral.lighter}",        textColor: "{text.neutral.primary}" }   # #cfd9e2 — for dark backgrounds

  # ─── COACHMARK ────────────────────────────────────────────────────────────
  # Source: Figma › page "Coachmark" (5976:1665) › component set "Coachmark" (6813:2843) + "Skip or X" (11132:16044)
  # Matrix: Pointer (Up, Down, Left, Right) × Position (3 per pointer) × Colour (Default, Dark, Light) = 36 variants
  # Props: title, description, counter + counterNumber ("1 of 3"), doubleButton, singleButton
  coachmark:
    width: 370px                                # desktop max · 320px on mobile
    padding: "{spacing.2xl}"                    # 16px
    borderRadius: "{rounded.lg}"                # 6px
    elevation: "1px 2px 40px 4px {shadow.medium}"   # lg geometry with navy 12% (shadow.lg uses 16%) ⚠ hybrid
    pointer: 16 × 10px                          # flattened vector ⚠
    gap-sections: "{spacing.2xl}"               # 16px content ↔ footer
    gap-title-description: "{spacing.md}"       # 8px
    gap-actions: "{spacing.xl}"                 # 12px
    title-typography: "{typography.body-3-bold}"
    description-typography: "{typography.caption-medium}"
    counter-typography: "{typography.caption-medium}"   # ⚠ unbound (raw Inter 12, ls 0.048) in single-button footer
    dismiss: Skip-or-X — Text ("Lewati", button-label-sm) or Icon (X 12px)
    actions:
      previous: outline button-sm ("Sebelumnya")
      next: secondary button-sm + CaretRight 18px ("Selanjutnya")
    behavior: anchored to target; pointer re-positions and flips when space is insufficient; shifts to avoid nearby elements; keep title/description short

  coachmark-default:
    backgroundColor: "{surface.brand-primary.moderate}"   # #00458a
    titleColor: "{text.brand-secondary.base}"             # gold #f8ca0f, 6.06:1
    descriptionColor: "{text.neutral.muted}"              # #f5f7f9
    counterColor: "{text.neutral.inverse}"
    dismissColor: "{text.neutral.inverse}"
    previous: { borderColor: "{border.inverse.inverse}", labelColor: "{text.neutral.inverse}" }
    next:     { backgroundColor: "{surface.brand-secondary.base}", labelColor: "{text.info.strong}" }   # ⚠ info role; single-button variant uses text.brand-primary.base
  coachmark-dark:
    backgroundColor: "{surface.neutral.strong}"           # #162533
    titleColor: "{text.brand-secondary.base}"
    descriptionColor: "{text.neutral.muted}"
    previous: { borderColor: "{border.inverse.inverse}", labelColor: "{text.neutral.inverse}" }
    next:     { backgroundColor: "{surface.brand-secondary.base}", labelColor: "{text.info.strong}" }
  coachmark-light:
    backgroundColor: "{surface.neutral.lightest}"         # #f5f7f9
    titleColor: "{text.brand-primary.muted}"              # #0052a3
    descriptionColor: "{text.neutral.primary}"
    counterColor: "{text.neutral.primary}"
    dismissColor: "{text.neutral.primary}"
    previous: { borderColor: "{border.state.interactive}", labelColor: "{text.info.strong}" }
    next:     { backgroundColor: "{surface.brand-secondary.base}", labelColor: "{text.info.strong}" }

  # ─── LOADER ───────────────────────────────────────────────────────────────
  # Source: Figma › page "Loader" (12724:30226) › component "Loading State - HOL Logo" (3254:1486)
  # Single component (animated HOL logo, raster/GIF asset). Sizes are documented, not built as variants.
  loader:
    asset: animated HOL logo (GIF; "LINK GIF" on canvas)   # raster — no colour tokens apply
    sizes: { sm: 16px, md: 24px, lg: 40px }                 # ⚠ component itself is 160px; sizes exist only in docs
    type: indeterminate
    usage:
      - short, indeterminate waits where completion time cannot be predicted
      - partial UI updates: loading a content section, refreshing data, fetching quick results
      - confirms the system is responding; does not communicate progress
    do-not: long or measurable processes → use Progress Bar (related component)
    accessibility: expose role="status" / aria-busy on the loading region; respect prefers-reduced-motion   # recommendation, not in Figma
  # Related (not documented here): Progress Bar (2472:13597), Bar (2470:13557).
  # Note: Button loading state uses a separate "Spinner" component (Button page), not this loader.

  # ─── BACK TO TOP ──────────────────────────────────────────────────────────
  # Source: Figma › page "Back to Top" (2190:15521) › component set "Back to Top" (8708:7497)
  # Variants: Style = With Text | Icon. Prop: text (default "Back to Top").
  back-to-top:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.state.disabled}"      # #cfd9e2 — same pattern as Input / Chip default
    borderWidth: "{border.width.sm}"            # 1px
    borderRadius: "{rounded.6xl}"               # 30px pill — Figma binds border/radius/7xl (=30 in Figma; 7xl=100 in ds-v4.json) ⚠
    elevation: "1px 6px 20px 4px {shadow.light}"   # md geometry with navy 9% (shadow.md uses navy 12%) ⚠ hybrid
    iconSize: 24px                              # ArrowLineUp
    iconColor: "{icon.brand-primary.base}"
    gap: "{spacing.md}"                         # 8px
  back-to-top-with-text:
    height: 40px
    padding: "{spacing.md} {spacing.2xl}"       # 8px 16px
    label-typography: "{typography.button-label-md}"   # Nunito Sans Bold 14/24
    labelColor: "{text.brand-primary.base}"
    position: bottom-center
    useCase: inner scroll — article, document, PDF
  back-to-top-icon:
    size: 48px
    padding: "{spacing.md} {spacing.2xl}"       # ⚠ 16+24+16 = 56 > 48 (fixed size overrides padding)
    position: bottom-right
    useCase: regular scroll — landing page, catalogue
  back-to-top-behavior:
    visibility: page height ≥ 4× above-the-fold (desktop 3072px · mobile 3200px)
    stacking: lowest priority among floating elements; shifts to avoid overlapping floating buttons (e.g. WhatsApp)
    interaction: smooth-scroll to top

  # ─── BREADCRUMB ───────────────────────────────────────────────────────────
  # Source: Figma › page "Breadcrumb" (5294:1430) › component set "New Breadcumb" (6809:3918)
  #         atoms: home (19207:42674), Level (19207:42687), DotsThree (19207:42704), Dropdown (19207:42711)
  # Matrix: Type (Dashboard = leading home icon, Media = leading "Beranda" text) × Color (Default, Dark) × Level (2, 3, 4, 4+)
  # Legacy set "Breadcumb" (5294:1709, Device × Level) is superseded and not documented.
  breadcrumb:
    height: 24px
    gap: "{spacing.xs}"                         # 4px between items and separators
    typography: "{typography.body-3-medium}"
    separator: CaretRight 14px
    homeIcon: 20px                              # Dashboard type
    overflow: Level 4+ collapses middle levels into DotsThree (20px) → Dropdown listing hidden levels
    maxCharacters: { desktop: 20, mobile: 10 }  # per level, then truncate with "…"
    maxVisibleLevels: 4
    currentPage: last item, non-interactive
  breadcrumb-default:                           # on light backgrounds
    linkColor: "{text.brand-primary.base}"
    homeIconColor: "{icon.brand-primary.base}"
    separatorColor: "{icon.neutral.muted}"      # #607a93
    currentColor: "{text.neutral.secondary}"    # ⚠ Media L2–L4 render the current item in brand-primary.base, not secondary
  breadcrumb-dark:                              # on navy backgrounds
    linkColor: "{text.neutral.inverse}"
    homeIconColor: "{icon.neutral.inverse}"
    separatorColor: "{icon.neutral.muted}"      # ⚠ #607a93 on #003366 = 2.82:1
    currentColor: "{text.neutral.quaternary}"   # #a8b8c7, 6.21:1 on #003366
  breadcrumb-level-states:                      # atom "Level" — Type names are inverted vs. parent (atom "Dark" = light bg)
    onLight: { default: "{text.brand-primary.base}", hover: "{text.info.base}",    pressed: "{text.brand-primary.muted}", disabled: "{text.neutral.secondary}" }
    onDark:  { default: "{text.neutral.inverse}",    hover: "{text.brand-primary.soft}", pressed: "{text.info.base}",     disabled: "{text.neutral.quaternary}" }   # ⚠ pressed #2877c5 on navy = 2.72:1

  # ─── PAGINATION ───────────────────────────────────────────────────────────
  # Source: Figma › page "Pagination" (5294:1989) › "pagination" (5294:2016) + atoms "molecule/pagination" (5294:1991)
  # Variants: State = Default (≤5 pages), Left (current near start), Centered (current in middle), Right (current near end), no_number (arrows only)
  pagination:
    itemSize: 32px                              # square
    gap: "{spacing.2xl}"                        # 16px between items
    itemPadding: "{spacing.xs}"                 # 4px
    borderRadius: "{rounded.sm}"                # 4px
    typography: "{typography.body-3-bold}"
    iconSize: 16px                              # CaretLeft / CaretRight
    truncation: ellipsis item replaces hidden ranges when pages exceed display limit
    placement: below the content it paginates, aligned with the result summary ("Showing 1–14 of 200 entries")
  pagination-number-default: { borderColor: "{border.state.disabled}", borderWidth: "{border.width.sm}", textColor: "{text.brand-primary.base}" }   # ⚠ disabled role on enabled item
  pagination-number-active:  { backgroundColor: "{surface.brand-primary.base}", textColor: "{text.neutral.inverse}" }                          # current page → aria-current="page"
  pagination-arrow-default:  { borderColor: "{border.state.disabled}", borderWidth: "{border.width.sm}", iconColor: "{icon.brand-primary.base}" }
  pagination-arrow-hover:    { backgroundColor: "{surface.brand-primary.moderate}", iconColor: "{icon.neutral.inverse}" }   # #00458a
  pagination-arrow-pressed:  { backgroundColor: "{surface.brand-primary.subtle}",   iconColor: "{icon.neutral.inverse}" }   # #2877c5 ⚠ lighter than hover (inverse of Button)
  pagination-ellipsis:       { color: "{surface.neutral.subtle}" }   # #8398ab, flattened vector ⚠
  # ⚠ Missing: hover/pressed for number items, disabled arrow (first/last page), focus-visible.

  # ─── CARRIED OVER FROM v4 (not re-specified from Figma in v4.1) ──────────
  # ─── TAB ──────────────────────────────────────────────────────────────────
  tab:
    height: 40px
    indicatorHeight: 4px
    indicatorBorderRadius: "{rounded.7xl}"      # 100px (was rounded.6xl)
    iconSize: 16px
    typography: "{typography.body-3-medium}"    # no longer matches button-md label (now Nunito Sans) — see Known Gaps

  tab-default:
    labelColor: "{text.neutral.primary}"
    iconColor: "{icon.neutral.soft}"
  tab-hover:
    labelColor: "{text.brand-primary.muted}"
    iconColor: "{icon.neutral.soft}"
  tab-active:
    labelColor: "{text.neutral.primary}"
    iconColor: "{icon.neutral.soft}"
    indicatorColor: "{surface.brand-secondary.base}"
  tab-disabled:
    labelColor: "{text.neutral.tertiary}"
    iconColor: "{icon.neutral.soft}"

  # ─── CARD ARTICLE — FEATURED ──────────────────────────────────────────────
  # Gaps were prose-only before v4; spacing.gap.* now exists, so they are tokenized.
  card-article-featured:
    thumbnail-width: 256px
    thumbnail-height: 160px
    thumbnail-border-radius: "{rounded.sm}"     # 4px
    gap-thumbnail-content: "{spacing.2xl}"      # 16px → spacing.gap.horizontal.2xl
    gap-content: "{spacing.xs}"                 # 4px  → spacing.gap.vertical.xs
    gap-metadata: "{spacing.2xl}"               # 16px → spacing.gap.horizontal.2xl (date ↔ author)
    gap-list: "{spacing.5xl}"                   # 32px → spacing.gap.vertical.5xl
    title-typography: "{typography.body-1-semibold}"  # Δ v4: letter-spacing 0 → 0.13px
    desc-typography: "{typography.body-2-regular}"
    date-typography: "{typography.body-3-medium}"
    author-typography: "{typography.body-3-medium}"
    titleColor: "{text.neutral.primary}"
    descColor: "{text.neutral.primary}"
    dateColor: "{text.neutral.secondary}"
    authorColor: "{text.brand-primary.muted}"

  # ─── CARD ARTICLE — GRID ──────────────────────────────────────────────────
  card-article-grid:
    thumbnail-width: 160px
    thumbnail-height: 256px
    thumbnail-border-radius: "{rounded.md}"     # 5px
    gap-thumbnail-content: "{spacing.md}"       # 8px  → spacing.gap.vertical.md
    gap-content: "{spacing.xs}"                 # 4px  → spacing.gap.vertical.xs
    gap-grid: "{spacing.5xl}"                   # 32px → spacing.gap.horizontal/vertical.5xl
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-medium}"
    titleColor: "{text.neutral.primary}"
    dateColor: "{text.neutral.secondary}"

  # ─── CARD ARTICLE — SIDE ──────────────────────────────────────────────────
  card-article-side:
    thumbnail-width: 176px
    thumbnail-height: 117px
    thumbnail-border-radius: "{rounded.md}"     # 5px
    gap-thumbnail-content: "{spacing.2xl}"      # 16px → spacing.gap.horizontal.2xl
    gap-content: "{spacing.xs}"                 # 4px  → spacing.gap.vertical.xs
    gap-list: "{spacing.4xl}"                   # 24px → spacing.gap.vertical.4xl
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-medium}"
    titleColor: "{text.neutral.primary}"
    dateColor: "{text.neutral.secondary}"

  # ─── CARD ARTICLE — MINIMAL ───────────────────────────────────────────────
  card-article-minimal:
    gap-content: "{spacing.xs}"                 # 4px  → spacing.gap.vertical.xs
    gap-list: "{spacing.5xl}"                   # 32px → spacing.gap.vertical.5xl
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-medium}"
    titleColor: "{text.neutral.primary}"
    dateColor: "{text.neutral.secondary}"

  # ─── CARD EVENT ───────────────────────────────────────────────────────────
  card-event:
    borderRadius: "{rounded.lg}"                # 6px
    borderWidth: "{border.width.md}"            # 1.5px
    borderColor: "{border.neutral.soft}"        # #f5f7f9 → resolves former hardcode; same hex, now a real border role
    backgroundColor: "{surface.neutral.white}"
    thumbnailBorderRadiusTop: "{rounded.lg}"    # 6px
    thumbnailBorderRadiusBottom: 0px
    contentPaddingHorizontal: "{spacing.2xl}"   # 16px
    contentPaddingVertical: "{spacing.xl}"      # 12px
    gap-label-title: "{spacing.md}"             # 8px  → spacing.gap.vertical.md
    gap-rows: "{spacing.md}"                    # 8px  → spacing.gap.vertical.md
    gap-price: "{spacing.md}"                   # 8px  → spacing.gap.vertical.md
    gap-grid: "{spacing.5xl}"                   # 32px
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-regular}"
    location-typography: "{typography.body-3-regular}"
    narasumber-typography: "{typography.body-3-regular}"
    price-value-typography: "{typography.body-2-semibold}"   # Inter 16 Semi Bold / 26 — replaces stale primitive refs (font.weight.300, font.size.mobile.600)
    price-label-typography: "{typography.caption-regular}"   # Inter 12 Regular / 20 — replaces stale primitive refs (font.weight.100, font.size.mobile.400)
    hover-elevation: "{shadow.sm}"
    titleColor: "{text.neutral.primary}"
    dateColor: "{text.neutral.secondary}"
    locationColor: "{text.neutral.secondary}"
    narasumberColor: "{text.neutral.secondary}"
    priceLabelColor: "{text.neutral.tertiary}"
    priceValueColor: "{text.neutral.primary}"
---

## Overview

Hukumonline (HOL) is Indonesia's leading legal information platform. Its design language
reflects authority, clarity, and trust — values critical in the legal domain. The canvas
is clean white (`{colors.surface-neutral-white}`) with light neutral hairlines
(`{colors.border-neutral-default}` — `#a8b8c7`) doing separation work rather than heavy
shadows. Depth, when needed, is expressed through brand-tinted box shadows (brand navy at
low alpha).

The brand runs on two colors: a deep **HOL Navy** (`{colors.surface-brand-primary-base}` —
`#003366`) carrying every primary CTA, active indicators, link text, and navigation; and a
warm **HOL Gold** (`{colors.surface-brand-secondary-base}` — `#f8ca0f`) reserved for
secondary call-to-action moments and active tab indicators. This restraint keeps pages from
feeling cluttered — most surfaces are white with navy type, with gold appearing only at
deliberate moments.

Typography uses **Nunito Sans** for display, heading, title, label, and — as of v4 — button
labels, and **Inter** for body, captions, form chrome, and data. At body sizes (14–18px)
Inter maximises legibility for long-form legal text. Chips, tabs, and cards stay on Inter to
keep UI chrome quiet; buttons now carry Nunito Sans Bold so actions read as a distinct,
deliberate layer.

**Key Characteristics:**
- Two-color brand system: navy primary + gold secondary. Status colors (green, red, yellow,
  blue) are used for semantic meaning only — never as accent decoration. The purple and
  indigo accent ramps that now exist in the source are not yet consumed by any component.
- Shadow as brand tone: all elevation uses box shadows with brand navy alpha rather than
  neutral gray shadows, keeping depth warm rather than cold.
- Typography hierarchy is size-and-weight-driven, not decorative, and every style now has a
  Desktop and a Mobile mode.
- Card components (article + event) rely on layout, typography, and text color — no
  card-level background token (defaults to white canvas) and no card border except on
  card-event.
- Interactive components (button, chip, tab) use the full navy scale across states:
  lighter fills on hover, base on default/active, strong on pressed.

---

## Colors

All color roles live in `Colors - Semantic` and alias the primitive ramps in
`Colors - Primitive` (blue, yellow, neutral, red, green — 12 steps each except neutral at 8 —
plus purple and indigo). Components consume semantic roles only; never reference a
primitive directly.

The semantic set is organised by **role first, then intent**: `surface.*` (fills),
`background.*` (page/section backgrounds), `text.*`, `border.*`, `icon.*`, `shadow.*`
(navy alpha tints for elevation), and `surface.overlay.*` (alpha scrims).

### Brand & Accent

- **HOL Navy — base** (`{colors.surface-brand-primary-base}` — `#003366`): The primary brand
  color. Primary buttons, active chip fills, label-dark solid, badge-text-dark. Also
  `text.brand-primary.base` for navy labels and `border.brand.primary` for brand outlines.
- **HOL Navy — strong** (`#05213e`): Pressed state for primary button and chip.
- **HOL Navy — moderate / mild** (`#00458a` / `#125190`): New intermediate steps, no
  component consumer yet.
- **HOL Navy — muted** (`#0052a3`): Primary button hover. Also `text.brand-primary.muted`
  (author links, tab hover, tertiary button hover/pressed) and `border.state.interactive`
  (outline button, chip hover, label-dark outline).
- **HOL Navy — subtle** (`#2877c5`): Same hex as `border.state.active` (focused inputs) and
  the info family.
- **HOL Navy — soft** (`#89bff4`): Outline button pressed background.
- **HOL Navy — lighter** (`#e0ecf9`): Outline button and chip hover background; label-dark
  default background.
- **HOL Gold — base** (`{colors.surface-brand-secondary-base}` — `#f8ca0f`): Secondary
  button background and active tab indicator. One gold moment per page is the intended
  rhythm.
- **HOL Gold — subtle** (`#ffe168`): Secondary button hover.
- **HOL Gold — soft** (`#fff3c5`): New in v4, no consumer yet.
- **HOL Gold — strong**: ⚠ still not defined as a surface role. `text.brand-secondary.strong`
  (`#8d7101`) exists but is a text role and must not be used as a fill. See Known Gaps.

### Surface & Background

- **White** (`{colors.surface-neutral-white}` — `#ffffff`): Default canvas and card
  background.
- **Lightest** (`#f5f7f9`): Disabled input and outline-button backgrounds, label-light
  background.
- **Lighter** (`#cfd9e2`): Chip disabled, badge-icon-light, badge-text-light, label-light
  solid.
- **Soft** (`#a8b8c7`): Disabled primary/secondary button fill.
- `background.*` mirrors the soft status tints (`#ffeff0`, `#ebf6fc`, `#eefdf6`, `#fff9e3`)
  plus four neutrals, for section-level backgrounds rather than component fills.

### Text

- **Primary** (`{colors.text-neutral-primary}` — `#2b4156`): Default body text, card titles,
  input labels and values.
- **Secondary** (`#607a93`): Dates, locations, narasumber, helper text, disabled button labels.
- **Tertiary** (`#8398ab`): Placeholders, card-event price label, disabled tab label.
  Note: 2.98:1 on white — acceptable for placeholder only, never for meaningful content.
- **Quaternary** (`#a8b8c7`) / **Muted** (`#f5f7f9`): New in v4, no consumer yet.
- **Inverse** (`#ffffff`): Text on navy and solid status fills.
- **Brand primary** — base `#003366`, strong `#05213e`, muted `#0052a3`, soft `#89bff4`.
  The previous `subtle` step was removed in v4.
- **Status** — `danger.base/strong`, `success.base/strong`, `info.base/strong`,
  `warning.strong` (⚠ `#6f4e37`, see Known Gaps), and `brand-secondary.base/moderate/strong`.

### Border

v4 reorganised borders into four intent groups. Two values swapped between roles —
read this section before shipping.

- **`border.neutral.default`** (`#a8b8c7`): Input default/filled, chip default, label-light
  outline. **Δ v4: was `#cfd9e2`.** Contrast on white rises from 1.43:1 to 2.03:1.
- **`border.neutral.soft / moderate / strong`** (`#f5f7f9` / `#8398ab` / `#607a93`): soft is
  now the card-event border.
- **`border.state.active`** (`#2877c5`): Focused input.
- **`border.state.interactive`** (`#0052a3`): Outline button, chip hover, label-dark outline.
  Replaces the previous `border.interactive` / `border-brand` alias.
- **`border.state.disabled`** (`#cfd9e2`): Outline button disabled, input disabled.
  **Δ v4: was `#a8b8c7`.**
- **`border.status.*`**: danger `#dc381f`, danger-strong `#800000`, success `#00875a`,
  warning `#daa520`. ⚠ **There is no `info` step** — label-blue-outline is unresolved.
- **`border.brand.primary / primary-soft`** (`#003366` / `#e0ecf9`) and
  **`border.inverse.*`** (white at 100% / 30% / 0%): new, no consumer yet.

### Semantic (status)

- **Success** (`#00875a` / soft `#eefdf6` / text-strong `#006040`): Green label, success input.
- **Danger** (`#dc381f` / soft `#ffeff0` / text-strong `#800000`): Red label, failed input,
  badge-dot.
- **Warning** (`#daa520` / soft `#fff9e3` / text-strong `#6f4e37` ⚠): Yellow label.
- **Info** (`#2877c5` / soft `#ebf6fc` / text-strong `#00458a`): Blue label. **Δ v4: info.base
  moved from `#0177cc` to `#2877c5`** (now shares the blue.600 step with brand-subtle). The
  solid blue label now uses `surface.info.base` directly — white on `#2877c5` is 4.63:1 and
  passes AA, so the missing `surface.info.strong` is no longer needed.

### Overlay

`surface.overlay.*` provides alpha scrims: navy (`blue.1100` @ 30% / 40%) for modal
backdrops, white (@ 10–30%) for overlays on dark imagery, neutral-500 @ 20% for contrast
lifts, and info/danger tints. No component in this document consumes them yet; the modal and
drawer specs should when they are added.

---

## Typography

HOL uses two typefaces across the entire system.

**Nunito Sans** handles headings (1–4), titles (1–2), subtitle, the `label-*` styles, and
button labels. It is friendly and readable at large sizes without appearing either too
corporate or too casual — appropriate for a platform that is authoritative but not cold.

**Inter** handles body copy, captions, form chrome, and data text. Its open apertures make it
exceptionally legible at the 12–18px range where legal content is consumed.

Every style resolves through two modes — **Desktop** and **Mobile**. The frontmatter stores
the Desktop value as the reference; the Mobile value is noted per entry and listed below.
Implement as a responsive swap at the mobile breakpoint, not as a separate token name.

| Token | Family | Weight | Desktop size / LH / LS | Mobile size / LH / LS |
|---|---|---|---|---|
| `{typography.heading-1-extrabold}` | Nunito Sans | 800 Extra Bold | 50px / 60px / 0.7px | 32px / 44px / 0.5px |
| `{typography.heading-1-bold}` | Nunito Sans | 700 Bold | 50px / 60px / 0.7px | 32px / 44px / 0.5px |
| `{typography.heading-1-semibold}` | Nunito Sans | 600 Semi Bold | 50px / 60px / 0.7px | 32px / 44px / 0.5px |
| `{typography.heading-2-extrabold}` | Nunito Sans | 800 Extra Bold | 42px / 50px / 0.6px | 24px / 32px / 0.4px |
| `{typography.heading-2-bold}` | Nunito Sans | 700 Bold | 42px / 50px / 0.6px | 24px / 32px / 0.4px |
| `{typography.heading-2-semibold}` | Nunito Sans | 600 Semi Bold | 42px / 50px / 0.6px | 24px / 32px / 0.4px |
| `{typography.heading-3-extrabold}` | Nunito Sans | 800 Extra Bold | 35px / 46px / 0.15px | 22px / 30px / 0px |
| `{typography.heading-3-bold}` | Nunito Sans | 700 Bold | 35px / 46px / 0.15px | 22px / 30px / 0px |
| `{typography.heading-3-semibold}` | Nunito Sans | 600 Semi Bold | 35px / 46px / 0.15px | 22px / 30px / 0px |
| `{typography.heading-4-extrabold}` | Nunito Sans | 800 Extra Bold | 29px / 40px / 0px | 20px / 28px / 0px |
| `{typography.heading-4-bold}` | Nunito Sans | 700 Bold | 29px / 40px / 0px | 20px / 28px / 0px |
| `{typography.heading-4-semibold}` | Nunito Sans | 600 Semi Bold | 29px / 40px / 0px | 20px / 28px / 0px |
| `{typography.title-1-extrabold}` | Nunito Sans | 800 Extra Bold | 24px / 36px / 0px | 18px / 26px / 0px |
| `{typography.title-1-bold}` | Nunito Sans | 700 Bold | 24px / 36px / 0px | 18px / 26px / 0px |
| `{typography.title-2-extrabold}` | Nunito Sans | 800 Extra Bold | 20px / 30px / 0px | 16px / 26px / 0px |
| `{typography.title-2-bold}` | Nunito Sans | 700 Bold | 20px / 30px / 0px | 16px / 26px / 0px |
| `{typography.title-2-semibold}` | Nunito Sans | 600 Semi Bold | 20px / 30px / 0px | 16px / 26px / 0px |
| `{typography.subtitle-extrabold}` | Nunito Sans | 800 Extra Bold | 18px / 30px / 0px | 16px / 26px / 0px |
| `{typography.subtitle-bold}` | Nunito Sans | 700 Bold | 18px / 30px / 0px | 16px / 26px / 0px |
| `{typography.subtitle-semibold}` | Nunito Sans | 600 Semi Bold | 18px / 30px / 0px | 16px / 26px / 0px |
| `{typography.body-1-bold}` | Inter | 700 Bold | 18px / 28px / 0.13px | 16px / 26px / 0px |
| `{typography.body-1-semibold}` | Inter | 600 Semi Bold | 18px / 28px / 0.13px | 16px / 26px / 0px |
| `{typography.body-1-medium}` | Inter | 500 Medium | 18px / 28px / 0.13px | 16px / 26px / 0px |
| `{typography.body-1-regular}` | Inter | 400 Regular | 18px / 28px / 0.13px | 16px / 26px / 0px |
| `{typography.body-2-bold}` | Inter | 700 Bold | 16px / 26px / 0.25px | 14px / 24px / 0px |
| `{typography.body-2-semibold}` | Inter | 600 Semi Bold | 16px / 26px / 0px | 14px / 24px / 0px |
| `{typography.body-2-medium}` | Inter | 500 Medium | 16px / 26px / 0px | 14px / 24px / 0px |
| `{typography.body-2-regular}` | Inter | 400 Regular | 16px / 26px / 0px | 14px / 24px / 0px |
| `{typography.body-3-bold}` | Inter | 700 Bold | 14px / 22px / 0px | 12px / 20px / 0px |
| `{typography.body-3-semibold}` | Inter | 600 Semi Bold | 14px / 22px / 0px | 12px / 20px / 0px |
| `{typography.body-3-medium}` | Inter | 500 Medium | 14px / 22px / 0px | 12px / 20px / 0px |
| `{typography.body-3-regular}` | Inter | 400 Regular | 14px / 22px / 0px | 12px / 20px / 0px |
| `{typography.body-article-bold}` | Inter | 700 Bold | 18px / 32px / 0.13px | 18px / 32px / 0.13px |
| `{typography.body-article-regular}` | Inter | 400 Regular | 18px / 32px / 0.13px | 18px / 32px / 0.13px |
| `{typography.caption-medium}` | Inter | 500 Medium | 12px / 20px / 0px | 10px / 16px / 0px |
| `{typography.caption-bold}` | Inter | 700 Bold | 12px / 20px / 0px | 10px / 16px / 0px |
| `{typography.caption-semibold}` | Inter | 600 Semi Bold | 12px / 20px / 0px | 10px / 16px / 0px |
| `{typography.caption-regular}` | Inter | 400 Regular | 12px / 20px / 0px | 12px / 16px / 0px |
| `{typography.small-extrabold}` | Inter | 800 Extra Bold | 10px / 16px / 0.15px | 9px / 14px / 0.13px |
| `{typography.small-semibold}` | Inter | 600 Semi Bold | 10px / 16px / 0.15px | 9px / 14px / 0.13px |
| `{typography.extra-small-extrabold}` | Inter | 800 Extra Bold | 8px / 16px / 0.13px | 8px / 16px / 0.13px |
| `{typography.extra-small-semibold}` | Inter | 600 Semi Bold | 8px / 16px / 0.13px | 8px / 16px / 0.13px |
| `{typography.2x-small-extrabold}` | Inter | 800 Extra Bold | 6px / 16px / 0.13px | 6px / 16px / 0.13px |
| `{typography.2x-small-semibold}` | Inter | 600 Semi Bold | 6px / 16px / 0.13px | 6px / 16px / 0.13px |
| `{typography.label-extrabold}` | Nunito Sans | 800 Extra Bold | 14px / 22px / 0.13px | 12px / 20px / 0.13px |
| `{typography.label-bold}` | Nunito Sans | 700 Bold | 14px / 22px / 0.13px | 12px / 20px / 0.13px |
| `{typography.label-semibold}` | Nunito Sans | 600 Semi Bold | 14px / 22px / 0.13px | 12px / 20px / 0.13px |
| `{typography.button-label-lg}` | Nunito Sans | 700 Bold | 16px / 24px / 0.4px | 16px / 24px / 0.4px |
| `{typography.button-label-md}` | Nunito Sans | 700 Bold | 14px / 24px / 0.25px | 14px / 24px / 0.25px |
| `{typography.button-label-sm}` | Nunito Sans | 700 Bold | 12px / 24px / 0.15px | 12px / 24px / 0.15px |
### Principles

- **Body-1 through Body-3** carry card content, form inputs, and navigation labels — the
  typographic workhorse range. **Body-article** (18 / 32, identical on mobile) is the
  dedicated long-form reading style; use it for article and legal-text bodies rather than
  stretching body-1, whose mobile size drops to 16px.
- **Caption-medium** is used for input labels, helper text, and labels — keeping form chrome
  visually subordinate to input values.
- **Small / extra-small / 2x-small** now exist as real tokens (10 / 8 / 6px). The sub-scale
  sizes that badge-text and badge-dot previously hardcoded are now tokenized — they remain
  intentional and are only for count digits inside small circular containers. Never use
  extra-small or 2x-small for readable text.
- **Button labels** use the dedicated `button-label-*` styles (Nunito Sans Bold, 24px
  line-height across sizes). Do not substitute a body style.
- Within a weight family, desktop letter-spacing tightens toward 0 on mobile for headings and
  body-1; that is intentional optical compensation at smaller sizes.

### Note on Font Substitutes

Nunito Sans and Inter are both available on Google Fonts and are the canonical HOL typefaces.
If either is unavailable, system sans-serif is the fallback — never substitute a serif face.

---

## Layout

HOL spacing is a numeric scale (2 / 4 / 6 / 8 / 10 / 12 / 16 / 20 / 24 / 32 / 40 / 48 / 56 /
64 / 123 px) named `2xs` → `9xl` + `max`. v4 renamed every step so the names now match the
source exactly — `{spacing.X}` here equals `spacing.padding.X`, `spacing.gap.horizontal.X`,
and `spacing.gap.vertical.X` in Figma. Use the padding variant for padding properties and the
matching gap variant for auto-layout gaps; their values are identical.

| Token | Value | Common Use |
|---|---|---|
| `{spacing.2xs}` | 2px | Label & chip-sm vertical padding, badge-dot-xl vertical padding |
| `{spacing.xs}` | 4px | Chip md/lg vertical padding; card content gaps (title → meta) |
| `{spacing.sm}` | 6px | Badge-dot-xl horizontal padding |
| `{spacing.md}` | 8px | Input padding, label & chip sm/md horizontal, button-sm vertical, card-event row gaps |
| `{spacing.lg}` | 10px | — (no consumer yet) |
| `{spacing.xl}` | 12px | Button-md vertical, chip-lg horizontal, card-event vertical padding |
| `{spacing.2xl}` | 16px | Button-sm horizontal, button-lg vertical, input left padding, card-event horizontal, thumbnail → content gap |
| `{spacing.3xl}` | 20px | — (no consumer yet) |
| `{spacing.4xl}` | 24px | Button md/lg horizontal, side-card list gap |
| `{spacing.5xl}` | 32px | Card list and grid gaps |
| `{spacing.6xl}` – `{spacing.9xl}` | 40–64px | Section spacing (no component consumer yet) |
| `{spacing.max}` | 123px | ⚠ purpose undocumented in source |

**Migration note for code:** the step *names* moved, not the component values. Example: the
old `spacing.sm` meant 16px; in v4 `spacing.sm` is 6px and 16px is `spacing.2xl`. Any code
that consumed the old doc-level aliases must be remapped by value, not by name.

Card gaps were previously prose-only; they are now tokenized in each card component
(`gap-*` properties).

### Radius

| Token | Value | Consumer |
|---|---|---|
| `{rounded.2xs}` / `{rounded.xs}` | 2 / 3px | — |
| `{rounded.sm}` | 4px | Label square, featured-card thumbnail |
| `{rounded.md}` | 5px | Inputs, chip square, grid/side thumbnails |
| `{rounded.lg}` | 6px | Buttons, card-event |
| `{rounded.xl}` / `{rounded.2xl}` / `{rounded.3xl}` / `{rounded.4xl}` | 8 / 10 / 12 / 16px | — |
| `{rounded.5xl}` | 24px | Chip round |
| `{rounded.6xl}` | 30px | — |
| `{rounded.7xl}` | 100px | Label round, tab indicator, badge-dot-xl |
| `{rounded.full}` | 999px | Badges |

---

## Elevation

HOL uses a single family of box shadows, all tinted with brand navy alpha rather than neutral
gray. Values are unchanged in v4. There are five tiers:

| Token | Value | Usage |
|---|---|---|
| `{shadow.xs}` | 0 1 4 1 / navy 7% | Subtle card lift, tooltip |
| `{shadow.sm}` | 1 2 12 2 / navy 9% | Card-event hover, dropdown |
| `{shadow.md}` | 1 6 20 4 / navy 12% | Modal, active card |
| `{shadow.lg}` | 1 2 40 4 / navy 16% | Navigation drawer, sticky header |
| `{shadow.xl}` | 2 2 56 9 / navy 16% | Full-page overlay, dialog |

Card article variants use no shadow — separation is achieved through spacing alone.
Card-event uses `{shadow.sm}` on hover. For modal/drawer backdrops pair elevation with
`surface.overlay.default` (navy @ 40%).

---

## Components

Fifteen components below are specified from the HOL Design System 2.0 Figma library
(file `1gSTFbZHnohv4iJr9k51et`). Tab and the card components are carried over from v4
unchanged. Where Figma binds a radius name that differs from `ds-v4.json`, the value is
written against the JSON name and the Figma name is noted (see Cross-component Issues).

### Actions

**`button`** — Five styles: **Primary** (navy fill), **Secondary** (gold fill, navy label),
**Outline** (1px `{border.state.interactive}`), **Text Icon** (label only, formerly
"tertiary"), and **Light** (white outline and overlays, for navy or image backgrounds).
Three sizes — sm 40px, md 48px, lg 56px — all with `{rounded.lg}` and
`button-label-*` typography (Nunito Sans Bold, 24px line-height). States: default, hover,
pressed, disabled, and loading (Spinner 20px, neutral fill). Each size has an icon-only
square variant. Primary hover deepens to `{surface.brand-primary.moderate}`; pressed goes
to `{surface.brand-primary.strong}`. Secondary pressed uses `{surface.warning.base}`
(navy label 5.63:1). Labels max 25 characters. Fixed-width and full-width layouts are both
valid; in groups, primary sits on the right of its secondary action.

**`back-to-top`** — Floating pill (`{rounded.6xl}`, 30px) with white fill, 1px light border
and a soft navy shadow. **With Text** (40px, `button-label-md`, bottom-center) for inner
scroll — article, document, PDF. **Icon** (48px, bottom-right) for regular scroll —
landing page, catalogue. Appears only when the page is at least 4× above-the-fold
(3072px desktop, 3200px mobile). It has the lowest stacking priority among floating
elements and shifts to avoid them (e.g. the WhatsApp button). Click smooth-scrolls to top.

### Forms

**`input`** — Two types share one spec. **Field** (48px, leading search icon, trailing
caret/status icon) and **Text Area** (min 82px, 8px padding, trailing copy icon). Label
and helper use `caption-medium`, value uses `body-3-medium`, all stacked with a 4px gap.
Radius `{rounded.md}`. States: default and filled (1px border), active (1.5px
`{border.state.active}`), failed (1.5px danger border, warning icon, danger helper),
success (Field only), disabled (`{surface.neutral.lightest}` fill, tertiary text).

**`checkbox`** — 16px box, `{rounded.sm}`, 1px border, label `body-3-medium` 8px to the
right. Checked fills `{surface.brand-primary.subtle}` with a white check; an indeterminate
dash exists on the inner Check component. The whole row (box + label) is the hit area.
Keep labels short and stack options vertically rather than in a multi-column grid.

**`radio`** — Same anatomy and colours as Checkbox with a circular control
(`{rounded.full}`). One option per group; selecting another deselects the previous one,
and re-clicking the selected option does nothing. Labels left-aligned. Keyboard: arrow keys
move selection within the group.

**`toggle`** — 32×20px pill switch with a white handle and `body-3-medium` label. Track:
on `{surface.brand-primary.subtle}`, off `{surface.neutral.soft}`, disabled on
`{surface.brand-primary.soft}`, disabled off `{surface.neutral.lighter}`. Takes effect
immediately — no save step. Use for on/off states, not for choosing between two equal
options. Figma restricts the hit area to the switch only; see Cross-component Issues.

### Selection and tagging

**`chip`** — Interactive filter. Three sizes (26 / 30 / 36px) × Rounded (`{rounded.5xl}`,
24px) or Square (radius scales 3 / 4 / 5px by size). Optional 16px icon on the left
(context) or right (action). States: default, hover (navy lighter fill + interactive
border), active (navy fill), pressed (navy strong), disabled (lighter fill, tertiary
label). Labels max 25 characters; group chips by category.

**`label`** — Non-interactive tag, 24px tall, `caption-medium`. Six colours × Default
(soft fill), Outline (soft fill + 1px status border) and Solid (full fill, white text) ×
Square (`{rounded.sm}`) or Round (`{rounded.7xl}`). Width hugs content; 10–25 characters.
Yellow text now uses `{text.brand-secondary.strong}`; blue uses the brand-primary muted
family. Use colour to encode status consistently (blue info, red error, green success,
yellow warning).

**`badges`** — One set covering five types on a 16 / 20 / 32 / 48px scale: **Image**
(avatar), **Text** (≤2 characters), **Icon** (filled circle), **Icon No Fill**, and
**dot** (notification). Light style uses `{surface.neutral.lighter}`, dark style uses
`{surface.brand-primary.base}`. Notification dots are `{surface.danger.base}`: S 6px and
M 10px dots without a count, L 16px with ≤2 characters, XL 32×20px pill with ≤3 ("99+").
Place notification dots on the top-right of their host.

### Feedback

**`alert`** — Status message in five states (info, success, warning, failed, neutral),
each with soft fill, status border, status icon and strong title. **Medium** (320px,
stacked) for mobile, **Large** (container width, single row) for desktop. Title
`body-1-bold`, description `body-3-medium` secondary. Optional close icon and two small
actions (text-icon + primary). Fixed top-center, auto-dismiss after 3–5 s unless
persistent; title plus description max 100 characters.

**`tooltip`** — Short contextual text (`caption-medium`, ≤250 characters) in Default
(`{surface.brand-primary.moderate}`), Dark (`{surface.neutral.strong}`, for light
backgrounds) or Light (`{surface.neutral.lighter}`, for dark backgrounds). 5px radius,
8×12px padding, pointer on any side with three alignments. 4px offset from the target,
16px from the viewport edge, auto-flips to available space, fades in with a short slide.
Show on keyboard focus as well as hover; dismiss with Esc; never cover the target.

**`coachmark`** — Guided onboarding card, 370px desktop / 320px mobile, `{rounded.lg}`,
16px padding. Title `body-3-bold`, description `caption-medium`, optional step counter,
"Lewati" or X to dismiss, and Previous (outline) / Next (secondary + caret) actions.
Default (`{surface.brand-primary.moderate}`, gold title), Dark
(`{surface.neutral.strong}`, gold title) and Light (`{surface.neutral.lightest}`, muted
navy title). Anchors to its target, re-positions or flips its pointer when space is
short, and shifts to avoid nearby elements. Use for discrete steps, not long copy; use
Tooltip for single-line hints.

**`loader`** — Animated HOL logo for short, indeterminate waits on partial UI updates
(section loading, data refresh, quick results). Sizes 16 / 24 / 40px. Do not use it for
long or measurable processes — use a progress bar. Inline actions use the Button Spinner
instead. Mark the loading region with `role="status"` / `aria-busy` and honour
`prefers-reduced-motion`.

### Navigation

**`breadcrumb`** — 24px trail in `body-3-medium` with CaretRight separators.
**Dashboard** type starts with a home icon; **Media** type starts with "Beranda". Default
(navy links on light) and Dark (white links on navy). Up to four visible levels; beyond
that the middle levels collapse into a DotsThree overflow menu. Each level max 20
characters on desktop and 10 on mobile. The last item is the current page: secondary
colour, not a link, `aria-current="page"`.

**`pagination`** — 32px square items with a 16px gap, `{rounded.sm}`, `body-3-bold`
numbers. Current page is navy-filled; other numbers and arrows use a 1px light border.
Five layouts — Default (≤5 pages), Left, Centered, Right (by current-page position), and
arrows-only. Overflowing ranges collapse into an ellipsis. Place below the paginated
content next to the result count.

**`tab`** — Height 40px. Horizontal (page sections, topic navigation) and Vertical (sidebar,
modal navigation). Typography `{typography.body-3-medium}`. Active indicator: 4px bar,
`{rounded.7xl}`, `{surface.brand-secondary.base}` (HOL Gold), bottom edge for horizontal,
right edge for vertical. States: default, hover (`{text.brand-primary.muted}`), active
(primary label + gold indicator), disabled (tertiary label). Not re-specified from Figma in
v4.1.

### Content cards (carried over from v4)

**`card-article-featured`** — Horizontal: thumbnail left (256 × 160px, `{rounded.sm}`),
content right. Gaps 16 / 4 / 16 / 32px. Title `{typography.body-1-semibold}`, description
`{typography.body-2-regular}`, date and author `{typography.body-3-medium}`; author in
`{text.brand-primary.muted}`. Title underlines on hover.

**`card-article-grid`** — Portrait thumbnail on top (160 × 256px, `{rounded.md}`), 8px to
content, 32px grid gap. Title `{typography.body-2-semibold}`.

**`card-article-side`** — Compact horizontal (176 × 117px thumbnail), 16px to content, 24px
list gap.

**`card-article-minimal`** — Text only; on hover a button-md primary "Daftar" appears.

**`card-event`** — Vertical card, `{rounded.lg}`, 1.5px `{border.neutral.soft}` border,
16 × 12px content padding, 8px row gaps, price block in `caption-regular` /
`body-2-semibold`, `{shadow.sm}` and a "Daftar" button on hover.

---

## Cross-component Issues (v4.1)

These patterns recur across the Figma components. Fixing them once — in tokens or in the
library — is cheaper than patching each component.

| # | Pattern | Affected | Recommended fix |
|---|---|---|---|
| X1 | Figma radius names are one step ahead of `ds-v4.json` (Figma `6xl`=24 / `7xl`=30 / `8xl`=100 vs JSON `5xl` / `6xl` / `7xl`). This document uses the JSON names. | Chip, Label, Back to Top, Badges | Re-export tokens from the library; then rename the four references here. |
| X2 | `border.state.disabled` (#cfd9e2, 1.43:1) used as the *enabled* resting border | Input, Chip, Label Light, Back to Top, Pagination | Add a dedicated role (e.g. `border.neutral.subtle`) and decide its contrast target explicitly. |
| X3 | Form-control boundary `#a8b8c7` is 2.03:1 (WCAG 1.4.11 needs 3:1) | Checkbox, Radio, Toggle (off track) | One control-border role at `#8398ab` or darker. |
| X4 | Status roles (`info`, `warning`) used inside brand components | Button (outline hover, text-icon hover/pressed, secondary pressed), Label, Breadcrumb, Coachmark | Alias brand roles (e.g. `surface.brand-secondary.strong`) so status colour changes don't leak. |
| X5 | Hybrid elevation — geometry and colour from different tiers | Back to Top, Tooltip (md + light), Coachmark (lg + medium) | Add an `elevation.floating` token or use whole tiers. |
| X6 | Flattened vectors — colour not bound to variables | Checkbox check, Radio dot, Toggle switch, Badge dots, Tooltip/Coachmark pointer, Pagination ellipsis | Rebuild as shapes with variable fills. |
| X7 | Buttons rebuilt inside composites instead of `New Button` instances | Alert, Coachmark | Swap to instances so Button updates propagate. |
| X8 | Variant naming defects | Input (duplicate Success), Coachmark (trailing spaces), Toggle (Status5–8), Breadcrumb ("Presse", "Breadcumb"), Pagination (Property 2/3) | Rename; required before Code Connect. |
| X9 | No focus-visible state | All interactive components | Add a shared focus ring token and state. |
| X10 | Device property duplicates typography modes | Checkbox, Radio, Toggle | Replace with variable modes; halves variant count. |
| X11 | Fixed size ≠ padding + content | Button icon-only sm/lg, Back to Top icon, Chip sm, Label | Align padding with fixed dimensions. |
| X12 | Documentation copy pasted from another page or stale spec text ("Info-300", "Info-500") | Input, Radio, Toggle, Checkbox, Chip, Tooltip, Label | Refresh doc frames from bindings. |

---

## Responsive Behavior

Breakpoint definitions for HOL are not yet formally extracted from a specification source.
The ranges below are provisional. The typography Desktop/Mobile modes should switch at the
Mobile boundary.

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 768px | Mobile typography mode; single-column layout; card-article-featured stacks vertically; tab bar scrolls horizontally |
| Tablet | 768–1024px | Two-column card grids; navigation condenses |
| Desktop | 1024–1440px | Desktop typography mode; multi-column layouts; card grids at 3-up or 4-up |
| Wide | > 1440px | Content capped; gutters absorb excess width |

### Touch Targets

- Buttons: button-md (48px) and button-lg (56px) meet the 44 × 44px target. button-sm (40px)
  falls slightly below — avoid it as a primary mobile action.
- Input fields: 48px fixed height meets touch target requirements.
- Chips: SM (26px) falls below the 44px threshold — use MD or LG in mobile contexts, or extend
  the hit area beyond the visual bounds.
- Tabs: 40px — acceptable at full-width tab rows; add vertical padding on mobile if tabs are
  narrow.
- Checkbox, Radio (24px rows) and Toggle (32×20px switch): extend the hit area to at least
  44px on mobile; Checkbox and Radio already include the label.
- Pagination items (32px) and Breadcrumb links (24px): keep ≥8px spacing and extend hit
  areas on mobile.

---

## Token Update Log (v4.1)

Source: HOL Design System 2.0 Figma library, 15 component pages, read on 2026-10-12.
Tokens unchanged — still `ds-v4.json` (see X1 for the radius naming offset).

### Components added (10)

Checkbox, Radio, Toggle, Alert, Tooltip, Coachmark, Loader, Back to Top, Breadcrumb,
Pagination.

### Components re-specified from Figma (5) — visual changes vs v4 (Δ)

| Component | Change | v4 → v4.1 |
|---|---|---|
| Button | Primary hover | `brand-primary.muted` #0052a3 → `brand-primary.moderate` #00458a |
| Button | Outline border width | 1.5px → 1px |
| Button | Outline hover fill | `brand-primary.lighter` → `info.soft` |
| Button | Outline disabled border | `state.disabled` → `neutral.default` |
| Button | Tertiary renamed Text Icon; hover/pressed label | `brand-primary.muted` → `info.base` |
| Button | Secondary pressed | ⚠ undefined → `surface.warning.base` |
| Button | New: Light style, Loading state, icon-only variants | — |
| Input | Resting border (default/filled) | `neutral.default` 2px → `state.disabled` 1px |
| Input | Active / failed / success border | 2px → 1.5px |
| Input | Text Area padding | 16px left → 8px all sides |
| Chip | Resting border | `neutral.default` 1.5px → `state.disabled` 1px |
| Chip | Square radius | 5px all sizes → 3 / 4 / 5px by size |
| Chip | Disabled | interactive border, primary label → `neutral.default` border, tertiary label |
| Label | Vertical padding | 2px → 4px |
| Label | Dark default/outline fill | `brand-primary.lighter` → `info.soft` |
| Label | Yellow text | `warning.strong` #6f4e37 → `brand-secondary.strong` #8d7101 |
| Label | Blue text / solid fill | `info.strong` / `info.base` → `brand-primary.muted` |
| Label | Blue outline border | ⚠ undefined → `border.state.active` |
| Badges | Merged badge-icon / badge-text / badge-dot into one set; added Icon No Fill | — |
| Badges | Dot XL | hug pill, 100px radius → fixed 32×20px, 30px radius |

### Resolved by v4.1

- `surface.brand-secondary.strong` no longer referenced (Button secondary pressed uses
  `surface.warning.base`; see X4).
- `border.status.info` no longer referenced (Label blue outline uses `border.state.active`).
- Label yellow text moved off the brown `#6f4e37` (Alert warning title still uses it).
- Chip disabled no longer shows an interactive border.
- Badge sub-scale typography confirmed against Figma (2x-small / extra-small / small).

### New open items

See Cross-component Issues X1–X12, plus:
- Label yellow solid still fails contrast (white on #daa520, 2.24:1); yellow default text
  #8d7101 on #fff9e3 is 4.43:1.
- Alert: description #607a93 on soft fills is 4.07:1; close icon 2.71–2.83:1; warning icon
  2.12:1.
- Breadcrumb Dark: separator 2.82:1 and pressed level 2.72:1 on navy; Media type does not
  distinguish the current page.
- Pagination: missing disabled arrows at first/last page and number hover/pressed; pressed
  is lighter than hover (inverse of Button).
- Toggle: hit area is the switch only (32×20px) — consider including the label.
- Loader: sizes exist only in docs; asset is raster.
- Badges: dark Text XL is 40px; Icon No Fill uses its own 12/16/24/40 scale.

---

## Token Update Log (v4)

Source: `ds-v4.json` (Tokens Brücke, DTCG 2025.10, 11 collections, exported 2026-10-08).

### Visual changes introduced by v4 (Δ)

These change what users see. Confirm each with product/brand before shipping.

| # | Change | Before → After | Affected components |
|---|---|---|---|
| 1 | Button label typography moved to dedicated `button-label-*` tokens | Inter 14 Medium / 16 SB / 18 SB → Nunito Sans Bold 12 / 14 / 16, LH 24, LS 0.15 / 0.25 / 0.4px | All buttons (heights now 40 / 48 / 56px) |
| 2 | `border.neutral.default` value | `#cfd9e2` → `#a8b8c7` | Input & textarea default/filled, chip default, label-light outline |
| 3 | `border.state.disabled` value | `#a8b8c7` → `#cfd9e2` | Button-outline disabled |
| 4 | Info palette base | `#0177cc` → `#2877c5` | Label-blue (all) |
| 5 | Label-blue-solid fill | `#00458a` (undefined token) → `surface.info.base` `#2877c5` | Label-blue-solid |
| 6 | `text.brand-primary.subtle` removed | `#2877c5` → `text.brand-primary.muted` `#0052a3` | Button-tertiary hover/pressed |
| 7 | Letter-spacing adjustments | body-1 0 → 0.13px; small 0.1 → 0.15px; heading-1 0.8 → 0.7px; heading-3 0.2 → 0.15px | Card-article-featured title, badge-dot-xl, badge-text-lg |
| 8 | Badge sub-scale text tokenized | LS 0.2 → 0.13px (sm/md) | Badge-text sm/md, badge-dot-lg |
| 9 | Title-2-bold & subtitle-bold weight now matches name | 800 → 700 (800 remains as `-extrabold`) | No component consumer |

### Renames / remaps (no visual change)

- **Spacing**: doc aliases renamed to match source step names. 2→`2xs`, 4→`xs`, 8→`md`,
  12→`xl`, 16→`2xl`, 24→`4xl`, 32→`5xl`, 48→`7xl`, 64→`9xl`. New steps 6 / 10 / 20 / 40 / 56 /
  123px. New `spacing.gap.horizontal.*` and `spacing.gap.vertical.*` collections mirror padding.
- **Radius**: 24px `4xl`→`5xl`, 100px `6xl`→`7xl`, 30px `5xl`→`6xl`, 16px `3xl`→`4xl`, 12px
  `2xl`→`3xl`. New 3px (`xs`) and 10px (`2xl`); 2px moved `xs`→`2xs`.
- **Color role paths**: `text.primary/secondary/tertiary/inverse` → `text.neutral.*`;
  `icon.inverse` → `icon.neutral.inverse`; `icon.danger` / `icon.success` → `.base`;
  `text.info` → `text.info.strong`; `text.warning` → `text.warning.strong`;
  `border.interactive/active/disabled` → `border.state.*`; `border.danger/success/warning` →
  `border.status.*`; `border.default` → `border.neutral.default`.
- **Line-height primitives** were renumbered (e.g. 60px is now `desktop.1400`, was `1300`).
  Semantic typography absorbs this; only code that referenced primitives directly is affected.
- **Elevation and border width**: values unchanged; `border.width.xl` (3px) added.

### Resolved by this update

- 2px spacing now exists (`spacing.2xs`) — label and chip-sm vertical padding are fully
  tokenized. ✅
- Mobile typography is surfaced: every style carries Desktop and Mobile values. ✅
- `surface.info.strong` dependency removed — label-blue-solid uses `surface.info.base`, which
  passes AA with white text. ✅
- Card-event border is a real border role (`border.neutral.soft`) instead of a surface token. ✅
- Badge-text sm/md/lg and badge-dot-lg no longer hardcode 6 / 8 / 10px — dedicated
  2x-small / extra-small / small styles exist. ✅
- Badge-dot-xl 6px horizontal padding is tokenized (`spacing.sm`). ✅
- Card-event price typography no longer references stale primitives from the old 5-step
  weight scale (`font.weight.300`, `font.weight.100`). ✅
- Card gaps are tokenized via `spacing.gap.*` instead of prose-only. ✅
- Buttons have dedicated label tokens; all sizes now share a 24px line-height. ✅

### Still open

**Blocking — undefined references in components**
- `surface.brand-secondary.strong` (button-secondary-pressed) is still not defined. Add it in
  Figma Variables, e.g. → `yellow.500` (`#daa520`) for a visible-but-on-brand press state.
- `border.status.info` (label-blue-outline) is not defined. Add → `blue.600` (`#2877c5`).

**Accessibility**
- Label-yellow-solid: white on `#daa520` is 2.24:1, failing WCAG 1.4.3 AA. Recommended
  fix: switch the text to `text.brand-primary.base` — navy on `#daa520` is 5.63:1 and mirrors
  the navy-on-gold pattern already used by button-secondary. Not applied here because it
  changes the label's visual language; needs a brand decision.
- `border.neutral.default` (`#a8b8c7`) is 2.03:1 on white — better than before (1.43:1) but
  still under the 3:1 non-text contrast threshold (WCAG 1.4.11) for input boundaries.
  `border.neutral.moderate` (`#8398ab`) lands at 2.98:1 — just short; `border.neutral.strong`
  (`#607a93`, 4.47:1) is the nearest compliant role.
- `text.neutral.tertiary` (`#8398ab`, 2.98:1) must stay limited to placeholders.

**Source data quality**
- `text.warning.strong` still resolves to `#6f4e37` (`yellow.800`), a brown outside the yellow
  hue family. Renumbered across two updates, never fixed.
- Indigo primitive ramp breaks hue at the light end: `indigo.100` (`#1cb1d1`) and `indigo.200`
  (`#218eb9`) are cyan (~191–197°) while the rest sits at ~230–255°. `surface.accent-indigo.lighter`
  and `.soft` inherit this. The purple ramp is also uneven (`purple.400` `#b314e4` is magenta;
  `purple.1200` `#080d26` is near-navy). Audit both before any component consumes accents.
- `caption.reguler` is misspelled in the source (normalised to `caption-regular` here). Its
  mobile size is 12px while the other caption weights drop to 10px — confirm intent.
- The `[unuse]` group (5 tokens) is still exported in `Colors - Semantic`. Delete it in Figma
  so it can't be picked up by code generation.
- `spacing.max` / `spacing.scale-123` (123px) has no documented purpose.
- Primitive keys carry different values per platform (`font.size.mobile.500` = 14px vs
  `font.size.desktop.500` = 18px). Consume semantic typography only; never map primitives by
  key across modes.

**Component-level**
- Tab typography (`body-3-medium`, Inter) no longer matches button-md label (Nunito Sans Bold
  14). Decide whether tabs should move to `label-semibold` / `label-bold` for parity, or stay
  on Inter as quieter navigation chrome.
- Chip-disabled uses `border.state.interactive`, which makes the disabled chip read as
  enabled. Likely should be `border.state.disabled`.
- Badge-image and badge-dot dark borders use `surface.neutral.lighter` as a border color.
  No border role exists at `#cfd9e2` other than `border.state.disabled`; consider a dedicated
  separator role.
- No sizing tokens exist (input 48px, chip 26 / 30 / 36px, tab 40px, badge and icon sizes are
  hardcoded).
- `border.width.xl`, radius `2xs` / `xs` / `xl` / `2xl` / `3xl` / `4xl` / `6xl`, spacing `lg` /
  `3xl` / `6xl`+, accent ramps, overlays, `body-article`, `label-*`, and the extra weight
  variants have no consuming component yet. Per demand-driven tokenization, leave them
  unconsumed until a real component needs them.

**Carried over**
- Breakpoints and responsive rules are not formally specified — values above are provisional.
- Animation and transition timings (button press, chip selection, tab switch) are not
  documented.
- Dark mode is not a documented variant. HOL renders a single light canvas mode.
- Card-article components have no explicit background or border token — they inherit the
  white canvas.
- Hover interaction behaviors (underline on card titles, "Daftar" button appearance) are
  documented in prose only — no interaction tokens exist.
- Narasumber badge stacking logic is contextual and not defined by a token.
- Card-event thumbnail width fills the card; exact thumbnail height is pending decision.
- Form error and success illustrations are out of scope.
- Sub-components inside card-event (Label, Badge-image, Button primary-MD) rely on their own
  component tokens; cross-component composition rules are prose only.
