---
name: stainless-builds-diagnostics
description: Retrieve a specific build and list its diagnostics.
api: openapi/stainless-builds-api-openapi.yml
operations:
- getV0Builds
- getV0BuildsByBuildId
- getV0BuildsByBuildIdDiagnostics
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/stainless-builds-api-openapi.yml ; every operationId checked against the contract
---

# stainless-builds-diagnostics

Retrieve a specific build and list its diagnostics.

## Steps

1. 1. Call `getV0Builds` with optional pagination parameters (limit, offset, page number, page size, starting_after, ending_before, or custom cursor) and include the `Authorization: Bearer <token>` header.
2. 2. Call `getV0BuildsByBuildId` with the `buildId` path parameter obtained from the list and the `Authorization` header.
3. 3. Call `getV0BuildsByBuildIdDiagnostics` with the same `buildId` and the `Authorization` header; the response may contain a `data` (or `items`) array and pagination fields such as `next_cursor`, `next_cursor_id`, or a next URL.

## Rules

- Auth: Include a Bearer token in the `Authorization` header for all requests.
- Pagination: Requests may include limit, offset, page number, page size, starting_after, ending_before, or a custom cursor; responses may include a data array (or items), next_cursor, next_cursor_id, or a next URL.
