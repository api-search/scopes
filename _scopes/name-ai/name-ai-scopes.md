---
api_specs:
- filename: name-ai-batch-api-openapi.yml
  format: yaml
  label: Name.ai Batch API
  slug: name-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-batch-api-openapi.yml
- filename: name-ai-domain-api-openapi.yml
  format: yaml
  label: Name.ai Domain API
  slug: name-ai-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-domain-api-openapi.yml
- filename: name-ai-domains-api-openapi.yml
  format: yaml
  label: Name.ai Domains API
  slug: name-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-domains-api-openapi.yml
- filename: name-ai-market-api-openapi.yml
  format: yaml
  label: Name.ai Market API
  slug: name-ai-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-market-api-openapi.yml
- filename: name-ai-pricing-api-openapi.yml
  format: yaml
  label: Name.ai Pricing API
  slug: name-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-pricing-api-openapi.yml
- filename: name-ai-tlds-api-openapi.yml
  format: yaml
  label: Name.ai Tlds API
  slug: name-ai-tlds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-tlds-api-openapi.yml
- filename: name-ai-tools-api-openapi.yml
  format: yaml
  label: Name.ai Tools API
  slug: name-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/name-ai/openapi/name-ai-tools-api-openapi.yml
authorization_urls:
- https://name.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Name.ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Name.ai publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Name.ai API on a user''s behalf.


  Tokens are issued from https://name.ai/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Name.ai
provider_slug: name-ai
schemes:
- description: Optional — only /api/domain/search reads it, and only to unmask aftermarket prices. Every endpoint in this spec works with no auth at all. See /AUTH.md for the full flow (RFC 7591 dynamic client registration, PKCE required, no client secret).
  flows:
  - authorizationUrl: https://name.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://name.ai/api/oauth/token
  name: oauth2
  source: openapi/name-ai-openapi.json
scope_count: 1
scope_names:
- pricing:read
scopes:
- description: See real marketplace/aftermarket prices instead of the signed-out placeholder.
  flows:
  - authorizationCode
  scope: pricing:read
slug: name-ai-scopes
source_filename: name-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/name-ai-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/name-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://name.ai/oauth/authorize\n    tokenUrl: https://name.ai/api/oauth/token\n  description: Optional — only /api/domain/search reads it, and only to unmask aftermarket prices.\n    Every endpoint in this spec works with no auth at all. See /AUTH.md for the full flow (RFC\n    7591 dynamic client registration, PKCE required, no client secret).\nscopes:\n- scope: pricing:read\n  description: See real marketplace/aftermarket prices instead of the signed-out placeholder.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/name-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/name-ai/scopes/name-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Domain
- Marketplace
- Software-as-a-Service
token_bound: false
token_urls:
- https://name.ai/api/oauth/token
---
