---
api_specs:
- filename: wegalvanize-highbond-openapi-original.yml
  format: yaml
  label: HighBond API
  slug: highbond-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wegalvanize/refs/heads/main/openapi/wegalvanize-highbond-openapi-original.yml
authorization_urls: []
description: ''
docs: https://help.highbond.com/helpdocs/highbond/en-us/Default.htm#cshid=lp-access-tokens
flows:
- authorizationCode
- clientCredentials
- implicit
- refreshToken
- tokenExchange
kind: oauth-scopes
layout: scope
method: searched
name: Wegalvanize Scopes
name_suffix: OAuth Scopes
note: 'The published OpenAPI declares a single http-bearer scheme (bearerFormat: oauth2) with no per-operation scope map, so scopes are not derivable from the spec. These scopes are taken verbatim from the HighBond OpenID Connect discovery document (scopes_supported). HighBond API tokens are user-bound and inherit that user''s HighBond permissions rather than being scoped per token.'
overview: 'Wegalvanize publishes 7 OAuth 2.0 scopes via the authorizationCode, clientCredentials, implicit, refreshToken, and tokenExchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wegalvanize API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wegalvanize
provider_slug: wegalvanize
schemes:
- authorization_endpoint: https://oidc.highbond.com/auth
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  - refreshToken
  - tokenExchange
  name: HighBond OIDC (oidc.highbond.com)
  token_endpoint: https://oidc.highbond.com/token
scope_count: 7
scope_names:
- openid
- profile
- email
- membership
- config
- offline_access
- none
scopes:
- description: OpenID Connect authentication; issues an ID token.
  flows: []
  scope: openid
- description: Access to the user's profile claims (name, locale, timezone, org info).
  flows: []
  scope: profile
- description: Access to the user's email claim.
  flows: []
  scope: email
- description: Organization membership / instance association for the user.
  flows: []
  scope: membership
- description: Access to configuration-level claims for the HighBond instance.
  flows: []
  scope: config
- description: Issue a refresh token for continued (offline) access.
  flows: []
  scope: offline_access
- description: Explicit no-scope value supported by the authorization server.
  flows: []
  scope: none
slug: wegalvanize-scopes
source_filename: wegalvanize-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://oidc.highbond.com/.well-known/openid-configuration\ndocs: https://help.highbond.com/helpdocs/highbond/en-us/Default.htm#cshid=lp-access-tokens\nnote: >\n  The published OpenAPI declares a single http-bearer scheme (bearerFormat:\n  oauth2) with no per-operation scope map, so scopes are not derivable from the\n  spec. These scopes are taken verbatim from the HighBond OpenID Connect\n  discovery document (scopes_supported). HighBond API tokens are user-bound and\n  inherit that user's HighBond permissions rather than being scoped per token.\nschemes:\n  - name: HighBond OIDC (oidc.highbond.com)\n    authorization_endpoint: https://oidc.highbond.com/auth\n    token_endpoint: https://oidc.highbond.com/token\n    flows: [authorizationCode, clientCredentials, implicit, refreshToken, tokenExchange]\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issues an ID token.\n  - scope: profile\n    description:\
  \ Access to the user's profile claims (name, locale, timezone, org info).\n  - scope: email\n    description: Access to the user's email claim.\n  - scope: membership\n    description: Organization membership / instance association for the user.\n  - scope: config\n    description: Access to configuration-level claims for the HighBond instance.\n  - scope: offline_access\n    description: Issue a refresh token for continued (offline) access.\n  - scope: none\n    description: Explicit no-scope value supported by the authorization server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wegalvanize/refs/heads/main/scopes/wegalvanize-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials/implicit/refreshToken/tokenExchange
tags:
- Company
- Governance
- Risk
- Compliance
- Audit
- GRC
- Analytics
- Automation
- Security
token_urls: []
---
