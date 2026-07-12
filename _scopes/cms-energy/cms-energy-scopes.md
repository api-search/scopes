---
authorization_urls:
- https://utilityapi.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cms Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CMS Energy publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CMS Energy API on a user''s behalf.


  Tokens are issued from https://utilityapi.com/api/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CMS Energy
provider_slug: cms-energy
schemes:
- flows:
  - authorizationUrl: https://utilityapi.com/authorize
    flow: authorizationCode
    tokenUrl: https://utilityapi.com/api/v2/oauth/token
  name: oauth2
  source: openapi/cms-energy-openapi.yml
scope_count: 1
scope_names:
- auth-sso
scopes:
- description: Production single-sign-on scope (Consumers Energy)
  flows:
  - authorizationCode
  scope: auth-sso
slug: cms-energy-scopes
source_filename: cms-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cms-energy-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cms-energy-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://utilityapi.com/authorize\n    tokenUrl: https://utilityapi.com/api/v2/oauth/token\nscopes:\n- scope: auth-sso\n  description: Production single-sign-on scope (Consumers Energy)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cms-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-energy/refs/heads/main/scopes/cms-energy-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Electric
- Energy
- Green Button
- Michigan
- Natural Gas
- Utility
- Fortune 500
token_urls:
- https://utilityapi.com/api/v2/oauth/token
---
