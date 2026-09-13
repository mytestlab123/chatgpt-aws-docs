# Context

Status: READY

## Project Identity

- Project: `chatgpt-aws-docs`
- Primary Repository: `mytestlab123/chatgpt-aws-docs`
- Related source repository: private `mytestlab123/chatgpt-aws`
- Purpose: public, sanitized learning documentation only
- Public site: `https://mytestlab123.github.io/chatgpt-aws-docs/`

## Current Truth

- Repository is public.
- Material for MkDocs builds successfully with `mkdocs build --strict`.
- GitHub Pages is configured to deploy through GitHub Actions.
- Initial Pages deployment succeeded after Pages was enabled.
- The private implementation repository remains separate and is not mirrored wholesale.

## Active Work

- Issue: `#1` bootstrap/closeout
- Current milestone: complete the public documentation publishing surface and record the verified deployment.

## Publishing Rule

Publish only reviewed, reusable learning content. Never publish secrets, credentials, authentication state, private-only account identifiers, or raw implementation evidence that is not intended for public sharing.

## Next Action

Keep the public documentation allowlist explicit. Future automation from the private source repository should use a narrowly scoped identity that can write only to this documentation repository.
