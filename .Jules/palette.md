# Palette UX Journal - EASYPIE

This journal holds critical UX and accessibility learnings from the EASYPIE codebase.

## 2025-02-18 - Native Alerts in Mobile-First UI
**Learning:** Jarring browser native `alert()` dialogs disrupt the premium feel of dark-themed mobile-first financial interfaces. Replacing them with custom toast notifications maintains visual consistency, keeps users in the app flow, and improves task confidence.
**Action:** Always verify if a screen or app flow has custom toast mechanics, and reuse or implement inline/overlay custom alerts over native browser `alert()` methods.
