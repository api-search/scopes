---
authorization_urls:
- https://customers.refectory.fr/oauth2/auth
description: ''
docs: https://customers.refectory.fr/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Dejbox Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the Refectory (Dejbox) OpenID Connect discovery document (scopes_supported). Only the standard OIDC/offline scopes are publicly advertised; no product/resource scope reference page is published.
overview: 'Dejbox (Refectory) publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dejbox (Refectory) API on a user''s behalf.


  Tokens are issued from https://customers.refectory.fr/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dejbox (Refectory)
provider_slug: dejbox
schemes:
- flows:
  - authorizationUrl: https://customers.refectory.fr/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://customers.refectory.fr/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://customers.refectory.fr/oauth2/token
  name: OAuth2
  source: well-known/dejbox-openid-configuration.json
scope_count: 3
scope_names:
- openid
- offline_access
- offline
scopes:
- description: Authenticate the end user and issue an ID token (OpenID Connect).
  flows:
  - authorizationCode
  scope: openid
- description: Request a refresh token for offline (long-lived) access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Legacy offline-access alias advertised by the authorization server.
  flows:
  - authorizationCode
  scope: offline
slug: dejbox-scopes
source_filename: dejbox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://customers.refectory.fr/.well-known/openid-configuration\ndocs: https://customers.refectory.fr/.well-known/openid-configuration\nnote: >-\n  Scopes advertised by the Refectory (Dejbox) OpenID Connect discovery document\n  (scopes_supported). Only the standard OIDC/offline scopes are publicly advertised;\n  no product/resource scope reference page is published.\nschemes:\n- name: OAuth2\n  source: well-known/dejbox-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://customers.refectory.fr/oauth2/auth\n    tokenUrl: https://customers.refectory.fr/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://customers.refectory.fr/oauth2/token\nscopes:\n- scope: openid\n  description: Authenticate the end user and issue an ID token (OpenID Connect).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/dejbox-openid-configuration.json\n- scope: offline_access\n  description:\
  \ Request a refresh token for offline (long-lived) access.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/dejbox-openid-configuration.json\n- scope: offline\n  description: Legacy offline-access alias advertised by the authorization server.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/dejbox-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dejbox/refs/heads/main/scopes/dejbox-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Company
- Food & Agritech
- Corporate Catering
- Food Delivery
- B2B
- France
- Meal Delivery
- OAuth2
- OpenID Connect
token_urls:
- https://customers.refectory.fr/oauth2/token
---
