# `OSINT Framework`

<div align="center">
  <img src="https://raw.githubusercontent.com/digital-clouds/osint/main/docs/images/osint-framework.png" alt="osint-framework" />
</div>
<hr />
<p align="center">
  <a href="https://github.com/digital-clouds/osint/actions/workflows/lychee.yml">
    <img src="https://github.com/digital-clouds/osint/actions/workflows/lychee.yml/badge.svg" alt="Lychee Check Links" />
  </a>
  <a href="https://github.com/digital-clouds/osint/actions/workflows/cloudflare-pages.yml">
    <img src="https://github.com/digital-clouds/osint/actions/workflows/cloudflare-pages.yml/badge.svg" alt="Deployment" />
  </a>
</p>

```sh
      # We trust you have received the usual lecture from the local System
      # Administrator. It usually boils down to these three things:

          #1) Respect the privacy of others.
          #2) Think before you type.
          #3) With great power comes great responsibility.
```

## Branching Strategy

- **`main`**: Production branch. Contains stable, released code.
  - _Rules_: No direct commits. Pull requests only from `next`.
- **`next`**: Development branch. Integration for new features and bug fixes.
  - _Rules_: No direct commits for major features. Pull requests from `feature-*` or `bug-*` branches.

## Development

- [Propose](https://github.com/digital-clouds/osint/issues/new) new resources via GitHub issues.
- The primary dataset is located at [`/public/arf.json`](/public/arf.json).
  - [Autochecked URLs](https://github.com/digital-clouds/osint/issues/49) are continuously verified; broken or dead links need to be removed, adjusted, or fixed.
  - Known working URLs that respond atypically to bots are ignored in [`.github/lychee.toml`](/.github/lychee.toml) to prevent false positives.
- The project is built using **Vite**, **D3 v7**, and **Vanilla JavaScript** (ESM).
- Dependencies: [Node.js](https://nodejs.org/) (>=22), [pnpm](https://pnpm.io/installation) (>=10).

### Local Setup

Clone and install dependencies:

```shell
git clone https://github.com/digital-clouds/osint
cd osint
pnpm install
```

Start the Vite development server:

```shell
pnpm dev
```

> The server will typically start at `http://localhost:5173`. Open this URL in your browser to view the framework.

### Linting and Formatting

This project uses [Trunk](https://trunk.io/) to manage linting and formatting.

```shell
# Format files
pnpm fmt

# Run all linters and checks
pnpm check
```

> Run `pnpm exec trunk check --help` to see available options.

### Testing

The project uses the native Node.js test runner (`node:test`).

```shell
# Run tests
pnpm test

# Run tests with coverage
pnpm test:coverage
```

### Build for Production

```shell
pnpm build
pnpm preview
```

> This generates a `dist/` directory optimized for deployment.
