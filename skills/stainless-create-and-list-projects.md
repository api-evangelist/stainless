---
name: stainless-create-and-list-projects
description: Create a new project and then list all projects.
api: openapi/stainless-projects-api-openapi.yml
operations:
- postV0Projects
- getV0Projects
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/stainless-projects-api-openapi.yml ; every operationId checked against the contract
---

# stainless-create-and-list-projects

Create a new project and then list all projects.

## Steps

1. 1. `postV0Projects` – body fields: project name and required configuration fields as defined in the contract.
2. 2. `getV0Projects` – optional query parameters: limit, offset, page number, page size, starting_after, ending_before, or custom cursor for pagination; response includes a data (or items) array and pagination cursors.

## Rules

- Auth: Include a Bearer token in the `Authorization` header (BearerAuth).
- Pagination: When listing projects, use the supported pagination parameters (limit, offset, etc.) and handle `next_cursor` or `next` URL in the response.
