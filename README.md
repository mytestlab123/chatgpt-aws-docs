# ChatGPT AWS Docs

Shareable learning notes for AWS, MCP-assisted operations, GitHub-based delivery, and documentation hosting.

## Site

The repository is prepared for Material for MkDocs and GitHub Pages.

Expected Pages address after Pages is enabled:

`https://mytestlab123.github.io/chatgpt-aws-docs/`

## What belongs here

Only selected learning material intended for sharing. The implementation lab remains separate.

Current guides:

- AWS control paths: fast live work vs deterministic delivery
- Static documentation hosting: GitHub Pages, AWS S3 + CloudFront, and Cloudflare Pages
- Cloudflare Pages + Access experiment notes
- Two-repository documentation publishing model

## Local build

```bash
pip install -r requirements-docs.txt
mkdocs build --strict
mkdocs serve
```

## Publishing

`.github/workflows/docs-pages.yml` builds the site and deploys it through GitHub Pages after Pages is configured to use GitHub Actions.

See `docs/PUBLISHING_MODEL.md` for the source-repository separation model.
