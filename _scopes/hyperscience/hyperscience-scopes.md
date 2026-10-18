---
api_specs:
- filename: hyperscience-audit-logs-api-openapi.yml
  format: yaml
  label: Hyperscience Audit Logs API
  slug: hyperscience-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-audit-logs-api-openapi.yml
- filename: hyperscience-cases-api-openapi.yml
  format: yaml
  label: Hyperscience Cases API
  slug: hyperscience-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-cases-api-openapi.yml
- filename: hyperscience-documents-api-openapi.yml
  format: yaml
  label: Hyperscience Documents API
  slug: hyperscience-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-documents-api-openapi.yml
- filename: hyperscience-flow-runs-api-openapi.yml
  format: yaml
  label: Hyperscience Flow Runs API
  slug: hyperscience-flow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flow-runs-api-openapi.yml
- filename: hyperscience-flows-api-openapi.yml
  format: yaml
  label: Hyperscience Flows API
  slug: hyperscience-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-flows-api-openapi.yml
- filename: hyperscience-layouts-api-openapi.yml
  format: yaml
  label: Hyperscience Layouts API
  slug: hyperscience-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-layouts-api-openapi.yml
- filename: hyperscience-pages-api-openapi.yml
  format: yaml
  label: Hyperscience Pages API
  slug: hyperscience-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-pages-api-openapi.yml
- filename: hyperscience-submissions-api-openapi.yml
  format: yaml
  label: Hyperscience Submissions API
  slug: hyperscience-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-submissions-api-openapi.yml
- filename: hyperscience-version-api-openapi.yml
  format: yaml
  label: Hyperscience Version API
  slug: hyperscience-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-version-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Hyperscience Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Hyperscience uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{server}.{company}.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hyperscience
provider_slug: hyperscience
schemes:
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-audit-logs-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-cases-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-documents-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-flow-runs-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-flows-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-layouts-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-pages-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-submissions-api-openapi.yml
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  source: openapi/hyperscience-version-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: hyperscience-scopes
source_filename: hyperscience-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/hyperscience-audit-logs-api-openapi.yml, openapi/hyperscience-cases-api-openapi.yml,\n  openapi/hyperscience-documents-api-openapi.yml, openapi/hyperscience-flow-runs-api-openapi.yml,\n  openapi/hyperscience-flows-api-openapi.yml, openapi/hyperscience-layouts-api-openapi.yml,\n  openapi/hyperscience-pages-api-openapi.yml, openapi/hyperscience-submissions-api-openapi.yml,\n  openapi/hyperscience-version-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/hyperscience-audit-logs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-cases-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by\
  \ the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-documents-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-flow-runs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-flows-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-layouts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n\
  \  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-pages-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-submissions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n- name: OAuth2\n  source: openapi/hyperscience-version-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and\
  \ no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/scopes/hyperscience-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Document AI
- Intelligent Document Processing
- Enterprise
- Automation
- Generative AI
- FedRAMP
token_bound: false
token_urls:
- https://{server}.{company}.com/oauth/token
---
