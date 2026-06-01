# Documentation project instructions

## About this project

- This is the Mintlify developer portal for Kyberis.
- Pages are MDX files with YAML frontmatter.
- Configuration lives in `docs.json`.
- Run `mint dev` to preview locally.
- Run `mint broken-links` to check links.

## Product focus

Kyberis provides deterministic, evidence-backed threat intelligence workflows for machine consumers and security teams. Documentation should help readers install Kyberis in agents, authenticate safely, conduct investigations, interpret responses, and use the API reference.

## Terminology

- Use "Kyberis" for the product.
- Use "agent context" for request metadata such as `objective`, `workflow_stage`, `run_id`, and `step_id`.
- Use "evidence" for bounded support returned by Kyberis.
- Use "assessment" for deterministic decision support.
- Use "signal" for a normalized item returned by `/v2/prioritize`.
- Use "MCP" for Model Context Protocol integrations.

## Style preferences

- Use active voice and second person.
- Keep sentences concise.
- Use sentence case for headings.
- Bold UI elements.
- Use code formatting for file names, commands, paths, endpoint paths, scopes, and response fields.
- Separate facts from inference in investigation examples.
- Preserve request IDs, evidence IDs, confidence, and caveats in examples that describe agent output.

## Content boundaries

- Do not document internal admin workflows unless they are exposed in the public OpenAPI spec.
- Do not include secrets, live credentials, or unsanitized customer data.
- Treat `api-reference/openapi.json` as the endpoint contract source of truth.
- Treat active Kyberis application docs and code as product behavior source of truth when updating guides.
