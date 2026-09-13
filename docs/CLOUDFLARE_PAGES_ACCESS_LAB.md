# Cloudflare Pages + Access Lab

## Goal

Test a small documentation site hosted on Cloudflare Pages and protected by Cloudflare Access.

```text
GitHub -> Cloudflare Pages -> Access -> reader
```

## ChatGPT MCP status

OAuth for the Cloudflare MCP connection completed successfully, but the current ChatGPT session has not yet exposed callable Cloudflare actions. The live Pages + Access creation test therefore remains pending.

## Planned proof

1. Read account and Pages inventory.
2. Create a small Pages project.
3. Deploy one static page.
4. Add an Access rule for the selected test identity.
5. Confirm an unauthenticated browser is challenged.
6. Confirm the authorized browser can open the page.
7. Record the result and cleanup steps.

## Learning

A connected account and usable MCP actions are separate states. OAuth may succeed before the client exposes the server tools required for live actions.

Do not record this lab as complete until the actual Pages and Access checks pass.
