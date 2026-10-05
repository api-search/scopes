---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agora Real Estate Scopes
name_suffix: OAuth Scopes
note: 'Derived from the discovery documents rather than from an OpenAPI — Agora''s specs declare no oauth2 securityScheme, because the one public specification in this repo describes the anonymous website content API. No scope reference page exists to upgrade this file to method: searched.'
overview: 'Agora Real Estate publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agora Real Estate API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agora Real Estate
provider_slug: agora-real-estate
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Requests an OpenID Connect ID token. Standard OIDC scope.
  flows: []
  scope: openid
- description: Requests basic profile claims (name, picture, updated_at). Standard OIDC scope.
  flows: []
  scope: profile
- description: Requests the email and email_verified claims. Standard OIDC scope.
  flows: []
  scope: email
- description: Requests a refresh token so the client can act after the user leaves. Standard OIDC scope.
  flows: []
  scope: offline_access
slug: agora-real-estate-scopes
source_filename: agora-real-estate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://auth.agorareal.com/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  The only scope surface Agora publishes is the scopes_supported list on its own OAuth 2.0 / OpenID\n  Connect authorization server at auth.agorareal.com. These are the four standard OIDC scopes — no\n  product or resource scopes (no read/write, no fund/investor/document scopes) are advertised, which\n  is consistent with the authorization server currently fronting interactive Cortex sign-in rather\n  than a public API. There is no published scopes or permissions reference page.\nauthorization_server: https://auth.agorareal.com\nscope_count: 4\nscopes:\n- name: openid\n  description: Requests an OpenID Connect ID token. Standard OIDC scope.\n  standard: true\n- name: profile\n  description: Requests basic profile claims (name, picture, updated_at). Standard OIDC scope.\n  standard: true\n- name: email\n  description: Requests the email and email_verified\
  \ claims. Standard OIDC scope.\n  standard: true\n- name: offline_access\n  description: Requests a refresh token so the client can act after the user leaves. Standard OIDC scope.\n  standard: true\nevidence:\n- url: https://auth.agorareal.com/.well-known/openid-configuration\n  status: 200\n- url: https://auth.agorareal.com/.well-known/oauth-authorization-server\n  status: 200\nnote: >-\n  Derived from the discovery documents rather than from an OpenAPI — Agora's specs declare no oauth2\n  securityScheme, because the one public specification in this repo describes the anonymous website\n  content API. No scope reference page exists to upgrade this file to method: searched.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/scopes/agora-real-estate-scopes.yml
summary_line: 4 scopes
tags:
- Real Estate
- Investment Management
- Private Equity
- Fund Administration
- Investor Relations
- Capital Raising
- Syndication
- Fund Accounting
- Investor Portal
- CRM
- Payments
- Content Management
- Software-as-a-Service
token_bound: false
token_urls: []
---
