---
authorization_urls: []
description: ''
docs: https://docs.keephq.dev/deployment/authentication/overview
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Keep Scopes
name_suffix: OAuth Scopes
note: Keep does not publish OAuth scopes; API access uses API keys/JWT bearer tokens with role-based access control (RBAC) configured per identity provider (Auth0, Keycloak, Azure AD, Okta, OneLogin), per https://docs.keephq.dev/deployment/authentication/overview.
overview: 'Keep uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keep
provider_slug: keep
schemes:
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/keep-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: keep-scopes
source_filename: keep-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keep-openapi.json\ndocs: https://docs.keephq.dev/deployment/authentication/overview\nnote: Keep does not publish OAuth scopes; API access uses API keys/JWT bearer tokens\n  with role-based access control (RBAC) configured per identity provider (Auth0,\n  Keycloak, Azure AD, Okta, OneLogin), per https://docs.keephq.dev/deployment/authentication/overview.\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/keep-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keep/refs/heads/main/scopes/keep-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AIOps
- Alerting
- Incident Management
- Observability
- Open Source
- SRE
- Workflow Automation
token_urls:
- token
---
