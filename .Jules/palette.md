# Palette's UX Journal

Critical UX/accessibility learnings for the EASYPIE premium NGN investment platform.

## 2026-02-15 - Premium Visual Consistency with Non-Disruptive Feedback

**Learning:** Using browser-native `alert()` popups in a dark-themed, premium fintech application is jarring and ruins the luxury experience, while causing keyboard focus and screen reader confusion. Inline or beautifully animated non-disruptive micro-toasts with explicit ARIA-live/alert roles preserve the visual flow and improve screen reader accessibility.
**Action:** Always replace standard `alert()` or `confirm()` with custom, styled dark-mode toasts and accessible modals across user-facing pages, and ensure icon-only buttons have descriptive `aria-label` attributes for assistive technologies.
