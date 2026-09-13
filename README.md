# ChatGPT AWS Docs

Shareable learning notes for AWS, MCP-assisted operations, GitHub-based delivery, and documentation hosting.

## Live site

**https://mytestlab123.github.io/chatgpt-aws-docs/**

The site is built with Material for MkDocs and deployed by GitHub Actions to GitHub Pages.

## What belongs here

Only selected learning material intended for public sharing. The implementation lab remains separate in the private `mytestlab123/chatgpt-aws` repository.

Current guides:

- AWS control paths: fast live work vs deterministic delivery
- Static documentation hosting: GitHub Pages, AWS S3 + CloudFront, and private sharing options
- Cloudflare Pages + Access experiment notes
- Two-repository documentation publishing model

## Local build

```bash
pip install -r requirements-docs.txt
mkdocs build --strict
mkdocs serve
```

## Publishing

`.github/workflows/docs-pages.yml` validates documentation on pull requests and deploys `main` through GitHub Pages.

See `docs/PUBLISHING_MODEL.md` for the source-repository separation model and the repository-creation lesson.
