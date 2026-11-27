---
api_specs:
- filename: createprints-ai-account-api-openapi.yml
  format: yaml
  label: Create Prints Account API
  slug: createprints-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-account-api-openapi.yml
- filename: createprints-ai-artwork-api-openapi.yml
  format: yaml
  label: Create Prints Artwork API
  slug: createprints-ai-artwork-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-artwork-api-openapi.yml
- filename: createprints-ai-checkout-api-openapi.yml
  format: yaml
  label: Create Prints Checkout API
  slug: createprints-ai-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-checkout-api-openapi.yml
- filename: createprints-ai-orders-api-openapi.yml
  format: yaml
  label: Create Prints Orders API
  slug: createprints-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-orders-api-openapi.yml
- filename: createprints-ai-product-discovery-api-openapi.yml
  format: yaml
  label: Create Prints Product discovery API
  slug: createprints-ai-product-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createprints-ai/openapi/createprints-ai-product-discovery-api-openapi.yml
authorization_urls:
- https://api.createprints.ai/api/oauth/authorize
description: ''
docs: https://www.createprints.ai/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Create Prints Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Create Prints publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Create Prints API on a user''s behalf.


  Tokens are issued from https://api.createprints.ai/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Create Prints
provider_slug: createprints-ai
schemes:
- description: Create Prints OAuth 2.0 authorization-code flow with PKCE for MCP and agent clients.
  flows:
  - authorizationUrl: https://api.createprints.ai/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.createprints.ai/api/oauth/token
  name: oauth2
  source: openapi/createprints-ai-openapi.yml
scope_count: 7
scope_names:
- artwork:create
- artwork:read
- checkout:create
- checkout:read
- orders:read
- print_options:read
- fulfillment:retry
scopes:
- description: Create, import, and retry artwork jobs.
  flows:
  - authorizationCode
  scope: artwork:create
- description: Read and list artwork jobs.
  flows:
  - authorizationCode
  scope: artwork:read
- description: Create checkout sessions and retry production submission.
  flows:
  - authorizationCode
  scope: checkout:create
- description: Read checkout, fulfilment, and shipment status.
  flows:
  - authorizationCode
  scope: checkout:read
- description: Read orders and, on the current credit endpoint, generation credits.
  flows:
  - authorizationCode
  scope: orders:read
- description: Read print variants, frames, prices, and postage estimates.
  flows:
  - authorizationCode
  scope: print_options:read
- description: Retry stuck order fulfilment
  flows:
  - authorizationCode
  scope: fulfillment:retry
slug: createprints-ai-scopes
source_filename: createprints-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.createprints.ai/auth.md\nschemes:\n- name: oauth2\n  source: openapi/createprints-ai-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.createprints.ai/api/oauth/authorize\n    tokenUrl: https://api.createprints.ai/api/oauth/token\n  description: Create Prints OAuth 2.0 authorization-code flow with PKCE for MCP and agent clients.\nscopes:\n- scope: artwork:create\n  description: Create, import, and retry artwork jobs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/createprints-ai-openapi.yml\n  - https://www.createprints.ai/auth.md\n  docs_description: Generate artwork using the user's credits\n- scope: artwork:read\n  description: Read and list artwork jobs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/createprints-ai-openapi.yml\n  - https://www.createprints.ai/auth.md\n  docs_description: View the user's generated artwork\n- scope: checkout:create\n \
  \ description: Create checkout sessions and retry production submission.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/createprints-ai-openapi.yml\n  - https://www.createprints.ai/auth.md\n  docs_description: Create print purchase checkouts\n- scope: checkout:read\n  description: Read checkout, fulfilment, and shipment status.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/createprints-ai-openapi.yml\n  - https://www.createprints.ai/auth.md\n  docs_description: View checkout/order status\n- scope: orders:read\n  description: Read orders and, on the current credit endpoint, generation credits.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/createprints-ai-openapi.yml\n  - https://www.createprints.ai/auth.md\n  docs_description: View the user's order status\n- scope: print_options:read\n  description: Read print variants, frames, prices, and postage estimates.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/createprints-ai-openapi.yml\n  - https://www.createprints.ai/auth.md\n\
  \  docs_description: View available print sizes and options\n- scope: fulfillment:retry\n  description: Retry stuck order fulfilment\n  flows:\n  - authorizationCode\n  sources:\n  - https://www.createprints.ai/auth.md\n  note: Listed in auth.md and the MCP protected-resource metadata example; not declared in the OpenAPI oauth2 scopes\n    (the spec describes retryAgentFulfilment under checkout:create).\ndocs: https://www.createprints.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/createprints-ai/scopes/createprints-ai-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- AI Art
- Generative AI
- Art Prints
- Print on Demand
- E-Commerce
- Interior Design
- MCP
token_bound: false
token_urls:
- https://api.createprints.ai/api/oauth/token
---
