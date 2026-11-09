---
api_specs:
- filename: adadiamonds-com-agentic-checkout-acp-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (ACP) API
  slug: adadiamonds-com-agentic-checkout-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-acp-api-openapi.yml
- filename: adadiamonds-com-agentic-checkout-hosted-link-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (hosted link) API
  slug: adadiamonds-com-agentic-checkout-hosted-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-hosted-link-api-openapi.yml
- filename: adadiamonds-com-agentic-checkout-ucp-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic checkout (UCP) API
  slug: adadiamonds-com-agentic-checkout-ucp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-checkout-ucp-api-openapi.yml
- filename: adadiamonds-com-agentic-commerce-discovery-api-openapi.yml
  format: yaml
  label: Ada Diamonds Agentic commerce discovery API
  slug: adadiamonds-com-agentic-commerce-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-agentic-commerce-discovery-api-openapi.yml
- filename: adadiamonds-com-appointments-api-openapi.yml
  format: yaml
  label: Ada Diamonds Appointments API
  slug: adadiamonds-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-appointments-api-openapi.yml
- filename: adadiamonds-com-bulk-api-openapi.yml
  format: yaml
  label: Ada Diamonds Bulk API
  slug: adadiamonds-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-bulk-api-openapi.yml
- filename: adadiamonds-com-catalog-api-openapi.yml
  format: yaml
  label: Ada Diamonds Catalog API
  slug: adadiamonds-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-catalog-api-openapi.yml
- filename: adadiamonds-com-content-api-openapi.yml
  format: yaml
  label: Ada Diamonds Content API
  slug: adadiamonds-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-content-api-openapi.yml
- filename: adadiamonds-com-discovery-api-openapi.yml
  format: yaml
  label: Ada Diamonds Discovery API
  slug: adadiamonds-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-discovery-api-openapi.yml
- filename: adadiamonds-com-mcp-api-openapi.yml
  format: yaml
  label: Ada Diamonds MCP API
  slug: adadiamonds-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-mcp-api-openapi.yml
- filename: adadiamonds-com-onboarding-api-openapi.yml
  format: yaml
  label: Ada Diamonds Onboarding API
  slug: adadiamonds-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-onboarding-api-openapi.yml
- filename: adadiamonds-com-search-api-openapi.yml
  format: yaml
  label: Ada Diamonds Search API
  slug: adadiamonds-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adadiamonds-com/openapi/adadiamonds-com-search-api-openapi.yml
authorization_urls:
- https://www.adadiamonds.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Adadiamonds Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ada Diamonds publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ada Diamonds API on a user''s behalf.


  Tokens are issued from https://www.adadiamonds.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ada Diamonds
provider_slug: adadiamonds-com
schemes:
- description: OAuth 2.1. PKCE is mandatory on the authorization code flow. Clients may self-register at /api/oauth/register (RFC 7591).
  flows:
  - authorizationUrl: https://www.adadiamonds.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.adadiamonds.com/api/oauth/token
  - flow: clientCredentials
    tokenUrl: https://www.adadiamonds.com/api/oauth/token
  name: oauth2
  source: openapi/adadiamonds-com-openapi.json
scope_count: 6
scope_names:
- appointments:write
- cart:write
- catalog:read
- content:read
- orders:read
- profile:read
scopes:
- description: Request a consultation or showroom appointment on the signed-in customer's behalf.
  flows:
  - authorizationCode
  scope: appointments:write
- description: Create and modify a shopping cart on the signed-in customer's behalf.
  flows:
  - authorizationCode
  scope: cart:write
- description: Read the public product catalog — diamonds, engagement rings, and fine jewelry, with prices and specifications.
  flows:
  - authorizationCode
  - clientCredentials
  scope: catalog:read
- description: Read published editorial content — knowledge base articles, buying guides, and showroom information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: content:read
- description: Read the signed-in customer's order history and order status.
  flows:
  - authorizationCode
  scope: orders:read
- description: Read the signed-in customer's account profile (name, email, saved preferences).
  flows:
  - authorizationCode
  scope: profile:read
slug: adadiamonds-com-scopes
source_filename: adadiamonds-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/adadiamonds-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/adadiamonds-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.adadiamonds.com/oauth/authorize\n    tokenUrl: https://www.adadiamonds.com/api/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://www.adadiamonds.com/api/oauth/token\n  description: OAuth 2.1. PKCE is mandatory on the authorization code flow. Clients may self-register\n    at /api/oauth/register (RFC 7591).\nscopes:\n- scope: appointments:write\n  description: Request a consultation or showroom appointment on the signed-in customer's behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adadiamonds-com-openapi.json\n- scope: cart:write\n  description: Create and modify a shopping cart on the signed-in customer's behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adadiamonds-com-openapi.json\n- scope: catalog:read\n\
  \  description: Read the public product catalog — diamonds, engagement rings, and fine jewelry,\n    with prices and specifications.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/adadiamonds-com-openapi.json\n- scope: content:read\n  description: Read published editorial content — knowledge base articles, buying guides, and\n    showroom information.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/adadiamonds-com-openapi.json\n- scope: orders:read\n  description: Read the signed-in customer's order history and order status.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adadiamonds-com-openapi.json\n- scope: profile:read\n  description: Read the signed-in customer's account profile (name, email, saved preferences).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adadiamonds-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/adadiamonds-com/scopes/adadiamonds-com-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Jewelry
- Lab Diamonds
- Engagement Rings
- New York
- E-Commerce
token_bound: false
token_urls:
- https://www.adadiamonds.com/api/oauth/token
---
