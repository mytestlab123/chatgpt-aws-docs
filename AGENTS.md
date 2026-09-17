# AGENTS.md

## Repository Role

This repository is a **legacy rollback/historical documentation path** for ChatGPT AWS learning material. The preferred active documentation architecture now lives with the public source repository `mytestlab123/chatgpt-aws` and its same-repo GitHub Pages site.

Preserve this repository and its published site until a separate archive/deletion decision. Do not treat legacy status as cleanup authority.

## Bootstrap / Recovery Order

Use this order for cold start, recovery, materially changed governing context, or stale/incomplete/contradictory state. For warm continuation, use the named Issue/PR, latest relevant authorized delta, and current HEAD; do not reread the full context set on every handoff.

1. `AGENTS.md`
2. `CONTEXT.md`
3. `INIT.md` only when repository initialization is incomplete
4. `CHATGPT.md` when ChatGPT/Codex/GitHub collaboration or connector safety matters
5. `ENV.md` when runtime, hosting, or tool facts matter
6. `SPEC.md` before publication-model changes, deployment, cleanup, or trusted-contract changes

## Rules

- Follow KISS: optimize for one useful outcome, not the smallest possible task.
- Preserve existing work. Do not revert unrelated changes or use destructive Git actions without authority.
- Keep durable code, decisions, and reports in Git. Never commit secrets, credentials, authentication state, or copied private implementation evidence.
- Keep `CONTEXT.md` current-only and update it when repository role, active Issue/PR, blocker, or next action materially changes.
- Preserve this repository's current Pages site/content as rollback/history unless a separately authorized migration/archive milestone changes that role.
- Do not create new duplicated public content here when the same learning belongs in the preferred `mytestlab123/chatgpt-aws` documentation path.
- `SPEC.md` remains the repository execution contract for any future change.
- Prefer one cohesive PR with related changes over micro-PRs.
- Before cross-repo mutation, apply the repository-binding guard in `CHATGPT.md`.

## Global Guidance

Agent OS is reusable guidance, never automatic project authority. Current user instruction plus this repository's own rules, owning Issue/PR, and current context take precedence.
