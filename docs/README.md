# `OSINT Framework`

<div align="center">
  <img src="https://raw.githubusercontent.com/digital-clouds/osint/main/docs/images/osint-framework.png" alt="osint-framework" />
</div>
<hr />
<p align="center">
  <a href="https://github.com/digital-clouds/osint/actions/workflows/lychee.yml">
    <img src="https://github.com/digital-clouds/osint/actions/workflows/lychee.yml/badge.svg" alt="Lychee Check Links" />
  </a>
</p>


## Development

- [Propose](https://github.com/digital-clouds/osint/issues/new) the resourses
- Links located at: [/public/arf.json](/public/arf.json)
- Dependencies: [git](https://github.com/git-guides/install-git), [pnpm](https://pnpm.io/installation)

Clone and install:

```shell
git clone https://github.com/digital-clouds/osint; cd osint
pnpm i
```

Check or lint files:

```shell
pnpm fmt
pnpm check
```

> Run: `pnpm trunk -h` to see available options.

Start server:

```shell
pnpm dev
```

Visit http://0.0.0.0:8787 or use keys to select required option:

- <kbd>b</kbd> `open a browser`
- <kbd>d</kbd> `open Devtools`
- <kbd>l</kbd> `turn on local mode`
- <kbd>c</kbd> `clear console`
- <kbd>x</kbd> `to exit`
