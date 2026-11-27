---
api_specs:
- filename: licium-ai-agents-capabilities-api-openapi.yml
  format: yaml
  label: Licium Agents & capabilities API
  slug: licium-ai-agents-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-agents-capabilities-api-openapi.yml
- filename: licium-ai-always-on-teammate-api-openapi.yml
  format: yaml
  label: Licium Always-on teammate API
  slug: licium-ai-always-on-teammate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-always-on-teammate-api-openapi.yml
- filename: licium-ai-authorizations-api-openapi.yml
  format: yaml
  label: Licium Authorizations API
  slug: licium-ai-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-authorizations-api-openapi.yml
- filename: licium-ai-bounties-needs-api-openapi.yml
  format: yaml
  label: Licium Bounties & needs API
  slug: licium-ai-bounties-needs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-bounties-needs-api-openapi.yml
- filename: licium-ai-discovery-api-openapi.yml
  format: yaml
  label: Licium Discovery API
  slug: licium-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-discovery-api-openapi.yml
- filename: licium-ai-mcp-directory-api-openapi.yml
  format: yaml
  label: Licium MCP directory API
  slug: licium-ai-mcp-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-mcp-directory-api-openapi.yml
- filename: licium-ai-payer-follow-ups-api-openapi.yml
  format: yaml
  label: Licium Payer follow-ups API
  slug: licium-ai-payer-follow-ups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-payer-follow-ups-api-openapi.yml
- filename: licium-ai-payments-api-openapi.yml
  format: yaml
  label: Licium Payments API
  slug: licium-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-payments-api-openapi.yml
- filename: licium-ai-provider-checks-api-openapi.yml
  format: yaml
  label: Licium Provider checks API
  slug: licium-ai-provider-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-provider-checks-api-openapi.yml
- filename: licium-ai-received-work-checks-api-openapi.yml
  format: yaml
  label: Licium Received-work checks API
  slug: licium-ai-received-work-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-received-work-checks-api-openapi.yml
- filename: licium-ai-sources-api-openapi.yml
  format: yaml
  label: Licium Sources API
  slug: licium-ai-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-sources-api-openapi.yml
- filename: licium-ai-supplier-checkout-api-openapi.yml
  format: yaml
  label: Licium Supplier Checkout API
  slug: licium-ai-supplier-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-supplier-checkout-api-openapi.yml
- filename: licium-ai-vendor-checks-api-openapi.yml
  format: yaml
  label: Licium Vendor checks API
  slug: licium-ai-vendor-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-vendor-checks-api-openapi.yml
authorization_urls:
- https://www.licium.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Licium Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Licium publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Licium API on a user''s behalf.


  Tokens are issued from https://www.licium.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Licium
provider_slug: licium-ai
schemes:
- description: Sign-in for the hosted MCP (/mcp, /mcp/claude, /mcp/chatgpt). The token works only at the MCP address it was issued for, never on /v1 routes.
  flows:
  - authorizationUrl: https://www.licium.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.licium.ai/oauth/token
  name: McpOAuth
  source: openapi/licium-ai-openapi.json
scope_count: 2
scope_names:
- account
- agent
scopes:
- description: Act as the signed-in email on what that email owns (checks, payer follow-ups, authorizations, their payer exchanges).
  flows:
  - authorizationCode
  scope: account
- description: Act as one agent the person chose, within its spending limits.
  flows:
  - authorizationCode
  scope: agent
slug: licium-ai-scopes
source_filename: licium-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/licium-ai-openapi.json\nschemes:\n- name: McpOAuth\n  source: openapi/licium-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.licium.ai/oauth/authorize\n    tokenUrl: https://www.licium.ai/oauth/token\n  description: Sign-in for the hosted MCP (/mcp, /mcp/claude, /mcp/chatgpt). The token works\n    only at the MCP address it was issued for, never on /v1 routes.\nscopes:\n- scope: account\n  description: Act as the signed-in email on what that email owns (checks, payer follow-ups,\n    authorizations, their payer exchanges).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/licium-ai-openapi.json\n- scope: agent\n  description: Act as one agent the person chose, within its spending limits.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/licium-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/licium-ai/scopes/licium-ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Healthcare
- Software-as-a-Service
- Credentialing
- Automation
token_bound: false
token_urls:
- https://www.licium.ai/oauth/token
---
