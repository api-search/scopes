---
api_specs:
- filename: tender-agents-com-agent-discovery-api-openapi.yml
  format: yaml
  label: tender-agents-com Agent Discovery API
  slug: tender-agents-com-agent-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-agent-discovery-api-openapi.yml
- filename: tender-agents-com-erp-export-api-openapi.yml
  format: yaml
  label: tender-agents-com ERP Export API
  slug: tender-agents-com-erp-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-erp-export-api-openapi.yml
- filename: tender-agents-com-gaeb-api-openapi.yml
  format: yaml
  label: tender-agents-com Gaeb API
  slug: tender-agents-com-gaeb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-gaeb-api-openapi.yml
- filename: tender-agents-com-keys-api-openapi.yml
  format: yaml
  label: tender-agents-com Keys API
  slug: tender-agents-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-keys-api-openapi.yml
- filename: tender-agents-com-mcp-api-openapi.yml
  format: yaml
  label: tender-agents-com MCP API
  slug: tender-agents-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-mcp-api-openapi.yml
- filename: tender-agents-com-oauth-api-openapi.yml
  format: yaml
  label: tender-agents-com OAuth API
  slug: tender-agents-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-oauth-api-openapi.yml
- filename: tender-agents-com-profiles-api-openapi.yml
  format: yaml
  label: tender-agents-com Profiles API
  slug: tender-agents-com-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-profiles-api-openapi.yml
- filename: tender-agents-com-signup-api-openapi.yml
  format: yaml
  label: tender-agents-com Signup API
  slug: tender-agents-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-signup-api-openapi.yml
- filename: tender-agents-com-source-status-api-openapi.yml
  format: yaml
  label: tender-agents-com Source Status API
  slug: tender-agents-com-source-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-source-status-api-openapi.yml
- filename: tender-agents-com-tenders-api-openapi.yml
  format: yaml
  label: tender-agents-com Tenders API
  slug: tender-agents-com-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-tenders-api-openapi.yml
- filename: tender-agents-com-tenders-public-api-openapi.yml
  format: yaml
  label: tender-agents-com Tenders Public API
  slug: tender-agents-com-tenders-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-tenders-public-api-openapi.yml
- filename: tender-agents-com-webhooks-api-openapi.yml
  format: yaml
  label: tender-agents-com Webhooks API
  slug: tender-agents-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tender-agents-com/openapi/tender-agents-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tender Agents Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'tender-agents-com publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the tender-agents-com API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: tender-agents-com
provider_slug: tender-agents-com
schemes:
- description: 'OAuth 2.0 Client Credentials. client_id ist die Kennung eines API-Schluessels, client_secret der Schluessel selbst. Das Token laeuft nach einer Stunde ab und nennt seinen Umfang; wird der Schluessel widerrufen, traegt es sofort nicht mehr. Metadaten: /.well-known/oauth-authorization-server und /.well-known/oauth-protected-resource.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: oauth2ClientCredentials
  source: openapi/tender-agents-com-agentleads-openapi.json
scope_count: 4
scope_names:
- fulltext:read
- profiles:read
- tenders:read
- webhooks:write
scopes:
- description: Full text search across indexed notices. Requires a plan that permits it.
  flows:
  - clientCredentials
  scope: fulltext:read
- description: Read company profiles and their explained matches.
  flows:
  - clientCredentials
  scope: profiles:read
- description: Read tender search, detail, source status and country coverage.
  flows:
  - clientCredentials
  scope: tenders:read
- description: Manage delivery webhooks.
  flows:
  - clientCredentials
  scope: webhooks:write
slug: tender-agents-com-scopes
source_filename: tender-agents-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/tender-agents-com-agentleads-openapi.json\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/tender-agents-com-agentleads-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: 'OAuth 2.0 Client Credentials. client_id ist die Kennung eines API-Schluessels,\n    client_secret der Schluessel selbst. Das Token laeuft nach einer Stunde ab und nennt seinen\n    Umfang; wird der Schluessel widerrufen, traegt es sofort nicht mehr. Metadaten: /.well-known/oauth-authorization-server\n    und /.well-known/oauth-protected-resource.'\nscopes:\n- scope: fulltext:read\n  description: Full text search across indexed notices. Requires a plan that permits it.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/tender-agents-com-agentleads-openapi.json\n- scope: profiles:read\n  description: Read company profiles and their explained matches.\n  flows:\n  - clientCredentials\n \
  \ sources:\n  - openapi/tender-agents-com-agentleads-openapi.json\n- scope: tenders:read\n  description: Read tender search, detail, source status and country coverage.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/tender-agents-com-agentleads-openapi.json\n- scope: webhooks:write\n  description: Manage delivery webhooks.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/tender-agents-com-agentleads-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tender-agents-com/scopes/tender-agents-com-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- EU
- Procurement
- Tenders
- Artificial Intelligence
- Public Data
token_bound: false
token_urls:
- /oauth/token
---
