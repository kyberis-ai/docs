# Kyberis Developer Portal

This repository contains the Mintlify documentation site for Kyberis developer documentation.

## Local preview

Install the Mintlify CLI and run the site locally:

```bash
npm i -g mint
mint dev
```

Check links before publishing:

```bash
mint broken-links
```

## Structure

- `index.mdx`: portal overview
- `quickstart.mdx`: first API calls
- `development.mdx`: authentication and request context
- `install/`: skill, MCP, and agent setup guides
- `guides/`: threat investigation workflows
- `responses/`: response interpretation guides
- `api-reference/`: OpenAPI-backed endpoint reference
- `docs.json`: Mintlify navigation and site configuration

## Source of truth

The API reference is generated from `api-reference/openapi.json`. Product workflow guidance should stay aligned with the Kyberis application repository and its active assistant-context docs.
