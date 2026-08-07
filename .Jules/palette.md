# Palette's UX & Accessibility Journal - EASYPIE

## 2026-08-07 - Accessible Floating Toast Copy-Notification Pattern
**Learning:** Browser-native alerts on clipboard actions disrupt the user journey. Replaced them with floating toast notifications styled with existing design system variables (such as `--success`). To ensure screen readers announce these notifications immediately, the element must contain `role="status"` and `aria-live="polite"` attributes. Rapid succession copying must be handled gracefully by storing the timeout globally and calling `clearTimeout` prior to re-triggering the animation, preventing overlapping animation cycles and early visual cutoffs. For overlays (like modal dialogs), a high `z-index` (e.g. `3000`) is required to prevent the toast from being obscured.
**Action:** Use the semantic `role="status"` and `aria-live="polite"` with `clearTimeout` reset logic for any micro-feedback notification in the EASYPIE design system.
