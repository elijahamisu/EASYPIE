# Palette's UX Journal

## 2026-10-24 - Copied feedback micro-interactions vs. browser alerts
**Learning:** In mobile-first fintech platforms like EASYPIE, using native browser `alert()` pop-ups for copy events (such as copying referral links or codes) is extremely disruptive to the user flow. It halts all JavaScript execution, demands an extra user tap to dismiss, and cheapens the premium dark-themed aesthetic. Transitioning to instant inline icon micro-interactions (e.g., swapping a copy icon to a checkmark icon) maintains design continuity and provides fluid, non-blocking visual feedback.
**Action:** Always replace blocking alerts with temporary icon/text state changes (e.g., `fa-copy` to `fa-check`) on copy buttons. Ensure all icon-only interactive elements contain unambiguous `aria-label` tags for screen readers.
