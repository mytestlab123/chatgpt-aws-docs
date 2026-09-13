# Static Documentation Hosting

## GitHub Pages

Best for the simplest GitHub-native documentation site.

Flow:

```text
GitHub -> Actions -> MkDocs -> Pages
```

## AWS S3 + CloudFront

Best when you want AWS-native infrastructure and more edge-control options.

Flow:

```text
GitHub -> Actions -> MkDocs -> S3 -> CloudFront
```

## Cloudflare Pages + Access

Best when you want a simple hosted docs site with an optional login gate.

Flow:

```text
GitHub -> Cloudflare Pages -> Access -> reader
```

## Quick choice

| Need | Choice |
|---|---|
| Simplest docs site | GitHub Pages |
| AWS-native hosting | S3 + CloudFront |
| Simple login-protected docs | Cloudflare Pages + Access |

Material for MkDocs can generate the same `site/` output for all three paths.
