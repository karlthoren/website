# AGENTS.md

Instructions and project context for AI coding assistants working on **karlthoren.de**.

## Project Context

This repository contains a personal website and an autodidactic web-development learning project.

It has two equally important purposes:

1. Build a useful and distinctive personal website.
2. Learn how web technologies work by developing a real project incrementally.

Producing working code is therefore not the only goal.

Changes should, where practical, remain understandable to the project owner and should help build technical understanding rather than hide complexity unnecessarily.

## Current Architecture

The website currently uses:

- HTML
- CSS
- Vanilla JavaScript
- Git
- GitHub
- GitHub Pages

The project currently has:

- no frontend framework
- no backend
- no database
- no package manager
- no build system

Do not introduce these merely because they are common in modern web development.

They may be introduced when they solve an actual problem or create a useful and deliberate learning opportunity.

## Current Repository Structure

```text
/
├── index.html
├── global.css
├── script.js
├── assets/
├── ignored/
├── .gitignore
├── README.md
├── AGENTS.md
├── DESIGN.md
└── CNAME
```

The structure may evolve as the site grows.

## File Responsibilities

### `index.html`

Contains the semantic structure and content of the landing page.

Prefer meaningful HTML elements such as:

- `header`
- `nav`
- `main`
- `section`
- `article`
- `footer`

Avoid unnecessary wrapper elements when semantic HTML can express the same structure clearly.

### `global.css`

Contains site-wide styling and the shared visual language.

It should remain understandable and reasonably structured.

Prefer grouping CSS into clear conceptual sections such as:

- design tokens
- base styles
- layout
- typography
- navigation
- reusable components
- page sections
- responsive rules
- accessibility

Avoid excessive specificity and unnecessary duplication.

### `script.js`

Contains shared client-side behaviour.

Keep JavaScript small and purposeful.

Prefer native browser APIs over dependencies when they reasonably solve the problem.

Do not move behaviour into JavaScript when HTML or CSS can handle it cleanly.

### `DESIGN.md`

Defines the intended visual identity.

Treat it as design direction rather than an exact immutable specification.

New visual ideas are welcome when they strengthen the intended identity.

### `README.md`

Provides the high-level project overview, architecture and development philosophy.

### `ignored/`

This directory is intentionally excluded from Git.

Do not reference its contents as part of the public website.

### `CNAME`

Required for the GitHub Pages custom domain.

Do not remove or modify it unless the custom-domain configuration is intentionally being changed.

## Development Priorities

When several solutions are possible, prefer the one that is:

1. understandable
2. standards-based
3. lightweight
4. maintainable
5. accessible
6. responsive
7. educational
8. visually coherent

Avoid adding complexity pre-emptively.

The project should grow in response to actual requirements.

## Learning-Oriented Development

The project owner is intentionally learning the technologies used in this repository.

When proposing meaningful technical changes:

- explain what is changing
- explain why it works
- identify important new concepts
- prefer incremental changes over large unexplained rewrites
- distinguish browser behaviour from server behaviour where relevant
- explain abstractions before introducing them

Do not assume that hiding complexity behind a framework is inherently helpful.

A slightly more manual implementation may be preferable if it provides useful understanding without creating unreasonable maintenance cost.

## Code Style

Prefer code that is explicit and readable.

Avoid:

- clever one-liners that reduce clarity
- unnecessary abstractions
- premature component systems
- large amounts of generated boilerplate
- unnecessary libraries
- duplicated styles
- unexplained magic numbers where meaningful variables would help

Comments should explain intent or non-obvious behaviour.

Do not comment every self-explanatory line.

## Dependencies

Do not add external dependencies without a clear reason.

Before suggesting a framework, library, package manager or build system, consider whether the same objective can reasonably be achieved with the existing stack.

If a new dependency would genuinely be useful, explain:

- what problem it solves
- what additional complexity it introduces
- what the project gains
- what the project gives up

The final decision belongs to the project owner.

## Design Direction

The visual identity is described in detail in `DESIGN.md`.

The short version is:

> Fantasy nerdery through the lens of a gentleman scholar.

The website should feel mature, distinctive, literary and slightly whimsical.

It should combine modern restraint with references to fantasy, books, research, craftsmanship and collected curiosities.

Avoid turning this into either:

- a generic corporate website
- a generic dark-mode SaaS interface
- a cyberpunk dashboard
- a medieval fantasy theme park
- a literal historical reconstruction

Fantasy elements are welcome.

Dragons, creatures, maps, symbols, books, strange objects and imaginative illustrations are all valid when treated with restraint and visual sophistication.

## Visual Implementation

Prefer:

- dark, warm backgrounds
- ivory or warm off-white typography
- bronze, brass, copper and muted gold accents
- occasional restrained secondary colors
- strong typography
- generous negative space
- subtle texture
- elegant lines and borders
- asymmetry where useful
- small illustrative details
- restrained animation

Avoid excessive use of:

- glassmorphism
- neon gradients
- glowing blobs
- generic rounded cards
- blue-grey corporate palettes
- dashboard-like UI
- decorative effects without purpose

Cards and panels are allowed when they genuinely serve the composition.

They should not become the default solution for every piece of content.

## Illustration

The visual system should leave room for minimalist whimsical illustrations.

Possible subjects include:

- dragons
- fantastical animals
- books
- swords
- strange plants
- maps
- tools
- bottles
- astronomical instruments
- mysterious artifacts
- architectural fragments
- fictional creatures
- absurd scholarly objects

Illustrations should generally feel like intentional editorial details rather than large commercial hero graphics.

They may resemble:

- ink drawings
- engravings
- marginalia
- field-guide illustrations
- bookplate art
- restrained line drawings
- stylised silhouettes

Humour and oddity are welcome.

## Responsive Design

All meaningful changes should remain usable on both desktop and mobile.

Desktop design may be more ambitious and asymmetrical.

Mobile layouts should simplify rather than merely shrink the desktop composition.

Avoid horizontal overflow.

Navigation, text and interactive elements must remain comfortably usable.

## Accessibility

Use reasonable accessibility practices from the beginning.

In particular:

- maintain sufficient text contrast
- preserve visible focus states
- use semantic HTML
- provide meaningful alternative text for informative images
- mark purely decorative images appropriately
- avoid conveying essential meaning using color alone
- respect `prefers-reduced-motion` for significant animations

Accessibility improvements should generally be preferred over purely decorative behaviour when the two conflict.

## Git and Deployment

The public site is deployed from the `main` branch through GitHub Pages.

Typical flow:

```text
local change
    ↓
review
    ↓
commit
    ↓
push to GitHub
    ↓
GitHub Pages deployment
    ↓
karlthoren.de
```

Treat changes to `main` as changes that may become public.

Do not deliberately include files from `ignored/`.

Do not expose secrets, credentials, private notes or API keys.

## Refactoring

Refactoring is welcome when it improves clarity or solves an emerging structural problem.

Do not perform large unrelated refactors while implementing a small feature.

Prefer:

> improve structure when the project actually begins to need improved structure.

If a larger refactor would be beneficial, explain it separately before making it part of an otherwise simple change.

## Future Technologies

The current simple architecture is intentional, not permanent.

Possible future additions may include:

- additional pages
- subdomains
- content stored outside HTML
- static-site generation
- APIs
- small web applications
- backend services
- databases
- frontend frameworks

None of these are forbidden.

They should be introduced because the project reaches a point where they provide clear value.

## General Rule

When uncertain, follow this principle:

> Prefer the simplest solution that solves the current problem, preserves the project's visual identity, and teaches something useful without creating unnecessary future burden.