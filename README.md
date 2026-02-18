# Claude Code Plugins

Collection of skills for quick integration into frontend projects (mobile + web).

## Structure

```
shared/                  # Shared between mobile & web
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
│   ├── reanimated.md
│   └── skia.md
├── components/
│   └── lists.md
├── navigation/
│   └── react-navigation.md
└── styling/
    └── pixel-precision.md

web/                     # Web (Next.js) only
├── agent-web-developer.md
├── animations/
│   └── gsap.md
├── routing/
│   └── nextjs-routing.md
└── styling/
    └── tailwind.md
```

## Usage

Each skill is an `.md` file with instructions for Claude Code.
Copy into `.claude/skills/` in the target project.

```bash
# Add a specific skill
cp mobile/animations/reanimated.md ~/my-app/.claude/skills/

# Add all shared skills
cp shared/**/*.md ~/my-app/.claude/skills/

# Add all mobile skills (shared + mobile)
cp shared/**/*.md mobile/**/*.md ~/my-app/.claude/skills/

# Add all web skills (shared + web)
cp shared/**/*.md web/**/*.md ~/my-app/.claude/skills/
```
