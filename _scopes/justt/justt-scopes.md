---
api_specs:
- filename: justt-chargebacks-api-openapi.yml
  format: yaml
  label: Justt Chargebacks API
  slug: justt-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-chargebacks-api-openapi.yml
- filename: justt-data-subjects-api-openapi.yml
  format: yaml
  label: Justt Data Subjects API
  slug: justt-data-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-data-subjects-api-openapi.yml
- filename: justt-evidence-api-openapi.yml
  format: yaml
  label: Justt Evidence API
  slug: justt-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-evidence-api-openapi.yml
- filename: justt-files-api-openapi.yml
  format: yaml
  label: Justt Files API
  slug: justt-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-files-api-openapi.yml
- filename: justt-integrations-api-openapi.yml
  format: yaml
  label: Justt Integrations API
  slug: justt-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-integrations-api-openapi.yml
- filename: justt-merchants-api-openapi.yml
  format: yaml
  label: Justt Merchants API
  slug: justt-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-merchants-api-openapi.yml
- filename: justt-pre-chargeback-alerts-api-openapi.yml
  format: yaml
  label: Justt Pre-chargeback Alerts API
  slug: justt-pre-chargeback-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-pre-chargeback-alerts-api-openapi.yml
- filename: justt-sandbox-api-openapi.yml
  format: yaml
  label: Justt Sandbox API
  slug: justt-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-sandbox-api-openapi.yml
- filename: justt-transactions-api-openapi.yml
  format: yaml
  label: Justt Transactions API
  slug: justt-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-transactions-api-openapi.yml
authorization_urls:
- https://justt.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Justt Scopes
name_suffix: OAuth Scopes
note: The Justt REST API and Pre-Chargeback Alerts API declare NO oauth2 security scheme and publish no scope or permission model — a bearer API key carries full privilege (see authentication/justt-authentication.yml). The only OAuth surface Justt exposes is the MCP endpoint on its WordPress host, whose RFC 8414 metadata declares a single scope. That is what is recorded here; it is discovered by probe, not documented by Justt, and it does not govern the chargeback API.
overview: 'Justt publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Justt API on a user''s behalf.


  Tokens are issued from https://justt.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Justt
provider_slug: justt
schemes:
- flows:
  - authorizationUrl: https://justt.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://justt.ai/oauth/revoke
    tokenUrl: https://justt.ai/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://justt.ai
  name: mcp-oauth
  source: well-known/justt-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope advertised by Justt's authorization-server metadata, and the only scope named by the protected-resource document for https://justt.ai/wp-json/mcp/mcp-oauth-server. No finer-grained scope is published; what it grants could not be determined because tools/list returns HTTP 401.
  flows:
  - authorizationCode
  scope: mcp
slug: justt-scopes
source_filename: justt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://justt.ai/.well-known/oauth-authorization-server\napplies_to: MCP endpoint only\nnote: >-\n  The Justt REST API and Pre-Chargeback Alerts API declare NO oauth2 security\n  scheme and publish no scope or permission model — a bearer API key carries full\n  privilege (see authentication/justt-authentication.yml). The only OAuth surface\n  Justt exposes is the MCP endpoint on its WordPress host, whose RFC 8414 metadata\n  declares a single scope. That is what is recorded here; it is discovered by\n  probe, not documented by Justt, and it does not govern the chargeback API.\ndocs: null\nschemes:\n- name: mcp-oauth\n  source: well-known/justt-oauth-authorization-server.json\n  issuer: https://justt.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://justt.ai/oauth/authorize\n    tokenUrl: https://justt.ai/oauth/token\n    revocationUrl: https://justt.ai/oauth/revoke\n    pkce: S256\n    token_endpoint_auth_methods:\
  \ [none]\nscopes:\n- scope: mcp\n  description: >-\n    The single scope advertised by Justt's authorization-server metadata, and the\n    only scope named by the protected-resource document for\n    https://justt.ai/wp-json/mcp/mcp-oauth-server. No finer-grained scope is\n    published; what it grants could not be determined because tools/list returns\n    HTTP 401.\n  flows: [authorizationCode]\n  sources:\n  - well-known/justt-oauth-authorization-server.json\n  - well-known/justt-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-23'\n  urls:\n  - url: https://justt.ai/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://justt.ai/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/scopes/justt-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Payments
- Chargebacks
- Disputes
- Fraud
- Risk
- Financial-Services
- E-Commerce
- Artificial Intelligence
- Webhook
token_urls:
- https://justt.ai/oauth/token
---
