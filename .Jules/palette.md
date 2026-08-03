# Palette's Journal - EASYPIE

## 2025-02-13 - Icon-only Buttons Accessibility
**Learning:** Icon-only interactive elements (like the notification badge, logout buttons, and copy/clipboard action buttons) are completely non-descriptive for screen readers without clear ARIA labels. They must always have an explicit `aria-label` defining their behavior.
**Action:** Always inspect the layout for raw font-awesome or SVG icon buttons lacking text content, and add an appropriate `aria-label`.
