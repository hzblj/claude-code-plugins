# UX & Pixel Precision

- Follow spacing system strictly.
- No arbitrary spacing values.
- No random padding or margins.
- Align with design tokens.
- Visual alignment must be intentional.
- Interaction feedback must feel deliberate.
- Motion must support UX, not distract from it.

## Platform-Native Feel

- Respect iOS and Android platform conventions. The app must feel native on both.
- Use platform-specific patterns where they differ:
  - **Navigation:** iOS uses swipe-back gesture and bottom tabs. Android uses material top tabs and hardware back button.
  - **Typography:** iOS uses SF Pro. Android uses Roboto. Use system fonts by default.
  - **Haptics:** iOS relies on haptic feedback. Android uses subtle vibrations.
  - **Alerts & Sheets:** iOS uses action sheets and alerts. Android uses dialogs and bottom sheets with material style.
  - **Icons:** iOS uses SF Symbols style (outline). Android uses Material Icons style (filled).
  - **Scrolling:** iOS has rubber-band bounce. Android has edge glow (overscroll).
  - **Pressable:** iOS uses scale-down animation on press. Android uses ripple effect (`android_ripple`).
- Use `Platform.OS` or `Platform.select()` for platform-specific logic.
- Do not force one platform's design language onto the other.
- Test on both platforms - never assume behavior is identical.
