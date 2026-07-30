# Palette's Journal - EASYPIE

## 2025-02-18 - Non-blocking Copy Toasts and Icon Button Accessibility
**Learning:** Native `alert()` dialogs block the main browser thread and feel unpolished in a premium dark glassmorphism experience. Utilizing CSS/JS toast notifications is significantly more elegant, matching standard mobile-first application patterns. Additionally, dark themes require distinct, high-contrast `:focus-visible` ring colors for keyboard accessibility.
**Action:** Replace browser-blocking modal alerts with interactive toast elements and include detailed `aria-label` tags and outline-offset styling for all header/action icon buttons.
