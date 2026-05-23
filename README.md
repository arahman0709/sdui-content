# SDUI Content

Static SDUI widget-tree payloads, design tokens, and reusable partials, served via GitHub Pages.

## URL Contract

```
https://arahman0709.github.io/sdui-content/v1/screens/<id>.json
https://arahman0709.github.io/sdui-content/v1/tokens/<tier>.json
https://arahman0709.github.io/sdui-content/v1/partials/<id>.json
```

`<id>` and `<tier>` are kebab-case slugs.

## Source of Truth

The canonical fixtures live in the (private) `design-system` repo at
`app-catalog/src/main/assets/v1/`. The files in **this** repo are the
published mirror. Updates are pushed manually when payloads change.

`PayloadSourceContractTest` (in the private repo) catches drift between the
two trees.

## Why a Separate Repo

The `design-system` repo is private. GitHub Pages on a private repo requires
a paid plan; hosting from this public, content-only repo keeps the source
code private while making widget payloads freely fetchable.
