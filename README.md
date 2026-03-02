# Claude Code Plugins

Collection of React & React Native TypeScript skills for Claude Code. Quick integration into frontend projects (mobile | web).

## Structure

```
├── agents/                  # Custom agents
│   ├── mobile-developer     # React Native + Expo
│   └── web-developer        # Next.js + React
├── shared/                  # Shared skills (both platforms)
│   ├── components/
│   │   ├── component-architecture
│   │   └── performance
│   ├── hooks/
│   └── utils/
│       ├── code-style
│       ├── project-structure
│       └── type-safety
├── mobile/                  # Mobile-only skills
│   ├── animations/
│   │   ├── reanimated
│   │   └── skia
│   ├── components/lists
│   ├── navigation/react-navigation
│   └── styling/native-feel
└── web/                     # Web-only skills
    ├── animations/gsap
    ├── navigation/nextjs-routing
    └── styling/tailwind
```

## Skills

Each skill lives in its own folder with a `SKILL.md` file containing frontmatter and rules:

```md
---
name: skill-name
description: What the skill does and when to use it.
---

# Skill Title

- Rule one
- Rule two
```

### Shared

| Skill | Description |
|---|---|
| `component-architecture` | Component structure, prop typing, responsibility separation, ref handling |
| `performance` | Rendering performance — memoization, stable references, re-render prevention |
| `hooks` | Custom hooks — naming, logic extraction, view/logic separation |
| `code-style` | Readability, naming conventions, conditional classNames, exports |
| `project-structure` | Folder organization, API boundaries, re-exports |
| `type-safety` | Strict TypeScript — type over interface, no any, no enum, narrow types |

### Mobile

| Skill | Description |
|---|---|
| `reanimated` | Reanimated shared values, animated styles, layout animations, worklets |
| `skia` | React Native Skia — shaders, charts, complex drawing, GPU effects |
| `lists` | FlashList, stable renderItem, extracted item components, naming patterns |
| `native-feel` | UX precision, iOS/Android platform conventions, haptics, interactions |
| `react-navigation` | Typed routes, navigator structure, deep linking, navigation actions |

### Web

| Skill | Description |
|---|---|
| `tailwind` | Utility-first Tailwind CSS, class ordering, responsive, dark mode, cn() |
| `gsap` | GSAP timelines, ScrollTrigger, React integration, cleanup patterns |
| `nextjs-routing` | App Router, layouts, server/client components, dynamic routes, metadata |

## Agents

| Agent | Model | Description |
|---|---|---|
| `mobile-developer` | Sonnet | Senior React Native + Expo engineer |
| `web-developer` | Sonnet | Senior Next.js + React engineer |

## Usage

Add selected skills to your project's `.claude/settings.json`:

```json
{
  "permissions": {
    "allow": ["skills:shared/*", "skills:mobile/*"]
  }
}
```

Or reference individual skills directly in your `CLAUDE.md`.
