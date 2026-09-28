# charly-build

The `charly-build` family — the image-build and authoring command skills.

The `charly-build` candy is a **concept candy**: it ships no install content and
owns the `build` family of `skill:` entities that document charly's
image-building and project-authoring surface — `build`, `generate`, `list`,
`validate`, `migrate`, `new`, `merge`, `inspect`, `pull`, `load`, `reconcile`,
`secrets`, `settings`, `docs`, and `charly-mcp-cmd`. `candy/plugin-marketplace`
regenerates the standalone [opencharly/marketplace](https://github.com/opencharly/marketplace)
corpus from these entities, so the skills are authored here and projected there.

## What it provides

| Property | Value |
|---|---|
| Layer / candy | `charly-build` (concept candy) |
| Install content | none — a `true` no-op `plan:` |
| Owns | 15 `skill:` entities in the `build` family |
| Projected to | `marketplace/build/skills/` |
| Service / port | none |

## How to use it

This repo is consumed as a **skill source**, not as an image layer. Edit the
`skill:` entities in `charly.yml`; the marketplace regeneration projects them
into `/charly-build:*` pages.

To reference the repo directly, compose it in a box. A box is a `candy:` node
that carries the box's `base:` image and a nested `candy:` list of layer refs
(the nested `candy:` is the composition list; the outer `candy:` is the box
body):

```yaml
my-box:
  candy:                  # the box body (an IMAGE is a `candy:` node carrying `base:`)
    base: fedora          # the box's base image
    candy:                # the box's composition list
      - '@github.com/opencharly/layer-charly-build:v2026.271.1957'
```

## Layout

- `charly.yml` — the `charly-build:` concept candy entity plus 15 `skill:`
  entities (`build`, `generate`, `list`, `validate`, `migrate`, `new`, `merge`,
  `inspect`, `pull`, `load`, `reconcile`, `secrets`, `settings`, `docs`,
  `charly-mcp-cmd`).
- `.github/workflows/tag-on-merge.yml` — CalVer tag + `CHANGELOG/` on merge.
- `README.md` — this user overview.

## Related

- Owning skill: `/charly-build:build`
- Authoring reference: `/charly-image:layer`
- [`opencharly/marketplace`](https://github.com/opencharly/marketplace) — the projected corpus
- [`opencharly/charly`](https://github.com/opencharly/charly) — the charly CLI and image builder
- [`opencharly/opencharly`](https://github.com/opencharly/opencharly) — the umbrella
