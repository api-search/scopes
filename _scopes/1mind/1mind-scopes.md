---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: 1Mind Scopes
name_suffix: OAuth Scopes
note: 'The advertised set is the Ory Hydra default and contains NO product scopes — there is no 1mind-specific scope (no read/write, no resource-scoped permission) published anywhere anonymously. Product scopes may exist and simply not be advertised in scopes_supported, which the OAuth 2.0 authorization server metadata spec (RFC 8414 §2) permits as OPTIONAL. Nothing is inferred or invented here: this file records exactly what the server publishes.'
overview: '1mind publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1mind API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1mind
provider_slug: 1mind
schemes: []
scope_count: 3
scope_names:
- openid
- offline_access
- offline
scopes:
- description: OpenID Connect — request an ID token and identify the end user. Required for any OIDC flow against this issuer.
  flows: []
  scope: openid
- description: Request a refresh token so the client can obtain new access tokens without user interaction.
  flows: []
  scope: offline_access
- description: Legacy Ory Hydra alias for offline_access; grants a refresh token.
  flows: []
  scope: offline
slug: 1mind-scopes
source_filename: 1mind-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.1mind.com/.well-known/openid-configuration (HTTP 200) —\n  scopes_supported\nname: 1mind OAuth Scopes\nauthorization_server: https://auth.1mind.com\nauthentication_reference: ../authentication/1mind-authentication.yml\ndocs: null\ndocs_note: >-\n  No public scope/permission reference page exists. These are the only scopes\n  1mind's authorization server advertises anonymously.\nscope_count: 3\nscopes:\n- name: openid\n  description: OpenID Connect — request an ID token and identify the end user.\n    Required for any OIDC flow against this issuer.\n  standard: OpenID Connect Core 1.0\n  source: scopes_supported\n- name: offline_access\n  description: Request a refresh token so the client can obtain new access\n    tokens without user interaction.\n  standard: OpenID Connect Core 1.0\n  source: scopes_supported\n- name: offline\n  description: Legacy Ory Hydra alias for offline_access; grants a refresh\n    token.\n\
  \  standard: Ory Hydra (vendor alias)\n  source: scopes_supported\nnote: >-\n  The advertised set is the Ory Hydra default and contains NO product scopes —\n  there is no 1mind-specific scope (no read/write, no resource-scoped\n  permission) published anywhere anonymously. Product scopes may exist and\n  simply not be advertised in scopes_supported, which the OAuth 2.0\n  authorization server metadata spec (RFC 8414 §2) permits as OPTIONAL. Nothing\n  is inferred or invented here: this file records exactly what the server\n  publishes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1mind/refs/heads/main/scopes/1mind-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Sales
- Go-To-Market
- Conversational AI
- Sales Enablement
- Revenue Operations
token_bound: false
token_urls: []
---
