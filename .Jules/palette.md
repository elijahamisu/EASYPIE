# Palette UX Journal

## 2025-02-17 - [Initial setup]
**Learning:** Initial Palette UX setup.
**Action:** Always verify color contrast, accessibility, and ARIA labels.

## 2025-02-17 - [Non-disruptive Inline Clipboard Copy Feedback]
**Learning:** Browser-native alerts for clipboard copy operations are highly disruptive to mobile web applications. Changing the copy trigger's local state (transforming the icon to a checkmark or changing the text to "Copied!" and changing the button background to `var(--success)`) for 2 seconds provides instant, delighting, and non-disruptive copy feedback.
**Action:** Replace all generic `alert()` calls on copy actions with local inline state transitions that leverage existing design tokens and revert gracefully.
