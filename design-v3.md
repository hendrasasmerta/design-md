---
version: alpha
tokenSource: new-tokens.json (updated primitive + semantic export — supersedes the
  export this document was originally generated from)
name: Hukumonline (HOL) Design System
description: A legal-information platform that pairs an authoritative navy brand
  with a warm golden secondary accent. Typography stays grounded in Inter for
  body reading — long-form legal text demands high legibility at moderate sizes —
  while Nunito Sans carries display and heading moments with confident weight.
  Surfaces are predominantly white with a near-invisible neutral border; depth
  is expressed through subtle brand-tinted shadows rather than heavy drop
  shadows. Every primary CTA runs in HOL navy, secondary moments in gold, and
  status signals use conventional semantic colors (green success, red danger,
  yellow warning, blue info).

colors:
  # NOTE ON THE TOKEN UPDATE: the underlying primitive collections were
  # restructured — "brand" was merged into a single 7-step "blue" ramp
  # together with the old separate "info" blue, "secondary" was absorbed
  # into an 8-step "yellow" scale, and "ocean" was renamed "indigo". The
  # resolved hex values aliased below are unchanged; only the source
  # primitive names changed. See "Known Gaps" for what is still unresolved.
  # Brand
  brand-primary-base: "#003366"
  brand-primary-muted: "#0052a3"
  brand-primary-subtle: "#2877c5"
  brand-primary-soft: "#89bff4"
  brand-primary-lighter: "#e0ecf9"
  brand-secondary-base: "#f8ca0f"
  brand-secondary-subtle: "#ffe168"
  brand-secondary-strong: "#8d7101"
  # Neutral
  neutral-white: "#ffffff"
  neutral-lightest: "#f5f7f9"
  neutral-lighter: "#cfd9e2"
  neutral-soft: "#a8b8c7"
  neutral-subtle: "#8398ab"
  neutral-base: "#2b4156"
  neutral-strong: "#162533"
  # Semantic
  success-base: "#00875a"
  success-soft: "#eefdf6"
  success-strong: "#006040"
  danger-base: "#dc381f"
  danger-soft: "#ffeff0"
  danger-strong: "#800000"
  warning-base: "#daa520"
  warning-soft: "#fff9e3"
  info-base: "#0177cc"
  info-soft: "#ebf6fc"
  info-strong: "#00458a"
  # Text roles
  text-primary: "#2b4156"
  text-secondary: "#607a93"
  text-tertiary: "#8398ab"
  text-inverse: "#ffffff"
  text-brand-primary: "#003366"
  text-brand-primary-muted: "#0052a3"
  # Border roles
  border-default: "#cfd9e2"
  border-active: "#2877c5"
  border-brand: "#0052a3"
  border-danger: "#dc381f"
  border-success: "#00875a"
  border-warning: "#daa520"
  border-info: "#0177cc"
  border-disabled: "#a8b8c7"

typography:
  # --- Display / Heading (Nunito Sans) ---
  # NOTE: fontWeight tokens are now font-family-specific (Typo - Primitive
  # separates "nunito sans.*" and "inter.*" weight ramps). Values below are
  # desktop sizes; a parallel mobile ramp now exists in the source
  # (Typo – Semantic) but is not yet surfaced in this document — see Known Gaps.
  heading-1-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1100}"           # 50px
    fontWeight: "{font.weight.nunito sans.800}"    # Extra Bold
    lineHeight: "{line-height.desktop.1300}"       # 60px
    letterSpacing: "{letter-spacing.80}"           # 0.8px
  heading-2-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.1000}"           # 42px
    fontWeight: "{font.weight.nunito sans.700}"    # Bold
    lineHeight: "{line-height.desktop.1200}"       # 50px
    letterSpacing: "{letter-spacing.60}"           # 0.6px
  heading-3-semibold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.900}"            # 35px
    fontWeight: "{font.weight.nunito sans.600}"    # Semi Bold
    lineHeight: "{line-height.desktop.1100}"       # 46px
    letterSpacing: "{letter-spacing.20}"           # 0.2px
  heading-4-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.800}"            # 29px
    fontWeight: "{font.weight.nunito sans.700}"    # Bold
    lineHeight: "{line-height.desktop.1000}"       # 40px
    letterSpacing: "{letter-spacing.0}"            # 0px
  title-1-extrabold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.700}"            # 24px
    fontWeight: "{font.weight.nunito sans.800}"    # Extra Bold
    lineHeight: "{line-height.desktop.900}"        # 36px
    letterSpacing: "{letter-spacing.0}"
  title-2-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.600}"            # 20px
    fontWeight: "{font.weight.nunito sans.800}"    # Extra Bold (alias bold in this scale)
    lineHeight: "{line-height.desktop.700}"        # 30px
    letterSpacing: "{letter-spacing.0}"
  subtitle-bold:
    fontFamily: "'Nunito Sans', sans-serif"
    fontSize: "{font.size.desktop.500}"            # 18px
    fontWeight: "{font.weight.nunito sans.800}"    # Extra Bold
    lineHeight: "{line-height.desktop.700}"        # 30px
    letterSpacing: "{letter-spacing.0}"
  # --- Body / UI (Inter) ---
  body-1-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"        # 18px
    fontWeight: "{font.weight.inter.600}"      # Semi Bold
    lineHeight: "{line-height.desktop.600}"    # 28px
    letterSpacing: "{letter-spacing.0}"
  body-1-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.500}"        # 18px
    fontWeight: "{font.weight.inter.400}"      # Regular
    lineHeight: "{line-height.desktop.600}"    # 28px
    letterSpacing: "{letter-spacing.0}"
  body-2-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.400}"        # 16px
    fontWeight: "{font.weight.inter.600}"      # Semi Bold
    lineHeight: "{line-height.desktop.500}"    # 26px
    letterSpacing: "{letter-spacing.0}"
  body-2-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.400}"        # 16px
    fontWeight: "{font.weight.inter.400}"      # Regular
    lineHeight: "{line-height.desktop.500}"    # 26px
    letterSpacing: "{letter-spacing.0}"
  body-3-medium:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.300}"        # 14px
    fontWeight: "{font.weight.inter.500}"      # Medium
    lineHeight: "{line-height.desktop.400}"    # 22px
    letterSpacing: "{letter-spacing.0}"
  body-3-regular:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.300}"        # 14px
    fontWeight: "{font.weight.inter.400}"      # Regular
    lineHeight: "{line-height.desktop.400}"    # 22px
    letterSpacing: "{letter-spacing.0}"
  caption-medium:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.200}"        # 12px
    fontWeight: "{font.weight.inter.500}"      # Medium
    lineHeight: "{line-height.desktop.300}"    # 20px
    letterSpacing: "{letter-spacing.0}"
  small-semibold:
    fontFamily: "Inter, sans-serif"
    fontSize: "{font.size.desktop.100}"        # 10px
    fontWeight: "{font.weight.inter.600}"      # Semi Bold
    lineHeight: "{line-height.desktop.100}"    # 16px
    letterSpacing: "{letter-spacing.10}"       # 0.1px

# Border-radius primitive scale expanded from 7 to 11 steps. Values already in
# use (sm/md/lg/full) are unchanged; xl/2xl/pill were renumbered to 4xl/5xl/6xl
# to make room for three genuinely new steps (xl=8px, 2xl=12px, 3xl=16px) that
# now match the 8/12/16px radius the prose guidelines (Styles.md) always
# assumed existed. No component below consumes the three new steps yet —
# demand-driven tokenization says leave them unconsumed until a component needs them.
rounded:
  xs: "{border.radius.xs}"     # 2px   → new, no consumer yet
  sm: "{border.radius.sm}"     # 4px   → unchanged
  md: "{border.radius.md}"     # 5px   → unchanged
  lg: "{border.radius.lg}"     # 6px   → unchanged
  xl: "{border.radius.xl}"     # 8px   → new, no consumer yet
  2xl: "{border.radius.2xl}"   # 12px  → new, no consumer yet
  3xl: "{border.radius.3xl}"   # 16px  → new, no consumer yet
  4xl: "{border.radius.4xl}"   # 24px  → was "xl" in previous scale
  5xl: "{border.radius.5xl}"   # 30px  → was "2xl" in previous scale
  6xl: "{border.radius.6xl}"   # 100px → was "pill" in previous scale
  full: "{border.radius.full}" # 999px → unchanged

# Spacing primitive scale expanded from 6 to 10 steps (base-4 increments added
# below 8px, and 40px/56px filled in above). Aliases below are remapped so
# every "{spacing.X}" reference already used in the components section still
# resolves to the SAME pixel value as before — only the underlying key changed.
spacing:
  4xs: null                     # 2px  → STILL NOT DEFINED in source, see Known Gaps
  3xs: "{spacing.padding.2xs}"  # 4px  → new: was undefined, now backed by a real token
  2xs: "{spacing.padding.xs}"   # 8px
  xs: "{spacing.padding.sm}"    # 12px
  sm: "{spacing.padding.md}"    # 16px
  md: "{spacing.padding.lg}"    # 24px
  lg: "{spacing.padding.xl}"    # 32px
  xl: "{spacing.padding.3xl}"   # 48px
  2xl: "{spacing.padding.5xl}"  # 64px

# Shadow token set renamed "Shadow" → "Elevation" and split into a two-tier
# primitive/semantic structure (x/y/blur/spread primitives referenced by
# elevation.xs–xl). Numeric values are unchanged; only the reference path
# changed. The flat rgba composites below still use the same brand-tinted
# alpha overlays (shadow.extra-light/light/medium/heavy), which were not
# renamed in this update.
shadow:
  xs: "0px 1px 4px 1px {shadow.extra-light}"   # brand alpha 7%
  sm: "1px 2px 12px 2px {shadow.light}"         # brand alpha 9%
  md: "1px 6px 20px 4px {shadow.medium}"        # brand alpha 12%
  lg: "1px 2px 40px 4px {shadow.heavy}"         # brand alpha 16%
  xl: "2px 2px 56px 9px {shadow.heavy}"

components:
  # ─── BUTTON ───────────────────────────────────────────────────────────────
  button-sm:
    padding: "{spacing.2xs} {spacing.sm}"       # 8px 16px
    label-typography: "{typography.body-3-medium}"
  button-md:
    padding: "{spacing.xs} {spacing.md}"        # 12px 24px
    label-typography: "{typography.body-2-semibold}"
  button-lg:
    padding: "{spacing.sm} {spacing.md}"        # 16px 24px
    label-typography: "{typography.body-1-semibold}"
  button-border-radius: "{rounded.lg}"          # 6px

  button-primary-default:
    backgroundColor: "{surface.brand-primary.base}"
    labelColor: "{text.inverse}"
  button-primary-hover:
    backgroundColor: "{surface.brand-primary.muted}"
    labelColor: "{text.inverse}"
  button-primary-pressed:
    backgroundColor: "{surface.brand-primary.strong}"
    labelColor: "{text.inverse}"
  button-primary-disabled:
    backgroundColor: "{surface.neutral.soft}"
    labelColor: "{text.secondary}"

  button-secondary-default:
    backgroundColor: "{surface.brand-secondary.base}"
    labelColor: "{text.brand-primary.base}"
  button-secondary-hover:
    backgroundColor: "{surface.brand-secondary.subtle}"
    labelColor: "{text.brand-primary.base}"
  button-secondary-pressed:
    backgroundColor: "{surface.brand-secondary.strong}"  # ⚠ NOT DEFINED in Colors - Semantic (old or new). Nearest primitive: yellow.700 (#8d7101). Needs a real semantic token before this is safe to ship.
    labelColor: "{text.brand-primary.base}"
  button-secondary-disabled:
    backgroundColor: "{surface.neutral.soft}"
    labelColor: "{text.secondary}"

  button-outline-default:
    backgroundColor: "transparent"   # was "{fill.brand-primary.none}" — not a real token; corrected to match button-tertiary's convention
    borderColor: "{border.interactive}"
    borderWidth: "{border.width.md}"            # 1.5px (was 1px)
    labelColor: "{text.brand-primary.base}"
  button-outline-hover:
    backgroundColor: "{surface.brand-primary.lighter}"
    borderColor: "{border.interactive}"
    labelColor: "{text.brand-primary.base}"
  button-outline-pressed:
    backgroundColor: "{surface.brand-primary.soft}"
    borderColor: "{border.interactive}"
    labelColor: "{text.brand-primary.base}"
  button-outline-disabled:
    backgroundColor: "{surface.neutral.lightest}"
    borderColor: "{border.disabled}"
    labelColor: "{text.secondary}"

  button-tertiary-default:
    backgroundColor: "transparent"
    labelColor: "{text.brand-primary.base}"
  button-tertiary-hover:
    backgroundColor: "transparent"
    labelColor: "{text.brand-primary.subtle}"
  button-tertiary-pressed:
    backgroundColor: "transparent"
    labelColor: "{text.brand-primary.subtle}"
  button-tertiary-disabled:
    backgroundColor: "transparent"
    labelColor: "{text.secondary}"

  # ─── INPUT FIELD ──────────────────────────────────────────────────────────
  input-field:
    height: "{spacing.xl}"                      # 48px
    borderRadius: "{rounded.md}"                # 5px
    borderWidth: "{border.width.lg}"            # 2px (was 1.5px)
    paddingHorizontalLeft: "{spacing.sm}"       # 16px
    paddingHorizontalRight: "{spacing.2xs}"     # 8px
    paddingVertical: "{spacing.2xs}"            # 8px
    iconSize: 20px
    label-typography: "{typography.caption-medium}"
    placeholder-typography: "{typography.body-3-medium}"
    helper-typography: "{typography.caption-medium}"

  input-field-default:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.default}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.tertiary}"
    helperColor: "{text.secondary}"
  input-field-filled:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.default}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.secondary}"
  input-field-active:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.active}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.secondary}"
  input-field-failed:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.danger}"
    iconColor: "{icon.danger}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.danger.base}"
  input-field-success:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.success}"
    iconColor: "{icon.success}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.success.base}"
  input-field-disabled:
    backgroundColor: "{surface.neutral.lightest}"
    borderColor: "{border.default}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.tertiary}"
    helperColor: "{text.secondary}"

  # ─── INPUT TEXTAREA ───────────────────────────────────────────────────────
  input-textarea:
    borderRadius: "{rounded.md}"                # 5px
    borderWidth: "{border.width.lg}"            # 2px (was 1.5px)
    paddingHorizontalLeft: "{spacing.sm}"       # 16px
    paddingHorizontalRight: "{spacing.2xs}"     # 8px
    paddingVertical: "{spacing.2xs}"            # 8px
    iconSize: 20px
    label-typography: "{typography.caption-medium}"
    placeholder-typography: "{typography.body-3-medium}"
    helper-typography: "{typography.caption-medium}"

  input-textarea-default:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.default}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.tertiary}"
    helperColor: "{text.secondary}"
  input-textarea-filled:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.default}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.secondary}"
  input-textarea-active:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.active}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.secondary}"
  input-textarea-failed:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.danger}"
    iconColor: "{icon.danger}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.danger.base}"
  input-textarea-success:
    backgroundColor: "{surface.neutral.white}"
    borderColor: "{border.success}"
    iconColor: "{icon.success}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.primary}"
    helperColor: "{text.success.base}"
  input-textarea-disabled:
    backgroundColor: "{surface.neutral.lightest}"
    borderColor: "{border.default}"
    iconColor: "{icon.neutral.muted}"
    labelColor: "{text.primary}"
    placeholderColor: "{text.tertiary}"
    helperColor: "{text.secondary}"

  # ─── LABEL ────────────────────────────────────────────────────────────────
  label:
    typography: "{typography.caption-medium}"
    paddingHorizontal: "{spacing.2xs}"          # 8px
    paddingVertical: "{spacing.4xs}"            # 2px
    borderRadiusSquare: "{rounded.sm}"          # 4px
    borderRadiusRound: "{rounded.6xl}"         # 100px
    borderWidthOutline: "{border.width.sm}"     # 1px (was 0.8px)

  label-green-default:
    backgroundColor: "{surface.success.soft}"
    textColor: "{text.success.strong}"
  label-green-outline:
    backgroundColor: "{surface.success.soft}"
    textColor: "{text.success.strong}"
    borderColor: "{border.success}"
  label-green-solid:
    backgroundColor: "{surface.success.base}"
    textColor: "{text.inverse}"

  label-red-default:
    backgroundColor: "{surface.danger.soft}"
    textColor: "{text.danger.strong}"
  label-red-outline:
    backgroundColor: "{surface.danger.soft}"
    textColor: "{text.danger.strong}"
    borderColor: "{border.danger}"
  label-red-solid:
    backgroundColor: "{surface.danger.base}"
    textColor: "{text.inverse}"

  label-yellow-default:
    backgroundColor: "{surface.warning.soft}"
    textColor: "{text.warning}"
  label-yellow-outline:
    backgroundColor: "{surface.warning.soft}"
    textColor: "{text.warning}"
    borderColor: "{border.warning}"
  label-yellow-solid:
    backgroundColor: "{surface.warning.base}"
    textColor: "{text.inverse}"

  label-blue-default:
    backgroundColor: "{surface.info.soft}"
    textColor: "{text.info}"
  label-blue-outline:
    backgroundColor: "{surface.info.soft}"
    textColor: "{text.info}"
    borderColor: "{border.info}"
  label-blue-solid:
    backgroundColor: "{surface.info.strong}"  # ⚠ NOT DEFINED in Colors - Semantic (old or new). Nearest existing value: blue.600 (#00458a) — matches old "info-strong". Needs a real semantic token before this is safe to ship.
    textColor: "{text.inverse}"

  label-dark-default:
    backgroundColor: "{surface.brand-primary.lighter}"
    textColor: "{text.brand-primary.base}"
  label-dark-outline:
    backgroundColor: "{surface.brand-primary.lighter}"
    textColor: "{text.brand-primary.base}"
    borderColor: "{border.interactive}"
  label-dark-solid:
    backgroundColor: "{surface.brand-primary.base}"
    textColor: "{text.inverse}"

  label-light-default:
    backgroundColor: "{surface.neutral.lightest}"
    textColor: "{text.brand-primary.base}"
  label-light-outline:
    backgroundColor: "{surface.neutral.lightest}"
    textColor: "{text.brand-primary.base}"
    borderColor: "{border.default}"
  label-light-solid:
    backgroundColor: "{surface.neutral.lighter}"
    textColor: "{text.primary}"

  # ─── CHIP ─────────────────────────────────────────────────────────────────
  chip-sm:
    height: 26px
    typography: "{typography.caption-medium}"
    paddingHorizontal: "{spacing.2xs}"          # 8px
    paddingVertical: "{spacing.4xs}"            # 2px
    iconSize: 12px
  chip-md:
    height: 30px
    typography: "{typography.body-3-medium}"
    paddingHorizontal: "{spacing.2xs}"          # 8px
    paddingVertical: "{spacing.3xs}"            # 4px
    iconSize: 16px
  chip-lg:
    height: 36px
    typography: "{typography.body-3-medium}"
    paddingHorizontal: "{spacing.xs}"           # 12px
    paddingVertical: "{spacing.3xs}"            # 4px
    iconSize: 16px
  chip-border-radius-round: "{rounded.4xl}"      # 24px
  chip-border-radius-square: "{rounded.md}"     # 5px

  chip-default:
    backgroundColor: "{surface.neutral.white}"
    labelColor: "{text.primary}"
    borderColor: "{border.default}"
    borderWidth: "{border.width.md}"            # 1.5px (was 1px)
    iconColor: "{icon.brand-primary.base}"
  chip-hover:
    backgroundColor: "{surface.brand-primary.lighter}"
    labelColor: "{text.primary}"
    borderColor: "{border.interactive}"
    borderWidth: "{border.width.md}"
    iconColor: "{icon.brand-primary.base}"
  chip-active:
    backgroundColor: "{surface.brand-primary.base}"
    labelColor: "{text.inverse}"
    iconColor: "{icon.inverse}"
  chip-pressed:
    backgroundColor: "{surface.brand-primary.strong}"
    labelColor: "{text.inverse}"
    iconColor: "{icon.inverse}"
  chip-disabled:
    backgroundColor: "{surface.neutral.lighter}"
    labelColor: "{text.primary}"
    borderColor: "{border.interactive}"
    borderWidth: "{border.width.md}"
    iconColor: "{icon.brand-primary.base}"

  # ─── BADGE (Icon / Image / Text) ──────────────────────────────────────────
  badge-border-radius: "{rounded.full}"         # 999px
  badge-size-sm: 16px
  badge-size-md: 20px
  badge-size-lg: 32px
  badge-size-xl: 48px

  badge-icon-sm:
    dimension: 16px
    iconSize: 8px
  badge-icon-md:
    dimension: 20px
    iconSize: 12px
  badge-icon-lg:
    dimension: 32px
    iconSize: 22px
  badge-icon-xl:
    dimension: 48px
    iconSize: 30px
  badge-icon-dark:
    backgroundColor: "{icon.brand-primary.base}"
    iconColor: "{icon.inverse}"
  badge-icon-light:
    backgroundColor: "{surface.neutral.lighter}"
    iconColor: "{icon.brand-primary.base}"
  badge-icon-no-fill:
    iconColor: "{icon.brand-primary.base}"

  badge-image-border-width: "{border.width.md}" # 1.5px (was 1px)
  badge-image-border-dark:
    borderColor: "{surface.neutral.lighter}"

  badge-text-light:
    backgroundColor: "{surface.neutral.lighter}"
    labelColor: "{text.brand-primary.base}"
  badge-text-dark:
    backgroundColor: "{surface.brand-primary.base}"
    labelColor: "{text.inverse}"
  badge-text-sm:
    dimension: 16px
    fontSize: 6px                               # intentionally hardcoded — below primitive scale
    fontFamily: "{font.family.Inter}"
    fontWeight: "{font.weight.300}"             # Semi Bold
    lineHeight: "{line-height.desktop.100}"     # 16px
    letterSpacing: "{letter-spacing.20}"
  badge-text-md:
    dimension: 20px
    fontSize: 8px
    fontFamily: "{font.family.Inter}"
    fontWeight: "{font.weight.300}"
    lineHeight: "{line-height.desktop.100}"
    letterSpacing: "{letter-spacing.20}"
  badge-text-lg:
    dimension: 32px
    fontSize: 10px
    fontFamily: "{font.family.Inter}"
    fontWeight: "{font.weight.300}"
    lineHeight: "{line-height.desktop.100}"
    letterSpacing: "{letter-spacing.20}"
  badge-text-xl:
    dimension: 48px
    typography: "{typography.body-2-semibold}"

  # ─── BADGE DOT ────────────────────────────────────────────────────────────
  badge-dot-sm:
    dimension: 6px
    borderRadius: "{rounded.full}"
  badge-dot-md:
    dimension: 10px
    borderRadius: "{rounded.full}"
  badge-dot-lg:
    dimension: 16px
    borderRadius: "{rounded.full}"
    fontSize: 8px
    fontFamily: "{font.family.Inter}"
    fontWeight: "{font.weight.300}"
    lineHeight: "{line-height.desktop.100}"
    letterSpacing: "{letter-spacing.20}"
  badge-dot-xl:
    borderRadius: "{rounded.6xl}"
    paddingHorizontal: 6px
    paddingVertical: "{spacing.scale-2}"        # 2px
    typography: "{typography.small-semibold}"

  badge-dot-color:
    backgroundColor: "{surface.danger.base}"
    labelColor: "{text.inverse}"
  badge-dot-border-dark:
    borderColor: "{surface.neutral.lighter}"

  # ─── TAB ──────────────────────────────────────────────────────────────────
  tab:
    height: 40px
    indicatorHeight: 4px
    indicatorBorderRadius: "{rounded.6xl}"
    iconSize: 16px
    typography: "{typography.body-3-medium}"    # same as button-md label

  tab-default:
    labelColor: "{text.primary}"
    iconColor: "{icon.neutral.soft}"
  tab-hover:
    labelColor: "{text.brand-primary.muted}"
    iconColor: "{icon.neutral.soft}"
  tab-active:
    labelColor: "{text.primary}"
    iconColor: "{icon.neutral.soft}"
    indicatorColor: "{surface.brand-secondary.base}"
  tab-disabled:
    labelColor: "{text.tertiary}"
    iconColor: "{icon.neutral.soft}"

  # ─── CARD ARTICLE — FEATURED ──────────────────────────────────────────────
  card-article-featured:
    thumbnail-width: 256px
    thumbnail-height: 160px
    thumbnail-border-radius: "{rounded.sm}"     # 4px
    title-typography: "{typography.body-1-semibold}"
    desc-typography: "{typography.body-2-regular}"
    date-typography: "{typography.body-3-medium}"
    author-typography: "{typography.body-3-medium}"
    titleColor: "{text.primary}"
    descColor: "{text.primary}"
    dateColor: "{text.secondary}"
    authorColor: "{text.brand-primary.muted}"

  # ─── CARD ARTICLE — GRID ──────────────────────────────────────────────────
  card-article-grid:
    thumbnail-width: 160px
    thumbnail-height: 256px
    thumbnail-border-radius: "{rounded.md}"     # 5px
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-medium}"
    titleColor: "{text.primary}"
    dateColor: "{text.secondary}"

  # ─── CARD ARTICLE — SIDE ──────────────────────────────────────────────────
  card-article-side:
    thumbnail-width: 176px
    thumbnail-height: 117px
    thumbnail-border-radius: "{rounded.md}"     # 5px
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-medium}"
    titleColor: "{text.primary}"
    dateColor: "{text.secondary}"

  # ─── CARD ARTICLE — MINIMAL ───────────────────────────────────────────────
  card-article-minimal:
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-medium}"
    titleColor: "{text.primary}"
    dateColor: "{text.secondary}"

  # ─── CARD EVENT ───────────────────────────────────────────────────────────
  card-event:
    borderRadius: "{rounded.lg}"                # 6px
    borderWidth: "{border.width.md}"            # 1.5px (was 1px)
    borderColor: "{surface.neutral.lightest}"       # #f5f7f9
    backgroundColor: "{surface.neutral.white}"
    thumbnailBorderRadiusTop: "{rounded.lg}"    # 6px
    thumbnailBorderRadiusBottom: 0px
    contentPaddingHorizontal: "{spacing.sm}"    # 16px
    contentPaddingVertical: "{spacing.xs}"      # 12px
    title-typography: "{typography.body-2-semibold}"
    date-typography: "{typography.body-3-regular}"
    location-typography: "{typography.body-3-regular}"
    narasumber-typography: "{typography.body-3-regular}"
    price-value-typography:
      fontFamily: "{font.family.Inter}"
      fontWeight: "{font.weight.300}"           # Semi Bold
      fontSize: "{font.size.mobile.600}"        # 16px
      lineHeight: "{line-height.mobile.500}"    # 26px
      letterSpacing: "{letter-spacing.0}"
    price-label-typography:
      fontFamily: "{font.family.Inter}"
      fontWeight: "{font.weight.100}"           # Regular
      fontSize: "{font.size.mobile.400}"        # 12px
      lineHeight: "{line-height.mobile.300}"    # 20px
      letterSpacing: "{letter-spacing.0}"
    titleColor: "{text.primary}"
    dateColor: "{text.secondary}"
    locationColor: "{text.secondary}"
    narasumberColor: "{text.secondary}"
    priceLabelColor: "{text.tertiary}"
    priceValueColor: "{text.primary}"
---

## Overview

Hukumonline (HOL) is Indonesia's leading legal information platform. Its design language
reflects authority, clarity, and trust — values critical in the legal domain. The canvas
is clean white (`{colors.neutral-white}`) with near-invisible neutral hairlines
(`{colors.border-default}` — `#cfd9e2`) doing separation work rather than heavy shadows.
Depth, when needed, is expressed through brand-tinted box shadows (brand navy at low alpha).

The brand runs on two colors: a deep **HOL Navy** (`{colors.brand-primary-base}` — `#003366`)
carrying every primary CTA, active indicators, link text, and navigation; and a warm
**HOL Gold** (`{colors.brand-secondary-base}` — `#f8ca0f`) reserved for secondary
call-to-action moments and active tab indicators. This restraint keeps pages from feeling
cluttered — most surfaces are white with navy type, with gold appearing only at deliberate
moments.

Typography uses **Nunito Sans** for all display and heading levels — confident and approachable
without being heavy-handed — and **Inter** for body, UI labels, and data. At body sizes
(14–18px) Inter maximises legibility for long-form legal text. Component labels (buttons,
chips, tabs) and cards both lean on Inter to keep UI chrome quiet and let content breathe.

**Key Characteristics:**
- Two-color brand system: navy primary + gold secondary. Status colors (green, red, yellow,
  blue) are used for semantic meaning only — never as accent decoration.
- Shadow as brand tone: all elevation uses box shadows with brand navy alpha rather than
  neutral gray shadows, keeping depth warm rather than cold.
- Typography hierarchy is size-and-weight-driven, not decorative: display headings are
  Nunito Sans at modest Extra Bold; body is Inter regular/medium.
- Card components (article + event) rely entirely on layout, typography, and text color
  — no card-level background token (defaults to white canvas) and no card border except
  on card-event.
- Interactive components (button, chip, tab) use the full navy scale across states:
  lighter fills on hover, base on default active, strong on pressed.

---

## Colors

### Brand & Accent

- **HOL Navy — base** (`{colors.brand-primary-base}` — `#003366`): The primary brand color.
  Appears on primary buttons, active tab indicators (via `text.brand-primary.base`), active
  chip fills, icon tints, and link text. Used at full opacity only for primary moments.
- **HOL Navy — muted** (`{colors.brand-primary-muted}` — `#0052a3`): Hover state for primary
  button and outline button border. Also used as `text.brand-primary.muted` for author names
  in article cards.
- **HOL Navy — subtle** (`{colors.brand-primary-subtle}` — `#2877c5`): Active border on
  focused input fields (`border.active`).
- **HOL Navy — soft** (`{colors.brand-primary-soft}` — `#89bff4`): Pressed background on
  outline button. Mid-range fill in brand tinting contexts.
- **HOL Navy — lighter** (`{colors.brand-primary-lighter}` — `#e0ecf9`): Hover background
  for outline button and chip. Light background for dark-variant label and badge-icon-light.
- **HOL Gold — base** (`{colors.brand-secondary-base}` — `#f8ca0f`): Secondary button
  background. Active tab indicator fill. Use sparingly — one gold moment per page is the
  intended rhythm.
- **HOL Gold — subtle** (`{colors.brand-secondary-subtle}` — `#ffe168`): Secondary button
  hover background.
- **HOL Gold — strong** (`{colors.brand-secondary-strong}` — `#8d7101`): Secondary button
  pressed background.

### Surface

- **White** (`{colors.neutral-white}` — `#ffffff`): Default canvas and card background.
  All components default to this unless explicitly overridden.
- **Lightest** (`{colors.neutral-lightest}` — `#f5f7f9`): Disabled input background.
  Card-event border color. Used wherever a barely-there background lift is needed.
- **Lighter** (`{colors.neutral-lighter}` — `#cfd9e2`): Light chip disabled background.
  Badge-image border in dark context. Badge-icon-light background.

### Text

- **Primary** (`{colors.text-primary}` — `#2b4156`): Default body text. Card titles, card
  price values, all primary content reading.
- **Secondary** (`{colors.text-secondary}` — `#607a93`): Supporting text — dates, locations,
  narasumber labels, helper text in inputs.
- **Tertiary** (`{colors.text-tertiary}` — `#8398ab`): Placeholder text in inputs, price
  label in card-event.
- **Inverse** (`{colors.text-inverse}` — `#ffffff`): Text on dark backgrounds — primary
  button labels, solid label text, active chip label, badge-dot label.
- **Brand Primary** (`{colors.text-brand-primary}` — `#003366`): Used for author names in
  cards (via muted alias), outline/tertiary button labels, label-dark text, chip labels.

### Border

- **Default** (`{colors.border-default}` — `#cfd9e2`): Standard input border, default chip
  border, label-light outline border.
- **Active** (`{colors.border-active}` — `#2877c5`): Focused input field border.
- **Brand** (`{colors.border-brand}` — `#0052a3`): Outline button border, hover chip border,
  label-dark outline border.
- **Danger** (`{colors.border-danger}` — `#dc381f`): Failed input border, red label outline.
- **Success** (`{colors.border-success}` — `#00875a`): Success input border, green label
  outline.
- **Warning** (`{colors.border-warning}` — `#daa520`): Yellow label outline.
- **Info** (`{colors.border-info}` — `#0177cc`): Blue label outline.
- **Disabled** (`{colors.border-disabled}` — `#a8b8c7`): Outline button border in disabled
  state.

### Semantic

- **Success** (`{colors.success-base}` — `#00875a` / soft `#eefdf6`): Green label
  backgrounds, success input icon and helper text.
- **Danger** (`{colors.danger-base}` — `#dc381f` / soft `#ffeff0`): Red label, failed input
  state, badge-dot background.
- **Warning** (`{colors.warning-base}` — `#daa520` / soft `#fff9e3`): Yellow label states.
- **Info** (`{colors.info-base}` — `#0177cc` / soft `#ebf6fc` / strong `#00458a`): Blue label
  states. Info-strong used for solid blue label to ensure text contrast.

---

## Typography

HOL uses two typefaces across the entire system.

**Nunito Sans** handles all display and heading scales (heading-1 through heading-4, title-1,
title-2, subtitle). It is friendly and readable at large sizes without appearing either too
corporate or too casual — appropriate for a platform that is authoritative but not cold.

**Inter** handles all body copy, UI labels, captions, and data text. Its optical sizing and
open apertures make it exceptionally legible at the 12–18px range where legal content is
consumed.

| Token | Family | Size | Weight | Line Height |
|---|---|---|---|---|
| `{typography.heading-1-extrabold}` | Nunito Sans | 50px | Extra Bold | 60px |
| `{typography.heading-2-bold}` | Nunito Sans | 42px | Bold | 50px |
| `{typography.heading-3-semibold}` | Nunito Sans | 35px | Semi Bold | 46px |
| `{typography.heading-4-bold}` | Nunito Sans | 29px | Bold | 40px |
| `{typography.title-1-extrabold}` | Nunito Sans | 24px | Extra Bold | 36px |
| `{typography.title-2-bold}` | Nunito Sans | 20px | Extra Bold | 30px |
| `{typography.subtitle-bold}` | Nunito Sans | 18px | Extra Bold | 30px |
| `{typography.body-1-semibold}` | Inter | 18px | Semi Bold | 28px |
| `{typography.body-1-regular}` | Inter | 18px | Regular | 28px |
| `{typography.body-2-semibold}` | Inter | 16px | Semi Bold | 26px |
| `{typography.body-2-regular}` | Inter | 16px | Regular | 26px |
| `{typography.body-3-medium}` | Inter | 14px | Medium | 22px |
| `{typography.body-3-regular}` | Inter | 14px | Regular | 22px |
| `{typography.caption-medium}` | Inter | 12px | Medium | 20px |
| `{typography.small-semibold}` | Inter | 10px | Semi Bold | 16px |

### Principles

Body-1 through Body-3 carry all card content, form inputs, and navigation labels — the
typographic workhorse range. Caption-medium is used exclusively for input labels and helper
text, keeping form chrome visually subordinate to input values. Badge text (sm/md/lg) uses
raw font-size values (6px, 8px, 10px) intentionally below the primitive scale to fit count
numbers inside small circular containers — these are not typos.

### Note on Font Substitutes

Nunito Sans and Inter are both available on Google Fonts and are the canonical HOL typefaces.
If either is unavailable, system sans-serif is the fallback — never substitute a serif face.

---

## Layout

HOL spacing is a fixed numeric scale (2 / 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 px) named
with t-shirt sizes from `4xs` to `2xl`. All component padding and gaps reference semantic
spacing tokens, never raw pixel values.

| Token | Value | Common Use |
|---|---|---|
| `{spacing.4xs}` | 2px | Badge-dot XL padding vertical |
| `{spacing.3xs}` | 4px | Chip SM/MD padding vertical, card-article-minimal gap |
| `{spacing.2xs}` | 8px | Input padding, chip SM/MD horizontal, button SM padding vertical |
| `{spacing.xs}` | 12px | Button MD padding vertical, chip LG padding vertical |
| `{spacing.sm}` | 16px | Button SM horizontal, input left padding, card-event content padding |
| `{spacing.md}` | 24px | Button MD/LG horizontal padding, card gaps |
| `{spacing.lg}` | 32px | Section spacing within cards |
| `{spacing.xl}` | 48px | Input field height |
| `{spacing.2xl}` | 64px | Large section padding |

Card article components define gap values in prose (not as Variables) because they describe
layout behaviour between sibling components rather than padding on a single element:
featured gap = 16px horizontal (thumbnail → content), grid gap = 8px vertical, side gap =
16px horizontal, minimal gap = 4px (title → date only, no thumbnail).

---

## Elevation

HOL uses a single family of box shadows, all tinted with brand navy alpha rather than neutral
gray. This keeps depth warm and on-brand. There are five tiers:

| Token | Value | Usage |
|---|---|---|
| `{shadow.xs}` | 0 1 4 1 / brand-alpha-7% | Subtle card lift, tooltip |
| `{shadow.sm}` | 1 2 12 2 / brand-alpha-9% | Card-event hover, dropdown |
| `{shadow.md}` | 1 6 20 4 / brand-alpha-12% | Modal, active card |
| `{shadow.lg}` | 1 2 40 4 / brand-alpha-16% | Navigation drawer, sticky header |
| `{shadow.xl}` | 2 2 56 9 / brand-alpha-16% | Full-page overlay, dialog |

Card article variants (featured, grid, side, minimal) use no shadow — separation from the
canvas is achieved through layout spacing alone. Card-event uses `{shadow.sm}` on hover.

---

## Components

**`button-sm`** — Small button for compact contexts (table actions, inline CTAs). Padding
`{spacing.2xs}` × `{spacing.sm}` (8px × 16px). Label uses `{typography.body-3-medium}`.
Applies `{button-border-radius}` (6px) on all four corners.

**`button-md`** — Standard button, the most common size. Padding `{spacing.xs}` ×
`{spacing.md}` (12px × 24px). Label uses `{typography.body-2-semibold}`.

**`button-lg`** — Large button for hero or prominent action areas. Padding `{spacing.sm}` ×
`{spacing.md}` (16px × 24px). Label uses `{typography.body-1-semibold}`.

**`button-primary-*`** — The HOL navy fill button. Default: `{surface.brand-primary.base}`
background / `{text.inverse}` label. Hover: background lightens to `{surface.brand-primary.muted}`.
Pressed: background deepens to `{surface.brand-primary.strong}`. Disabled: neutral soft fill /
secondary text — icon and label both muted, no border.

**`button-secondary-*`** — Gold fill button. Default: `{surface.brand-secondary.base}` / label
`{text.brand-primary.base}`. Preserves the navy label across all interactive states for
contrast. Disabled follows same neutral-soft pattern as primary.

**`button-outline-*`** — Transparent background with `{border.interactive}` (1px) border and navy
label. Hover introduces a `{surface.brand-primary.lighter}` fill. Pressed fills to
`{surface.brand-primary.soft}`. Disabled collapses border to `{border.disabled}` and label to
`{text.secondary}`.

**`button-tertiary-*`** — Ghost button: always transparent background. Label only, no border.
Hover and pressed shift label to `{text.brand-primary.subtle}`. Used for low-emphasis actions.
Loading state shows a spinner inside the button; fixed-width layout prevents resize on
state change. Button groups arrange two buttons side by side — primary left, secondary or
outline right is the default order.

**`input-field`** — Single-line text input. Height fixed at 48px (`{spacing.xl}`). Left
padding `{spacing.sm}` (16px), right padding `{spacing.2xs}` (8px), vertical padding
`{spacing.2xs}` (8px). Border `{border.width.lg}` (2px, was 1.5px) with radius `{rounded.md}` (5px).
Anatomy: label above field, placeholder inside, trailing icon (optional), helper text below.
Icon size 20px. Six states: default, filled, active (border turns `{border.active}`, navy
subtle), failed (border and icon turn danger, helper text `{text.danger.base}`), success
(border and icon turn success, helper `{text.success.base}`), disabled (background
`{surface.neutral.lightest}`, placeholder `{text.tertiary}`). The tooltip coachmark appearing
on hover is a related component, not part of the input token set.

**`input-textarea`** — Multi-line text area sharing the same token architecture as
`input-field` (same border radius, width, horizontal padding). Height is not fixed — it
expands with content. The trailing icon (copy) floats in the top-right of the content area.
Same six states apply with identical color logic.

**`label`** — A small non-interactive visual tag. Two shape variants: **Square**
(`{rounded.sm}` — 4px) for categories and statuses; **Round** (`{rounded.6xl}` — 100px)
for tags and softer contexts. Typography always `{typography.caption-medium}` (12px Medium).
Padding `{spacing.2xs}` horizontal / `{spacing.4xs}` vertical (8px / 2px). Three style
variants per color: **Default** (soft fill background, semantic-strong text — grabs
attention), **Outline** (same soft fill + 1px semantic border, was 0.8px — subtle, detailed look),
**Solid** (full semantic fill, inverse text — highest emphasis). Six color families: green
(success), red (danger), yellow (warning), blue (info), dark (brand navy), light (neutral).
Icon placement is left-only. Max character limit is 30 characters. Labels sit inline with
primary content on the baseline.

**`chip-sm / chip-md / chip-lg`** — Interactive filter and selection components. Two shape
variants per size: **Round** (`{rounded.4xl}` — 24px, for consumer-facing filters) and
**Square** (`{rounded.md}` — 5px, for professional/data contexts). Icons are optional;
position is left when present. Max character limit 20 characters. States: default (white
fill, neutral border), hover (navy lighter fill, brand border), active (navy base fill,
inverse text — selected), pressed (navy strong fill, inverse text), disabled (lighter fill,
brand border — muted). Chips group together by function — filter chips group by category,
never mix categories in one row.

**`badge-icon-sm/md/lg/xl`** — Circular icon containers. Always `{rounded.full}` (999px).
Two color variants: **dark** (navy background, inverse icon) and **light** (neutral lighter
background, navy icon). **No-fill** variant shows only the icon with no container.
Icon sizes scale with dimension (8 / 12 / 22 / 30px inside 16 / 20 / 32 / 48px containers).

**`badge-image-*`** — Circular avatar/image container. Shares the same size scale (sm–xl).
In dark context, a `{border.width.md}` (1.5px, was 1px) border uses `{surface.neutral.lighter}` to
separate stacked images. Badge-images can stack with an overlap layout; the number of
visible avatars before a count badge is contextual.

**`badge-text-sm/md/lg/xl`** — Numeric count badge. SM/MD/LG sizes use intentionally
sub-scale font sizes (6px / 8px / 10px) in Inter — these fit count digits inside 16/20/32px
circles and are not a mistake. XL (48px) switches to `{typography.body-2-semibold}`. Two
color variants: **light** (neutral lighter bg, navy label) and **dark** (navy bg, inverse
label). Max 2 characters before switching to "99+" display. Always `{rounded.full}` radius.

**`badge-dot-sm/md/lg/xl`** — Notification dot badge. SM (6px) and MD (10px) are color-only
dots — no text. LG (16px) adds a compact label (8px Inter Semi Bold). XL uses
`{rounded.6xl}` with `{typography.small-semibold}` and becomes a pill-shaped notification
badge for high-count scenarios. All colored `{surface.danger.base}` / `{text.inverse}`. In
dark contexts a `{surface.neutral.lighter}` border separates the dot from the host surface.
Badge placement is top-right relative to the host element.

**`tab`** — Navigation tab bar. Fixed height 40px. Two layout variants: **Horizontal** (side
by side, for page sections or topic navigation) and **Vertical** (stacked, for sidebar or
modal navigation). Typography `{typography.body-3-medium}` (same as button-md label) to
keep tabs visually harmonious with button chrome. Active indicator: 4px tall bar,
`{rounded.6xl}` radius, colored `{surface.brand-secondary.base}` (HOL Gold). The indicator
sits at the bottom edge for horizontal tabs, right edge for vertical tabs. States: default
(primary label, soft icon), hover (brand-primary-muted label), active (primary label +
gold indicator), disabled (tertiary label — cannot receive interaction). Use a single active
tab at a time. Arrange tabs in a single row — never multi-row. Place tabs at the top of
their content area. Max character limit enforces readability; use short and distinct labels
and cut after two words. Related components: Breadcrumb (for page hierarchy), Pagination (for
sequential content sets).

**`card-article-featured`** — Horizontal card: thumbnail left (256 × 160px, `{rounded.sm}`
— 4px), content area right. Gap between thumbnail and content: 16px horizontal. Content
internal gap: 4px vertical between title, description, and metadata. Metadata row (date +
author) has 16px internal gap. Title uses `{typography.body-1-semibold}`, description
`{typography.body-2-regular}`, date and author `{typography.body-3-medium}`. Author text
uses `{text.brand-primary.muted}` (navy muted) to signal it is a clickable link. On hover,
title gains an underline. Cards in a list are separated by 32px vertical gap.

**`card-article-grid`** — Vertical card: thumbnail on top (160 × 256px — note width ×
height, portrait orientation, `{rounded.md}` — 5px), content below. Gap between thumbnail
and content: 8px vertical. Content internal gap: 4px (title → date). Title uses
`{typography.body-2-semibold}`, date `{typography.body-3-medium}`. On hover, title gains
an underline. Cards in a grid are separated by 32px gap.

**`card-article-side`** — Compact horizontal card: thumbnail left (176 × 117px,
`{rounded.md}` — 5px), content right. Gap between thumbnail and content: 16px horizontal.
Content internal gap: 4px (title → date). Same typography as grid variant. On hover, title
gains an underline. Cards in a list are separated by 24px vertical gap.

**`card-article-minimal`** — Text-only card: no thumbnail. Title and date with 4px gap.
Title `{typography.body-2-semibold}`, date `{typography.body-3-medium}`. On hover, a
primary-MD-size button labelled "Daftar" appears. Cards in a list are separated by 32px gap.

**`card-event`** — Vertical card with full-bleed thumbnail at top. Thumbnail border radius
follows the card only on top corners (`{rounded.lg}` — 6px), bottom corners are 0. Card
itself has `{rounded.lg}` radius, `{border.width.md}` (1.5px, was 1px) border in `{surface.neutral.lightest}`
(`#f5f7f9`), white background. Content area padding: `{spacing.sm}` horizontal (16px),
`{spacing.xs}` vertical (12px). Label chips (event type badges using the Label component)
sit above the title; gap between label and title is 8px. Content rows — title, date, location,
narasumber — have 8px vertical gap between each. Price row has 8px gap between price-label
and price-value. Narasumber row shows Badge-image components (LG size) for avatar display.
Price-value uses Inter Semi Bold at 16px with Inter Regular 12px for the "Mulai dari" label
above. On hover, a primary-MD "Daftar" button appears. Cards in a grid are separated by
32px gap.

---

## Responsive Behavior

Breakpoint definitions for HOL are not yet formally extracted from a specification source.
The following is an anticipated range based on the platform's existing web-first orientation.

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 768px | Single-column layout; card-article-featured stacks vertically; tab bar collapses or scrolls horizontally |
| Tablet | 768–1024px | Two-column card grids; navigation condenses |
| Desktop | 1024–1440px | Full multi-column layouts; card grids at 3-up or 4-up |
| Wide | > 1440px | Content capped; gutters absorb excess width |

### Touch Targets

- Primary CTAs (button-md, button-lg): meet ≥ 44 × 44px WCAG AAA via height 48px and
  horizontal padding.
- Input fields: 48px fixed height meets touch target requirements.
- Chips: SM (26px height) falls below the 44px threshold — use MD or LG in mobile contexts.
- Tabs: 40px height — acceptable for tap targets at full-width tab rows; add vertical
  padding on mobile if tabs are narrow.

---

## Known Gaps

### Resolved by this token update
- Garbage tokens (`Dashboard - Level 1`, `Dashboard - Home`, `Spinner`, `fill.Color = #ffffff00`)
  that previously polluted the primitive/semantic color sets have been removed. ✅
- Border-radius gap between 6px and 24px is closed — `xl`(8px), `2xl`(12px), `3xl`(16px) now
  exist as real primitives, matching what the prose guidelines (Styles.md) always assumed. ✅
- Spacing gap below 8px is closed — a real 4px step (`spacing.padding.2xs`) now exists,
  and 40px/56px steps fill in what was previously a jump straight from 32px to 48px. ✅
- `spacing-letter.60` / `.80` (referenced by heading-2-bold and heading-1-extrabold
  respectively) were previously undefined in the primitive set — they now exist under the
  renamed `letter-spacing.*` namespace. ✅
- Font-weight is no longer a single ambiguous 5-step scale — Nunito Sans and Inter now
  have separate, correctly CSS-labelled weight ramps. ✅

### Still open — carried over or newly surfaced
- **`text.warning` data error is NOT resolved.** It still resolves to `#6f4e37` (now
  `yellow.800`, was `yellow.500`), a brown outside the yellow hue family. Renumbered, not
  fixed — still needs a real correction in Figma Variables.
- `surface.brand-secondary.strong` (used by `button-secondary-pressed`) and
  `surface.info.strong` (used by `label-blue-solid`) are **not defined** in either the old
  or the new semantic set — both were already broken before this update and remain broken.
  See inline `⚠` comments in the `components:` section above.
- `border.width` values changed (sm 0.8→1px, md 1→1.5px, lg 1.5→2px) — every component
  using a border got very slightly thicker. This is a visual change, not just a rename;
  confirm it's intentional before shipping.
- Breakpoints and responsive rules are not formally specified — values above are provisional.
- Animation and transition timings (button press, chip selection, tab switch) are not
  documented.
- Dark mode is not a documented variant. HOL renders a single light canvas mode.
- Mobile-specific typography now exists in the source (`Typo – Semantic` resolves separate
  desktop/mobile sizes) but is not yet surfaced anywhere in this document — every entry in
  the `typography:` block above is desktop-only.
- Card-article components have no explicit background or border token — they inherit the
  white canvas. If a surfaced card variant (with explicit border or shadow) is introduced,
  new tokens are needed.
- `card-event.color.border` was hardcoded as `#f5f7f9` in the source export; mapped here
  to `{surface.neutral.lightest}` pending formal token update in Figma Variables.
- Hover interaction behaviors (underline on card titles, "Daftar" button appearance) are
  documented in prose only — no interaction tokens exist in the current Variables set.
- Narasumber badge stacking logic (how many avatars before a count badge) is contextual and
  not defined by a token.
- The `thumbnail-width` on card-event is not set in component tokens — thumbnail fills
  full card width. Exact thumbnail height is pending decision.
- Form error and success state illustrations (empty state art, inline error icons beyond
  color) are out of scope.
- Sub-components referenced within card-event (Label, Badge-image, Button primary-MD) rely
  on their own component tokens; cross-component composition rules are described in prose
  only.
- The three newly-added radius steps (`rounded.xl`=8px, `rounded.2xl`=12px, `rounded.3xl`=16px)
  and `rounded.xs`=2px have no consuming component yet. Per demand-driven tokenization,
  leave them undocumented at the component level until a real component needs them — don't
  retrofit existing components just because the steps now exist.
