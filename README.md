# Claude Code Plugins

Collection of skills for quick integration into frontend projects (mobile + web).

## Structure

```
shared/                  # Shared between mobile & web
├── shared.md            # Single import for all shared guidelines
├── components/
│   ├── component-architecture.md
│   └── performance.md
├── hooks/
│   └── hooks.md
└── utils/
    ├── code-style.md
    ├── type-safety.md
    └── project-structure.md

mobile/                  # React Native (Expo) only
├── agent-mobile-developer.md
├── animations/
│   ├── reanimated/SKILL.md
│   └── skia/SKILL.md
├── components/
│   └── lists/SKILL.md
├── navigation/
│   └── react-navigation/SKILL.md
└── styling/
    └── native-feel/SKILL.md

web/                     # Web (Next.js) only
├── agent-web-developer.md
├── animations/
│   └── gsap/SKILL.md
├── navigation/
│   └── nextjs-routing/SKILL.md
└── styling/
    └── tailwind/SKILL.md
```

## Usage

Reference skills in your project's `CLAUDE.md` using `@import` syntax.

```md
# CLAUDE.md

@shared/shared.md
@mobile/agent-mobile-developer.md
```

`shared/shared.md` imports all shared guidelines (code style, type safety, project structure, component architecture, performance, hooks) as a single file.
