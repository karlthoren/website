# karlthoren.de

Source repository for my personal website at **karlthoren.de**.

The site is intended as a personal home on the web for writing, technology, experiments and other projects that are interesting enough to explore.

## Purpose

This project has two primary goals:

1. Build and maintain a personal website.
2. Learn web development autodidactically by building a real project instead of working through isolated exercises.

The codebase is therefore intentionally kept understandable and relatively simple.

New technologies should be introduced when they solve an actual problem or provide a useful learning opportunity, not merely because they are common in modern web development.

The goal is not only to make things work, but to understand how and why they work.

## Current Stack

The website currently uses:

- HTML
- CSS
- Vanilla JavaScript
- Git
- GitHub
- GitHub Pages
- Hetzner DNS

There is currently:

- no frontend framework
- no backend
- no database
- no build system
- no package manager

These may be introduced later if the project develops a genuine need for them or if they provide a useful next step in the learning process.

## Project Structure

```text
/
├── index.html      Main landing page
├── global.css      Shared site-wide styling
├── script.js       Shared frontend behaviour
├── assets/         Images and other static assets
├── ignored/        Local files excluded from Git
├── .gitignore      Git ignore rules
├── README.md       Project overview
├── AGENTS.md       Instructions and context for AI coding assistants
└── DESIGN.md       Visual language and design principles
```

The structure is intentionally simple and is expected to evolve as the website grows.

## Development Principles

The project should remain:

- understandable
- maintainable
- lightweight
- standards-based
- responsive
- accessible where reasonably possible
- free of unnecessary dependencies and abstractions

Readable code is preferred over clever code.

Complexity should be added deliberately rather than pre-emptively.

Because learning is one of the main goals, important technical decisions should remain understandable instead of being hidden behind tools, frameworks or abstractions without a clear reason.

Whenever possible, new concepts should be introduced incrementally so that their purpose and effects can be understood in the context of the existing project.

## Design

The current preferred visual direction is **fantasy nerdery through the lens of a gentleman scholar.**.

The detailed visual language, design goals, stylistic principles and things to avoid are documented in `DESIGN.md`.

Site-wide styling belongs primarily in `global.css`.

The design may evolve over time, but changes should aim to preserve a coherent visual identity rather than simply follow current web design trends.

## AI-Assisted Development

AI tools are used as coding and learning partners throughout the project.

They may assist with:

- explaining technical concepts
- proposing implementations
- reviewing code
- debugging
- exploring alternatives
- improving design
- discussing architecture
- identifying potential problems

The purpose of AI assistance is not only to produce working code.

Where practical, proposed changes should also be understandable, explainable and useful for learning.

Repository-specific instructions and context for AI coding assistants are documented in `AGENTS.md`.

## Local Development

The website is currently static and does not require a dedicated application server for basic local development.

A typical workflow is:

1. Edit the files locally.
2. Test the website in a browser.
3. Review the changes with Git.
4. Commit the changes locally.
5. Push the commits to GitHub.
6. Let GitHub Pages publish the updated site.

## Deployment

The `main` branch is the source for the public GitHub Pages deployment.

The current deployment flow is:

```text
Local files
    ↓
Git commit
    ↓
Git push
    ↓
GitHub repository
    ↓
GitHub Pages deployment
    ↓
GitHub Pages hosting
    ↓
karlthoren.de
```

GitHub Pages hosts and serves the static website.

The primary public domain is:

**karlthoren.de**

DNS for the domain is managed through Hetzner.

The repository contains a `CNAME` file used by GitHub Pages for the custom domain configuration. It should not be removed or changed unintentionally.

## Project Philosophy

This repository is both a real website and a learning environment.

It is deliberately allowed to evolve.

The project does not aim to start with a theoretically perfect architecture. Instead, structure and technology should grow alongside actual requirements and increasing understanding.

A useful rule of thumb is:

> Prefer the simplest solution that solves the current problem while leaving room to learn and evolve.

## Status

The website is an ongoing personal project.

Its content, structure, design and technology will continue to change as new ideas, requirements and learning goals emerge.