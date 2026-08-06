# Palette's UX & Accessibility Journal

This file contains critical learnings, guidelines, and standards for the EASYPIE design system and user experience design patterns.

## 2024-11-20 - [Unified and Delightful Copy Notifications]
**Learning:** Browser-native copy alerts (`alert()`) are extremely disruptive and degrade the premium feel of a mobile-first dark-themed fintech application. High-fidelity visual state transitions or styled toast notifications are much more graceful and non-disruptive.
**Action:** Replace `alert('Referral code copied!')` in dashboard.html and references to alerts during copy/clipboard interactions with highly polished inline feedback or stylized floating toast notifications. Ensure screen readers are notified of updates (e.g. via `aria-live` or clear accessibility hints).
