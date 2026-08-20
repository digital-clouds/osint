# AGENTS.md

## Repository Overview

This repository hosts the **OSINT Framework**, an interactive Open Source Intelligence reconnaissance tool built with Vanilla JavaScript (ESM), D3 v7, and Vite, deployed to Cloudflare Pages.

## Project Structure

- `index.html`: Entry point HTML
- `src/main.js`: Main application entry and D3 tree rendering logic
- `src/tree-utils.js`: Core tree manipulation helpers (collapsing, expanding, traversing)
- `src/style.css`: Stylesheet
- `public/arf.json`: Primary OSINT resources hierarchy dataset
- `public/favicon/`: Web favicons and application icons
- `test/arf.test.js`: Native Node.js tests for tree utility functions and dataset structure
- `.github/workflows/`: GitHub Actions workflows (Cloudflare Pages deploy, Lychee link checker, Trunk check)
- `.github/dependabot.yml`: Dependabot configuration with grouped updates
- `.trunk/trunk.yaml`: Trunk linter and formatter configuration

## Development Workflow & Commands

- **Install dependencies**: `pnpm install`
- **Development server**: `pnpm dev`
- **Unit testing**: `pnpm test` (or `pnpm test:coverage`)
- **Format code**: `pnpm fmt` (or `trunk fmt`)
- **Lint & security checks**: `pnpm check` (or `trunk check .`)
- **Production build**: `pnpm build`
- **Preview build**: `pnpm preview`

## Branching Conventions

- `main`: Stable production branch. Deployed automatically via Cloudflare Pages. No direct commits; pull requests only from `next`.
- `next`: Active development and integration branch. Pull requests branch off `next` (e.g., `feature-*`, `bug-*`).

## Code Standards & Verification

- Native Node.js test runner (`node:test`) is used for all unit tests.
- All code, configs, and assets must pass `trunk check .` before merging.
- Dependencies and GitHub Actions are kept up-to-date with Dependabot grouped update bundles.
