---
authorization_urls:
- https://auth.aircall.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aircall Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aircall publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aircall API on a user''s behalf.


  Tokens are issued from https://auth.aircall.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aircall
provider_slug: aircall
schemes:
- description: OAuth 2.0 authorization code flow for Aircall Marketplace technology partners.
  flows:
  - authorizationUrl: https://auth.aircall.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.aircall.io/oauth/token
  name: OAuth2
  source: openapi/aircall-openapi.yml
scope_count: 1
scope_names:
- public_api
scopes:
- description: Access to the Aircall Public API
  flows:
  - authorizationCode
  scope: public_api
slug: aircall-scopes
source_filename: aircall-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aircall-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/aircall-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.aircall.io/oauth/authorize\n    tokenUrl: https://auth.aircall.io/oauth/token\n  description: OAuth 2.0 authorization code flow for Aircall Marketplace technology partners.\nscopes:\n- scope: public_api\n  description: Access to the Aircall Public API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aircall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aircall/refs/heads/main/scopes/aircall-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Communications
- Voice
- Cloud Phone
- CRM
- Sales
token_urls:
- https://auth.aircall.io/oauth/token
---
