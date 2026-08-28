---
authorization_urls: []
description: The Pocus authorization server advertises only the three standard OpenID Connect scopes. No product-level or resource-level scopes (read/write over accounts, playbooks, lists, signals) are advertised, which means the published OAuth surface authenticates a user but does not express any granular authorization for the Pocus data API.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pocus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pocus uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pocus
provider_slug: pocus
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: pocus-scopes
source_filename: pocus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://auth.pocus.com/.well-known/openid-configuration and\n  https://auth.pocus.com/.well-known/oauth-authorization-server, both HTTP 200, fetched 2026-08-26\ndocs: null\ndocs_note: >-\n  Pocus publishes no scopes/permissions reference page. The scope list below is read directly from\n  the authorization server's own advertised metadata (`scopes_supported`) and nothing has been\n  added to it.\nname: Pocus OAuth 2.0 scopes\ndescription: >-\n  The Pocus authorization server advertises only the three standard OpenID Connect scopes. No\n  product-level or resource-level scopes (read/write over accounts, playbooks, lists, signals) are\n  advertised, which means the published OAuth surface authenticates a user but does not express any\n  granular authorization for the Pocus data API.\n\nissuer: https://auth.pocus.com\nauthorization_endpoint: https://auth.pocus.com/oauth/authorize\ntoken_endpoint: https://auth.pocus.com/oauth/token\n\
  \nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope requesting an ID token. Required to use the OIDC layer.\n  standard: OpenID Connect Core 1.0\n  source: scopes_supported\n- name: profile\n  description: >-\n    Standard OIDC claim scope granting access to the end user's default profile claims.\n  standard: OpenID Connect Core 1.0\n  source: scopes_supported\n- name: email\n  description: >-\n    Standard OIDC claim scope granting access to the end user's email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n  source: scopes_supported\n\nscope_count: 3\nproduct_scopes_published: 0\n\ngranted_grants:\n- authorization_code\n- refresh_token\n- client_credentials\n- 'urn:ietf:params:oauth:grant-type:token-exchange'\n- 'urn:ietf:params:oauth:grant-type:device_code'\n\npkce:\n  supported: true\n  code_challenge_methods: [S256]\n\nrelated_authorization_model:\n  note: >-\n    Pocus' actual permission model is role-based inside the workspace, not\
  \ scope-based on the\n    token. Roles and supplementary permissions are administered in Workspace Settings > User\n    Management and are documented at https://docs.pocus.com/docs/permissions; Okta groups map onto\n    those roles via SAML. That model is not expressed in OAuth scopes.\n  docs: https://docs.pocus.com/docs/permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pocus/refs/heads/main/scopes/pocus-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Sales Intelligence
- Product-Led Sales
- Revenue Operations
- Go-To-Market
- Data Enrichment
- CRM
- Artificial Intelligence
- GraphQL
token_urls: []
---
