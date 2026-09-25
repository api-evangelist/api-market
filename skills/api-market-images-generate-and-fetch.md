---
name: api-market-images-generate-and-fetch
description: Generate an image and then retrieve the result using the Images API.
api: openapi/_ae-authored/api-market-openapi-generated.yml
operations:
- post_images_generate
- get_images_result
generated: '2026-09-25'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/_ae-authored/api-market-openapi-generated.yml ; every operationId checked against the contract
---

# api-market-images-generate-and-fetch

Generate an image and then retrieve the result using the Images API.

## Steps

1. 1. Call `post_images_generate` with the required header `x-api-market-key`.
2. 2. Call `get_images_result` with the required header `x-api-market-key`.

## Rules

- Include the API key in the `x-api-market-key` header for all requests.
