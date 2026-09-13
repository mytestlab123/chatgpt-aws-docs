# Documentation Publishing Model

This repository contains selected public learning material from a separate private implementation repository.

## Two-repository model

```text
PRIVATE
mytestlab123/chatgpt-aws
        |
        | review + sanitize + allowlist
        v
PUBLIC
mytestlab123/chatgpt-aws-docs
        |
        | Material for MkDocs + GitHub Actions
        v
GitHub Pages
https://mytestlab123.github.io/chatgpt-aws-docs/
```

The private repository remains the implementation/evidence source of truth. This public repository contains only intentionally selected learning material.

## Recommended workflow

Phase 1: review and copy approved learning documents manually.

Phase 2: automate private-to-public publication with a narrowly scoped GitHub identity that can update only this repository. Keep an explicit publication allowlist; do not mirror the private repository wholesale.

## Repository creation lesson

For a dedicated documentation-only repository, **create an empty repository unless the template contracts are intentionally required**.

A starter template is usable, but it introduces project files such as `CONTEXT.md`, `SPEC.md`, `ENV.md`, and `INIT.md` that then need to be initialized or removed. For a pure publishing surface, an empty repository is usually the cleaner starting point.

When asking someone to create a repository, state explicitly which of these is intended:

```text
Option A: create EMPTY repository
Option B: create from <named template>
```

Do not leave that choice implicit.

## Verified deployment

The first main deployment initially failed because GitHub Pages had not yet been enabled for the repository. After setting **Settings -> Pages -> Source -> GitHub Actions**, the same deployment succeeded and GitHub reported:

`https://mytestlab123.github.io/chatgpt-aws-docs/`

This is a useful troubleshooting rule: a successful MkDocs build and Pages artifact upload do not prove that the repository's Pages control-plane setting is enabled.
