---
name: api-market-check-domain-availability
description: Check the availability of multiple domain extensions using the Domain Availability Checker API.
api: openapi/_ae-authored/api-market-openapi-generated.yml
operations:
- get_api_v1_magicapi_domainchecker_check_domains
- post_api_v1_magicapi_domainchecker_check_domains
generated: '2026-09-25'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/_ae-authored/api-market-openapi-generated.yml ; every operationId checked against the contract
---

# api-market-check-domain-availability

Check the availability of multiple domain extensions using the Domain Availability Checker API.

## Steps

1. 1. Call `get_api_v1_magicapi_domainchecker_check_domains` – no request body, include header `x-api-market-key` with your API key.
2. 2. Call `post_api_v1_magicapi_domainchecker_check_domains` – send a JSON body with the field `domains` (array of domain strings), include header `x-api-market-key`.
3. 3. Parse the response which lists each domain and its availability status.

## Rules

- Auth: Provide the API key in the request header `x-api-market-key` (apiKey scheme).
- Idempotency: The POST operation is safe to retry; it does not create persistent resources.
- Errors: The API returns standard HTTP error codes (e.g., 400 for bad request, 401 for missing/invalid API key, 429 for rate limiting).
