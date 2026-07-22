---
api_specs:
- filename: luminary-openapi-original.yml
  format: yaml
  label: Luminary API
  slug: luminary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminary/refs/heads/main/openapi/luminary-openapi-original.yml
authorization_urls:
- https://auth.withluminary.com/oauth2/authorize
description: ''
docs: https://api.withluminary.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Luminary Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Luminary publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Luminary API on a user''s behalf.


  Tokens are issued from https://auth.withluminary.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Luminary
provider_slug: luminary
schemes:
- flows:
  - authorizationUrl: https://auth.withluminary.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.withluminary.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://auth.withluminary.com/oauth2/token
  name: oauth2Profiles
  source: openapi/luminary-openapi-original.yml
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the authenticated user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the authenticated user's email address claim.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access without re-consent.
  flows: []
  scope: offline_access
slug: luminary-scopes
source_filename: luminary-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/luminary-openapi-original.yml\ndocs: https://api.withluminary.com/.well-known/oauth-authorization-server\nschemes:\n- name: oauth2Profiles\n  source: openapi/luminary-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.withluminary.com/oauth2/authorize\n    tokenUrl: https://auth.withluminary.com/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.withluminary.com/oauth2/token\n# The OpenAPI oauth2Profiles scheme declares empty scope maps (API access is\n# governed per-profile, not per-scope). The scopes below are the OIDC/OAuth\n# scopes advertised by the authorization server discovery documents\n# (scopes_supported in /.well-known/oauth-authorization-server).\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  sources: [https://auth.withluminary.com/.well-known/openid-configuration]\n- scope: profile\n  description:\
  \ Access to the authenticated user's basic profile claims.\n  sources: [https://auth.withluminary.com/.well-known/openid-configuration]\n- scope: email\n  description: Access to the authenticated user's email address claim.\n  sources: [https://auth.withluminary.com/.well-known/openid-configuration]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access without re-consent.\n  sources: [https://auth.withluminary.com/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminary/refs/heads/main/scopes/luminary-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Estate Planning
- Wealth Management
- Financial Services
- Legal Tech
- Document AI
- Family Office
- OAuth2
token_urls:
- https://auth.withluminary.com/oauth2/token
---
