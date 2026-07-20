---
api_specs:
- filename: autopass-openapi.yml
  format: yaml
  label: Autopass Service Authorization API
  slug: autopass-service-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autopass/refs/heads/main/openapi/autopass-openapi.yml
authorization_urls:
- https://api.autopass.xyz/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Autopass Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Autopass publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Autopass API on a user''s behalf.


  Tokens are issued from https://api.autopass.xyz/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Autopass
provider_slug: autopass
schemes:
- flows:
  - authorizationUrl: https://api.autopass.xyz/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.autopass.xyz/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.autopass.xyz/oauth/token
  name: autopassOAuth
  source: https://api.autopass.xyz/.well-known/openid-configuration
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication. Grants identity claims (sub, email, email_verified, phone_number, phone_number_verified) via the userinfo endpoint and ID token.
  flows:
  - authorizationCode
  scope: openid
slug: autopass-scopes
source_filename: autopass-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.autopass.xyz/.well-known/openid-configuration\nschemes:\n  - name: autopassOAuth\n    source: https://api.autopass.xyz/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.autopass.xyz/oauth/authorize\n        tokenUrl: https://api.autopass.xyz/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://api.autopass.xyz/oauth/token\nscopes:\n  - scope: openid\n    description: >-\n      OpenID Connect authentication. Grants identity claims (sub, email, email_verified,\n      phone_number, phone_number_verified) via the userinfo endpoint and ID token.\n    flows: [authorizationCode]\n    sources: [https://api.autopass.xyz/.well-known/openid-configuration]\nnotes: >-\n  scopes_supported in the published OIDC discovery lists only \"openid\". Autopass does not\n  document additional resource scopes; partner authorization to the /pois, /site-sessions\n\
  \  and /orders resources is governed at the client/partner level rather than by OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopass/refs/heads/main/scopes/autopass-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Mobility
- Parking
- Payments
- Automotive
- Financial Services
- OAuth
- Taiwan
token_urls:
- https://api.autopass.xyz/oauth/token
---
