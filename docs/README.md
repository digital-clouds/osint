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

```sh
      # We trust you have received the usual lecture from the local System
      # Administrator. It usually boils down to these three things:

          #1) Respect the privacy of others.
          #2) Think before you type.
          #3) With great power comes great responsibility.
```

## Development

- [Propose](https://github.com/digital-clouds/osint/issues/new) the resourses
- Links located at: [/public/arf.json](/public/arf.json)
  - [autochecked URL's](https://github.com/digital-clouds/osint/issues/49) are broken/dead and need to be removed/adjusted/fixed.
  - verified/working URL's, but [ignored](https://github.com/digital-clouds/osint/blob/main/.lycheeignore) from checking, because of it's specefic behaviour/response.
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
