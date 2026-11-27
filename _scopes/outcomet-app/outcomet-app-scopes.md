---
api_specs:
- filename: outcomet-app-ask-api-openapi.yml
  format: yaml
  label: Outcomet Ask API
  slug: outcomet-app-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-ask-api-openapi.yml
- filename: outcomet-app-batch-api-openapi.yml
  format: yaml
  label: Outcomet Batch API
  slug: outcomet-app-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-batch-api-openapi.yml
- filename: outcomet-app-discovery-api-openapi.yml
  format: yaml
  label: Outcomet Discovery API
  slug: outcomet-app-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-discovery-api-openapi.yml
- filename: outcomet-app-mcp-api-openapi.yml
  format: yaml
  label: Outcomet MCP API
  slug: outcomet-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-mcp-api-openapi.yml
- filename: outcomet-app-onboarding-api-openapi.yml
  format: yaml
  label: Outcomet Onboarding API
  slug: outcomet-app-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-onboarding-api-openapi.yml
- filename: outcomet-app-sandbox-api-openapi.yml
  format: yaml
  label: Outcomet Sandbox API
  slug: outcomet-app-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outcomet-app/openapi/outcomet-app-sandbox-api-openapi.yml
authorization_urls:
- https://mcp.outcomet.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Outcomet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Outcomet publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Outcomet API on a user''s behalf.


  Tokens are issued from https://mcp.outcomet.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Outcomet
provider_slug: outcomet-app
schemes:
- description: OAuth 2.1 Authorization Code with PKCE (S256). Dynamic Client Registration (RFC 7591) at https://mcp.outcomet.app/oauth/register; RFC 8414 metadata at https://mcp.outcomet.app/.well-known/oauth-authorization-server.
  flows:
  - authorizationUrl: https://mcp.outcomet.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.outcomet.app/oauth/token
  name: oauth2
  source: openapi/outcomet-app-openapi.json
scope_count: 10
scope_names:
- capabilities:create
- capabilities:write
- competitors:write
- contacts:write
- feedback:create
- feedback:write
- initiatives:write
- problems:write
- product_context:read
- work_items:write
scopes:
- description: Create new product capabilities in the capability hierarchy.
  flows:
  - authorizationCode
  scope: capabilities:create
- description: Update, reparent, merge, or retire existing capabilities.
  flows:
  - authorizationCode
  scope: capabilities:write
- description: Create and update competitor profiles and threat analysis.
  flows:
  - authorizationCode
  scope: competitors:write
- description: Create and update companies, contacts, and campaign interactions.
  flows:
  - authorizationCode
  scope: contacts:write
- description: Create new customer feedback items and attach source evidence.
  flows:
  - authorizationCode
  scope: feedback:create
- description: Update existing feedback items, status, and linked changes.
  flows:
  - authorizationCode
  scope: feedback:write
- description: Create and update product initiatives, goals, and capability links.
  flows:
  - authorizationCode
  scope: initiatives:write
- description: Create problems, link evidence, and review problem proposals.
  flows:
  - authorizationCode
  scope: problems:write
- description: Read capabilities, initiatives, problems, feedback, evidence chunks, contacts, campaigns, and competitors.
  flows:
  - authorizationCode
  scope: product_context:read
- description: Update engineering work items and link changes.
  flows:
  - authorizationCode
  scope: work_items:write
slug: outcomet-app-scopes
source_filename: outcomet-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/outcomet-app-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/outcomet-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.outcomet.app/oauth/authorize\n    tokenUrl: https://mcp.outcomet.app/oauth/token\n  description: OAuth 2.1 Authorization Code with PKCE (S256). Dynamic Client Registration (RFC\n    7591) at https://mcp.outcomet.app/oauth/register; RFC 8414 metadata at https://mcp.outcomet.app/.well-known/oauth-authorization-server.\nscopes:\n- scope: capabilities:create\n  description: Create new product capabilities in the capability hierarchy.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: capabilities:write\n  description: Update, reparent, merge, or retire existing capabilities.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: competitors:write\n  description: Create and\
  \ update competitor profiles and threat analysis.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: contacts:write\n  description: Create and update companies, contacts, and campaign interactions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: feedback:create\n  description: Create new customer feedback items and attach source evidence.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: feedback:write\n  description: Update existing feedback items, status, and linked changes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: initiatives:write\n  description: Create and update product initiatives, goals, and capability links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: problems:write\n  description: Create problems, link evidence, and review problem proposals.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: product_context:read\n  description: Read capabilities, initiatives, problems, feedback, evidence chunks, contacts,\n    campaigns, and competitors.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n- scope: work_items:write\n  description: Update engineering work items and link changes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/outcomet-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/outcomet-app/scopes/outcomet-app-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Company
- Product Management
- Feedback
- Decision-Making
token_bound: false
token_urls:
- https://mcp.outcomet.app/oauth/token
---
