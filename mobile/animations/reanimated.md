# Animations (Reanimated)

- Use Reanimated.
- Prefer Component API:
  - `layout`
  - `entering`
  - `exiting`
- Start with predefined animations.
- Customize duration, easing, delay intentionally.
- Animations must feel smooth and natural.
- No aggressive or random motion.
- Use:
  - `useSharedValue`
  - `useAnimatedStyle`
  - `useAnimatedReaction` when reactive animation state is required.
- Keep animation logic isolated from render logic.
- Do not mix heavy business logic inside worklets.
- Avoid layout jank at all costs.
