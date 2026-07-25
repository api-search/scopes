---
authorization_urls:
- https://api.ctfs.com:443/auth/oauth/v2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Canadian Tire Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Canadian Tire Bank publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canadian Tire Bank API on a user''s behalf.


  Tokens are issued from https://api.ctfs.com:443/auth/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canadian Tire Bank
provider_slug: canadian-tire-bank
schemes:
- flows:
  - authorizationUrl: https://api.ctfs.com:443/auth/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://api.ctfs.com:443/auth/oauth/v2/token
  issuer: https://api.ctfs.com
  name: openIdConnect
  source: well-known/canadian-tire-bank-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- profile
- openid_client_registration
scopes:
- description: Authenticate the end user and issue an ID token (OpenID Connect core scope).
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Release the end user's email address claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Release the end user's basic profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Permit dynamic OpenID Connect client registration (RFC 7591) against the registration endpoint.
  flows:
  - authorizationCode
  scope: openid_client_registration
slug: canadian-tire-bank-scopes
source_filename: canadian-tire-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.ctfs.com/.well-known/openid-configuration\nnotes: >-\n  Scopes are taken verbatim from scopes_supported in the bank's published OpenID\n  Connect discovery document. These are standard OIDC login scopes plus a dynamic\n  client-registration scope — a consumer identity surface, not a banking-data API\n  scope set.\nschemes:\n- name: openIdConnect\n  source: well-known/canadian-tire-bank-openid-configuration.json\n  issuer: https://api.ctfs.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.ctfs.com:443/auth/oauth/v2/authorize\n    tokenUrl: https://api.ctfs.com:443/auth/oauth/v2/token\nscopes:\n- scope: openid\n  description: Authenticate the end user and issue an ID token (OpenID Connect core scope).\n  flows: [authorizationCode, implicit]\n  sources: [well-known/canadian-tire-bank-openid-configuration.json]\n- scope: email\n  description: Release the end user's email address claim.\n\
  \  flows: [authorizationCode, implicit]\n  sources: [well-known/canadian-tire-bank-openid-configuration.json]\n- scope: profile\n  description: Release the end user's basic profile claims.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/canadian-tire-bank-openid-configuration.json]\n- scope: openid_client_registration\n  description: Permit dynamic OpenID Connect client registration (RFC 7591) against the registration endpoint.\n  flows: [authorizationCode]\n  sources: [well-known/canadian-tire-bank-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-tire-bank/refs/heads/main/scopes/canadian-tire-bank-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Credit Cards
- Mastercard
- Consumer-Driven Banking
- Data Aggregation
token_urls:
- https://api.ctfs.com:443/auth/oauth/v2/token
---
