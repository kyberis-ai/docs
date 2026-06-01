# Contributing

Keep this documentation focused on helping developers and agents use Kyberis safely and effectively.

## Local workflow

```bash
mint dev
mint broken-links
```

If `mint` is not installed:

```bash
npm i -g mint
```

## Writing standards

- Use active voice and second person.
- Keep sentences concise.
- Use sentence case for headings.
- Bold UI labels.
- Use code formatting for commands, paths, field names, scopes, and endpoint paths.
- Preserve exact API field names from `api-reference/openapi.json`.

## API docs

Endpoint pages in `api-reference/endpoint/` should reference operations from `api-reference/openapi.json` with the `openapi` frontmatter key.

When the OpenAPI spec changes, verify:

- every operation has a page
- every page references a real operation
- `docs.json` navigation includes the relevant pages

## Security

Never commit API keys, bearer tokens, connect tokens, MCP credentials, customer data, or live investigation output containing sensitive indicators unless explicitly approved and sanitized.
