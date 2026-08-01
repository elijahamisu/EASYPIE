# Palette's UX Journal

## 2025-02-23 - Screen Reader and Keyboard Accessibility on Icon-Only Buttons
**Learning:** Icon-only buttons (such as notification bells, copy buttons, and logouts) lack accessible text, rendering them completely silent or useless for screen readers. Furthermore, lacking a distinct focus indicator (`:focus-visible`) makes keyboard-only navigation extremely difficult and disorienting.
**Action:** Always add explicit `aria-label` and `title` attributes to icon-only buttons, and style `:focus-visible` focus rings to ensure interactive elements are clear and accessible.
