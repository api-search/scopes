---
api_specs:
- filename: inboxguard-io-account-api-openapi.yml
  format: yaml
  label: InboxGuard Account API
  slug: inboxguard-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-account-api-openapi.yml
- filename: inboxguard-io-alerts-api-openapi.yml
  format: yaml
  label: InboxGuard Alerts API
  slug: inboxguard-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-alerts-api-openapi.yml
- filename: inboxguard-io-domains-api-openapi.yml
  format: yaml
  label: InboxGuard Domains API
  slug: inboxguard-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-domains-api-openapi.yml
- filename: inboxguard-io-integrations-api-openapi.yml
  format: yaml
  label: InboxGuard Integrations API
  slug: inboxguard-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-integrations-api-openapi.yml
- filename: inboxguard-io-portfolio-api-openapi.yml
  format: yaml
  label: InboxGuard Portfolio API
  slug: inboxguard-io-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-portfolio-api-openapi.yml
- filename: inboxguard-io-reports-api-openapi.yml
  format: yaml
  label: InboxGuard Reports API
  slug: inboxguard-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-reports-api-openapi.yml
- filename: inboxguard-io-scanning-api-openapi.yml
  format: yaml
  label: InboxGuard Scanning API
  slug: inboxguard-io-scanning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-scanning-api-openapi.yml
- filename: inboxguard-io-system-api-openapi.yml
  format: yaml
  label: InboxGuard System API
  slug: inboxguard-io-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-system-api-openapi.yml
- filename: inboxguard-io-webhooks-api-openapi.yml
  format: yaml
  label: InboxGuard Webhooks API
  slug: inboxguard-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxguard-io/openapi/inboxguard-io-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: InboxGuard Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'InboxGuard publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the InboxGuard API on a user''s behalf.


  Tokens are issued from https://api.inboxguard.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: InboxGuard
provider_slug: inboxguard-io
schemes:
- description: 'OAuth-shaped wrapper around the same API key. The ONLY grant is client_credentials at POST https://api.inboxguard.io/oauth/token, where the client_secret IS an InboxGuard API key (HTTP Basic or body); the returned access_token is that same key. There is NO authorization_code flow, NO PKCE, and NO /oauth/authorize endpoint. Discovery: /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource on api.inboxguard.io. See https://inboxguard.io/auth.md.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.inboxguard.io/oauth/token
  name: OAuth2
  source: openapi/inboxguard-io-openapi.json
scope_count: 2
scope_names:
- full
- read
scopes:
- description: Full read/write access (all methods).
  flows:
  - clientCredentials
  scope: full
- description: Read-only access (GET).
  flows:
  - clientCredentials
  scope: read
slug: inboxguard-io-scopes
source_filename: inboxguard-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/inboxguard-io-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/inboxguard-io-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.inboxguard.io/oauth/token\n  description: 'OAuth-shaped wrapper around the same API key. The ONLY grant is client_credentials\n    at POST https://api.inboxguard.io/oauth/token, where the client_secret IS an InboxGuard\n    API key (HTTP Basic or body); the returned access_token is that same key. There is NO authorization_code\n    flow, NO PKCE, and NO /oauth/authorize endpoint. Discovery: /.well-known/oauth-authorization-server\n    and /.well-known/oauth-protected-resource on api.inboxguard.io. See https://inboxguard.io/auth.md.'\nscopes:\n- scope: full\n  description: Full read/write access (all methods).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/inboxguard-io-openapi.json\n- scope: read\n  description: Read-only access (GET).\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/inboxguard-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/inboxguard-io/scopes/inboxguard-io-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Email Deliverability
- DMARC
- DNS Monitoring
- Authentication
- Security
token_bound: false
token_urls:
- https://api.inboxguard.io/oauth/token
---
