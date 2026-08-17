---
api_specs:
- filename: snov-io-authentication-api-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-io-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-authentication-api-openapi.yml
- filename: snov-io-campaigns-api-openapi.yml
  format: yaml
  label: Snov.io Campaigns API
  slug: snov-io-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-campaigns-api-openapi.yml
- filename: snov-io-crm-pipeline-api-openapi.yml
  format: yaml
  label: Snov.io CRM Pipeline API
  slug: snov-io-crm-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-crm-pipeline-api-openapi.yml
- filename: snov-io-domain-search-api-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-io-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-domain-search-api-openapi.yml
- filename: snov-io-email-accounts-api-openapi.yml
  format: yaml
  label: Snov.io Email Accounts API
  slug: snov-io-email-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-accounts-api-openapi.yml
- filename: snov-io-email-finder-api-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-io-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-finder-api-openapi.yml
- filename: snov-io-email-verification-api-openapi.yml
  format: yaml
  label: Snov.io Email Verification API
  slug: snov-io-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-verification-api-openapi.yml
- filename: snov-io-email-warm-up-api-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-io-email-warm-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-email-warm-up-api-openapi.yml
- filename: snov-io-prospects-api-openapi.yml
  format: yaml
  label: Snov.io Prospects API
  slug: snov-io-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-prospects-api-openapi.yml
- filename: snov-io-user-api-openapi.yml
  format: yaml
  label: Snov.io User API
  slug: snov-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-user-api-openapi.yml
- filename: snov-io-webhooks-api-openapi.yml
  format: yaml
  label: Snov.io Webhooks API
  slug: snov-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/openapi/snov-io-webhooks-api-openapi.yml
authorization_urls:
- https://app.snov.io/mcp/authorize
description: 'Snov.io issues exactly ONE OAuth scope across its entire platform: "mcp", advertised by the authorization server on app.snov.io and required by the remote MCP server on mcp.snov.io. The REST API issues no scopes at all — its client_credentials exchange accepts no scope parameter and returns a token whose authority is derived entirely from the account''s subscription plan and credit balance.'
docs: https://snov.io/api
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Snov Io Scopes
name_suffix: OAuth Scopes
note: Upgraded from derived to probed. The previous round recorded "no OAuth scopes are documented", which was true of the REST API but missed the MCP authorization server entirely. Both discovery documents are now captured verbatim under well-known/.
overview: 'Snov.io uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.snov.io/v1/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Snov.io
provider_slug: snov-io
schemes:
- authorization_model: plan-derived
  description: POST client_id and client_secret to obtain a 3600-second Bearer token, then send it in the Authorization header. No scope parameter is accepted and none is returned.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.snov.io/v1/oauth/access_token
  name: OAuth2ClientCredentials
  note: Access is governed by the subscription tier (API access begins at the Starter plan) and by the credit balance, not by any scope on the credential. There is no read-only credential, no per-integration credential and no way to restrict a token to a subset of the surface.
  scopes_supported: []
  source: https://snov.io/api
  surface: REST API
- description: Public-client authorization code flow with PKCE and dynamic client registration. One scope, granted or not granted.
  flows:
  - authorizationUrl: https://app.snov.io/mcp/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://app.snov.io/back/mcp/oauth/register
    tokenUrl: https://app.snov.io/back/mcp/oauth/token
  name: OAuth2AuthorizationCodeMCP
  resource: https://mcp.snov.io/mcp
  scopes_supported:
  - mcp
  source: https://app.snov.io/.well-known/oauth-authorization-server
  surface: MCP server
scope_count: 0
scope_names: []
scopes: []
slug: snov-io-scopes
source_filename: snov-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://app.snov.io/.well-known/oauth-authorization-server and\n  https://mcp.snov.io/.well-known/oauth-protected-resource (both HTTP 200, 2026-08-13)\ndocs: https://snov.io/api\ndescription: >-\n  Snov.io issues exactly ONE OAuth scope across its entire platform: \"mcp\", advertised by the\n  authorization server on app.snov.io and required by the remote MCP server on mcp.snov.io. The\n  REST API issues no scopes at all — its client_credentials exchange accepts no scope parameter\n  and returns a token whose authority is derived entirely from the account's subscription plan\n  and credit balance.\n\nnote: >-\n  Upgraded from derived to probed. The previous round recorded \"no OAuth scopes are documented\",\n  which was true of the REST API but missed the MCP authorization server entirely. Both\n  discovery documents are now captured verbatim under well-known/.\n\nschemes:\n  - name: OAuth2ClientCredentials\n    surface:\
  \ REST API\n    source: https://snov.io/api\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.snov.io/v1/oauth/access_token\n    scopes_supported: []\n    description: >-\n      POST client_id and client_secret to obtain a 3600-second Bearer token, then send it in the\n      Authorization header. No scope parameter is accepted and none is returned.\n    authorization_model: plan-derived\n    note: >-\n      Access is governed by the subscription tier (API access begins at the Starter plan) and by\n      the credit balance, not by any scope on the credential. There is no read-only credential,\n      no per-integration credential and no way to restrict a token to a subset of the surface.\n\n  - name: OAuth2AuthorizationCodeMCP\n    surface: MCP server\n    source: https://app.snov.io/.well-known/oauth-authorization-server\n    resource: https://mcp.snov.io/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.snov.io/mcp/authorize\n\
  \        tokenUrl: https://app.snov.io/back/mcp/oauth/token\n        registrationUrl: https://app.snov.io/back/mcp/oauth/register\n        pkce: S256\n    scopes_supported:\n      - mcp\n    description: >-\n      Public-client authorization code flow with PKCE and dynamic client registration. One\n      scope, granted or not granted.\n\nscopes:\n  - name: mcp\n    surface: MCP server\n    resource: https://mcp.snov.io/mcp\n    description: >-\n      Grants an authorized MCP client the full published Snov.io action surface — prospect\n      search and enrichment, list and folder management, email verification, the Sales CRM\n      (pipelines, deals, notes, loss reasons, tasks) and LinkedIn account setup and outreach.\n    read_write: both\n    source: https://app.snov.io/.well-known/oauth-authorization-server\n    evidence: 'scopes_supported: [\"mcp\"] in the RFC 8414 metadata; scope=\"mcp\" in the RFC 9728 WWW-Authenticate challenge from mcp.snov.io.'\n\nsummary:\n  scope_count: 1\n \
  \ granular_scopes: false\n  read_only_scope_available: false\n  finding: >-\n    A single all-or-nothing scope covering more than 100 actions, including irreversible\n    write actions — sending LinkedIn connection requests and InMails, deleting prospect lists,\n    marking deals lost. An account holder connecting an AI assistant cannot grant it read access\n    only, and cannot withhold LinkedIn outreach while allowing prospect search. This is the most\n    consequential authorization gap on the Snov.io agent surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov-io/refs/heads/main/scopes/snov-io-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sales Automation
- Email Finder
- Email Verification
- Lead Generation
- Drip Campaigns
- CRM
- LinkedIn Automation
- Prospect Management
- Data Enrichment
- Cold Email
token_urls:
- https://api.snov.io/v1/oauth/access_token
- https://app.snov.io/back/mcp/oauth/token
---
