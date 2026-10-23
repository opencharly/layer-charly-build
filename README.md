# charly-build — RETIRED (archived)

> **RETIRED (archived) — this repo publishes nothing and is read-only.** All fifteen
> `build`-family skills live in the repo that holds the verb each one documents (the table
> below), the umbrella no longer pins a submodule here, and the repository is archived.
> Nothing is authored, built, deployed or consumed here. A change to a `build`-family skill
> is a change at its destination repo, in the same pull request as the verb it documents.

**This repo no longer authors a skill.** It was the `charly-build` concept candy:
a `true`-no-op `plan:` and 15 `skill:` entities, with the prose in
`.agents/skills/`. Under `AGENTS.md` Part II #5 a skill lives in the repo whose
code, plugin or config it describes — and this repo holds none of the verbs those
skills document — so all fifteen moved, byte-identically, to the repo that does:

| Skill | Now authored in |
|---|---|
| `build`, `generate`, `inspect`, `list`, `load`, `merge`, `new`, `pull`, `reconcile`, `validate` | [`opencharly/plugin-box`](https://github.com/opencharly/plugin-box) — the `command:*:box` provider |
| `migrate` | [`opencharly/plugin-migrate`](https://github.com/opencharly/plugin-migrate) |
| `docs` | [`opencharly/plugin-docs`](https://github.com/opencharly/plugin-docs) |
| `secrets` | [`opencharly/plugin-secrets`](https://github.com/opencharly/plugin-secrets) |
| `settings` | [`opencharly/plugin-settings`](https://github.com/opencharly/plugin-settings) |
| `charly-mcp-cmd` | [`opencharly/plugin-mcp`](https://github.com/opencharly/plugin-mcp) |

**The addresses did not change.** Every skill keeps its `build` family, so
`/charly-build:build` … `/charly-build:validate` still resolve — they are simply
authored where the verb is implemented. The full destination re-derivation for
both skills-only carriers is [opencharly/opencharly#611](https://github.com/opencharly/opencharly/issues/611).

## What remains here

| Property | Value |
|---|---|
| Layer / candy | `charly-build` (drained concept candy) |
| Install content | none — a `true` no-op `plan:` |
| Owns | nothing — 0 `skill:` entities |
| Service / port | none |

Do not compose, reference or edit this repo: the skills, their routing nodes and
their prose all live at the destinations above. Its retirement — the umbrella
gitlink, the `.gitmodules` stanza and the org-map row — landed under
[opencharly/opencharly#600](https://github.com/opencharly/opencharly/issues/600),
and the repository is archived.
