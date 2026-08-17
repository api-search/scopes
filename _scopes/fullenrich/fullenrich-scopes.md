---
api_specs:
- filename: fullenrich-contact-enrichment-api-openapi.yml
  format: yaml
  label: FullEnrich Contact Enrichment API
  slug: fullenrich-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-contact-enrichment-api-openapi.yml
- filename: fullenrich-reverse-email-lookup-api-openapi.yml
  format: yaml
  label: FullEnrich Reverse Email Lookup API
  slug: fullenrich-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-reverse-email-lookup-api-openapi.yml
- filename: fullenrich-search-api-openapi.yml
  format: yaml
  label: FullEnrich Search API
  slug: fullenrich-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-search-api-openapi.yml
- filename: fullenrich-lookup-api-openapi.yml
  format: yaml
  label: FullEnrich Lookup API
  slug: fullenrich-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-lookup-api-openapi.yml
- filename: fullenrich-account-api-openapi.yml
  format: yaml
  label: FullEnrich Account API
  slug: fullenrich-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-account-api-openapi.yml
authorization_urls:
- https://app.fullenrich.com/oauth2/authorize
- https://mcp.fullenrich.com/authorize
description: FullEnrich publishes two OAuth scope surfaces. The application authorization server declares 13 resource-scoped, read/write-split scopes. The MCP authorization server declares a single coarse `api:mcp` scope covering the whole agent surface. Neither is documented in prose anywhere on the developer site — both were recovered from well-known metadata, and no human-readable scope reference page exists.
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Fullenrich Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FullEnrich publishes 14 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the FullEnrich API on a user''s behalf.


  Tokens are issued from https://app.fullenrich.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FullEnrich
provider_slug: fullenrich
schemes:
- flows:
  - authorizationUrl: https://app.fullenrich.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.fullenrich.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://app.fullenrich.com/oauth2/token
  issuer: fullenrich
  name: FullEnrichOAuth
  source: well-known/fullenrich-app-openid-configuration.json
- flows:
  - authorizationUrl: https://mcp.fullenrich.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.fullenrich.com/token
  issuer: https://mcp.fullenrich.com
  name: FullEnrichMCPOAuth
  source: well-known/fullenrich-mcp-oauth-authorization-server.json
scope_count: 14
scope_names:
- workspace:read
- workspace:write
- enrichment:read
- enrichment:write
- crm:read
- crm:write
- credit:read
- credit:write
- listing:read
- listing:write
- payment:read
- token:read
- token:write
- api:mcp
scopes:
- description: Read workspace configuration and membership. (Inferred from scope name; not documented in prose.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: workspace:read
- description: Modify workspace configuration and membership. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: workspace:write
- description: Read enrichment jobs and their results. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrichment:read
- description: Submit enrichment jobs. This is the credit-spending scope. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: enrichment:write
- description: Read connected CRM objects (HubSpot / Salesforce integrations). (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: crm:read
- description: Write enriched data back to a connected CRM. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: crm:write
- description: Read the workspace credit balance. Corresponds to GET /account/credits. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: credit:read
- description: Modify credit allocation (e.g. per-user credit limits). (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: credit:write
- description: Read saved lists of people/companies. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: listing:read
- description: Create and modify saved lists. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: listing:write
- description: Read billing and payment state. Read-only — no payment:write scope is offered. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: payment:read
- description: Read API keys / tokens issued for the workspace. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: token:read
- description: Issue or revoke API keys / tokens. (Inferred.)
  flows:
  - authorizationCode
  - clientCredentials
  scope: token:write
- description: Single coarse scope granted to an MCP client for the whole agent surface — search, enrichment and export alike. There is no read-only variant, so an agent authorized for search is also authorized to spend credits.
  flows:
  - authorizationCode
  scope: api:mcp
slug: fullenrich-scopes
source_filename: fullenrich-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://app.fullenrich.com/.well-known/openid-configuration and\n  https://mcp.fullenrich.com/.well-known/oauth-protected-resource — read directly\n  from the provider's published RFC 8414 / RFC 9728 discovery metadata.\ndescription: >-\n  FullEnrich publishes two OAuth scope surfaces. The application authorization\n  server declares 13 resource-scoped, read/write-split scopes. The MCP\n  authorization server declares a single coarse `api:mcp` scope covering the whole\n  agent surface. Neither is documented in prose anywhere on the developer site —\n  both were recovered from well-known metadata, and no human-readable scope\n  reference page exists.\ndocs: null\ndocs_gap: >-\n  No published scopes/permissions reference page was found on fullenrich.com,\n  docs.fullenrich.com or help.fullenrich.com. The descriptions below are inferred\n  from the scope names' own resource:action structure and are marked as such —\n  the\
  \ provider publishes no prose definition to quote.\n\nschemes:\n  - name: FullEnrichOAuth\n    issuer: fullenrich\n    source: well-known/fullenrich-app-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.fullenrich.com/oauth2/authorize\n        tokenUrl: https://app.fullenrich.com/oauth2/token\n      - flow: clientCredentials\n        tokenUrl: https://app.fullenrich.com/oauth2/token\n  - name: FullEnrichMCPOAuth\n    issuer: https://mcp.fullenrich.com\n    source: well-known/fullenrich-mcp-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.fullenrich.com/authorize\n        tokenUrl: https://mcp.fullenrich.com/token\n\nscope_count: 14\n\nscopes:\n  - scope: workspace:read\n    resource: workspace\n    action: read\n    description: Read workspace configuration and membership. (Inferred from scope name; not documented in prose.)\n    flows: [authorizationCode, clientCredentials]\n\
  \    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: workspace:write\n    resource: workspace\n    action: write\n    description: Modify workspace configuration and membership. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: enrichment:read\n    resource: enrichment\n    action: read\n    description: Read enrichment jobs and their results. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: enrichment:write\n    resource: enrichment\n    action: write\n    description: Submit enrichment jobs. This is the credit-spending scope. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: crm:read\n    resource: crm\n    action: read\n    description: Read connected CRM objects (HubSpot / Salesforce\
  \ integrations). (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: crm:write\n    resource: crm\n    action: write\n    description: Write enriched data back to a connected CRM. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: credit:read\n    resource: credit\n    action: read\n    description: Read the workspace credit balance. Corresponds to GET /account/credits. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: credit:write\n    resource: credit\n    action: write\n    description: Modify credit allocation (e.g. per-user credit limits). (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: listing:read\n    resource: listing\n\
  \    action: read\n    description: Read saved lists of people/companies. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: listing:write\n    resource: listing\n    action: write\n    description: Create and modify saved lists. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: payment:read\n    resource: payment\n    action: read\n    description: Read billing and payment state. Read-only — no payment:write scope is offered. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: token:read\n    resource: token\n    action: read\n    description: Read API keys / tokens issued for the workspace. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n\
  \  - scope: token:write\n    resource: token\n    action: write\n    description: Issue or revoke API keys / tokens. (Inferred.)\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/fullenrich-app-openid-configuration.json]\n  - scope: api:mcp\n    resource: mcp\n    action: all\n    description: >-\n      Single coarse scope granted to an MCP client for the whole agent surface —\n      search, enrichment and export alike. There is no read-only variant, so an\n      agent authorized for search is also authorized to spend credits.\n    flows: [authorizationCode]\n    server: https://mcp.fullenrich.com\n    sources:\n      - well-known/fullenrich-mcp-oauth-protected-resource.json\n      - well-known/fullenrich-mcp-oauth-authorization-server.json\n\nobservations:\n  - >-\n    The application server's scopes are cleanly resource:action split, which is\n    good practice, but they are undocumented — an integrator cannot discover them\n    without reading the well-known\
  \ metadata.\n  - >-\n    The MCP server takes the opposite approach: one scope for everything. Agent\n    least-privilege is therefore not expressible on the MCP surface; the\n    preview-then-confirm pattern FullEnrich documents is a client-side convention,\n    not a scope boundary.\n\nx-evidence:\n  - url: https://app.fullenrich.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://mcp.fullenrich.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/scopes/fullenrich-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials
tags:
- B2B Data
- Contact Enrichment
- Email Finder
- Phone Finder
- Waterfall Enrichment
- Sales Intelligence
- People Search
- Company Search
- Reverse Email Lookup
- Agent Ready
token_urls:
- https://app.fullenrich.com/oauth2/token
- https://mcp.fullenrich.com/token
---
