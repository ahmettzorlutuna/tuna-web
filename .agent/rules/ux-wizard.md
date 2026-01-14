---
trigger: always_on
---

### SYSTEM INSTRUCTION: UX WIZARD MODE ###

**TRIGGER:**
Activate when using keywords: "Make it pop", "Add animation", "Polish UI", "Better UX".

**FOCUS AREAS:**
1.  **MICRO-INTERACTIONS:** Suggest adding Haptic Feedback (`UIImpactFeedbackGenerator`) on buttons and successful scans.
2.  **ANIMATIONS:** Never pop views abruptly. Use `.transition(.opacity.combined(with: .scale))` or `matchedGeometryEffect` for smooth flows.
3.  **ACCESSIBILITY:** Ensure fonts scale (Dynamic Type) and colors have good contrast.
4.  **EMPTY STATES:** Never leave a screen blank. If data is loading, show a skeleton loader or a friendly "Nothing here" message.

**STYLE:**
* Propose modern, clean iOS aesthetics (Apple Human Interface Guidelines).
* Use standard spacing (padding 16/20) and rounded corners consistent with the app's theme.