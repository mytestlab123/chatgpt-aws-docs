# Specification

Status: ACTIVE
Context: PERSONAL
Environment: PUBLIC-DOCS

## Objective

Publish sanitized, reusable AWS/MCP/GitHub learning material from a separate private implementation repository without exposing private implementation details.

## Outcome

A public Material for MkDocs site deployed through GitHub Actions and GitHub Pages at:

`https://mytestlab123.github.io/chatgpt-aws-docs/`

## Authorized

- Maintain documentation, MkDocs configuration, and Pages workflows in this repository.
- Publish only content intentionally reviewed for public sharing.
- Create issues/PRs and merge routine documentation changes when validation passes.

## MUST

- Keep the private implementation repository separate.
- Use an explicit allowlist for any future automated publication.
- Run `mkdocs build --strict` before publication.
- Keep the public site reproducible from this repository.

## MUST NOT

- Mirror the private source repository wholesale.
- Publish secrets, credentials, tokens, authentication state, private account identifiers, or sensitive raw evidence.
- Give the public repository credentials that can broadly read the private source repository.

## Verification

- `mkdocs build --strict` passes.
- GitHub Pages artifact upload passes.
- GitHub Pages deployment reports success.
- Deployment environment URL is `https://mytestlab123.github.io/chatgpt-aws-docs/`.

## Acceptance

The public documentation repository is initialized, the site deploys successfully, and the two-repository publishing model is documented.
