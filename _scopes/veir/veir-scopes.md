---
authorization_urls:
- https://veir.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Veir Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VEIR publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the VEIR API on a user''s behalf.


  Tokens are issued from https://veir.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VEIR
provider_slug: veir
schemes:
- flows:
  - authorizationUrl: https://veir.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://veir.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://veir.com/oauth/token
  issuer: https://veir.com
  name: OpenIDConnect
  source: well-known/veir-openid-configuration.json
scope_count: 3
scope_names:
- openid
- profile
- read
scopes:
- description: OpenID Connect subject identifier. Declared in scopes_supported.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims. Declared in scopes_supported.
  flows:
  - authorizationCode
  scope: profile
- description: Read access. Declared in scopes_supported; the resource it reads is not documented publicly.
  flows:
  - authorizationCode
  - clientCredentials
  scope: read
slug: veir-scopes
source_filename: veir-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://veir.com/.well-known/openid-configuration\ndocs: null\nschemes:\n- name: OpenIDConnect\n  source: well-known/veir-openid-configuration.json\n  issuer: https://veir.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://veir.com/oauth/authorize\n    tokenUrl: https://veir.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://veir.com/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect subject identifier. Declared in scopes_supported.\n  flows: [authorizationCode]\n  sources: [well-known/veir-openid-configuration.json, well-known/veir-oauth-protected-resource.json]\n- scope: profile\n  description: Basic profile claims. Declared in scopes_supported.\n  flows: [authorizationCode]\n  sources: [well-known/veir-openid-configuration.json, well-known/veir-oauth-protected-resource.json]\n- scope: read\n  description: Read access. Declared in scopes_supported; the resource it\
  \ reads is not documented publicly.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/veir-openid-configuration.json, well-known/veir-oauth-protected-resource.json]\ncaveats:\n- >-\n  These three scopes are the provider's own published scopes_supported values, recorded verbatim.\n  VEIR publishes no scopes/permissions reference page, and the authorization and token endpoints\n  the discovery document names both returned 404 on 2026-08-05, so no scope could be exercised.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://veir.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veir/refs/heads/main/scopes/veir-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Energy
- Electricity
- Data Centers
- Infrastructure
- Superconductors
- Content
token_urls:
- https://veir.com/oauth/token
---
