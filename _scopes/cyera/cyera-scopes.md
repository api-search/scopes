---
authorization_urls:
- https://auth.cyera.io/oauth/authorize
description: ''
docs: https://support.cyera.io/hc/en-us
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cyera Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cyera publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cyera API on a user''s behalf.


  Tokens are issued from https://auth.cyera.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cyera
provider_slug: cyera
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.cyera.io/oauth/token
  - authorizationUrl: https://auth.cyera.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.cyera.io/oauth/token
  name: OAuth2
  source: https://auth.cyera.io/.well-known/openid-configuration
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - clientCredentials
  - authorizationCode
  scope: openid
- description: Access to the authenticated principal's basic profile claims.
  flows:
  - clientCredentials
  - authorizationCode
  scope: profile
- description: Access to the authenticated principal's email claim.
  flows:
  - clientCredentials
  - authorizationCode
  scope: email
slug: cyera-scopes
source_filename: cyera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.cyera.io/.well-known/openid-configuration\ndocs: https://support.cyera.io/hc/en-us\nschemes:\n- name: OAuth2\n  source: https://auth.cyera.io/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cyera.io/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cyera.io/oauth/authorize\n    tokenUrl: https://auth.cyera.io/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [clientCredentials, authorizationCode]\n  sources: [https://auth.cyera.io/.well-known/openid-configuration]\n- scope: profile\n  description: Access to the authenticated principal's basic profile claims.\n  flows: [clientCredentials, authorizationCode]\n  sources: [https://auth.cyera.io/.well-known/openid-configuration]\n- scope: email\n  description: Access to the authenticated principal's email claim.\n  flows: [clientCredentials,\
  \ authorizationCode]\n  sources: [https://auth.cyera.io/.well-known/openid-configuration]\nnotes: >-\n  Only the OIDC-standard scopes (openid, profile, email) are advertised by the\n  authorization server's discovery document. Fine-grained data-access\n  authorization in Cyera is enforced by tenant/role rather than by additional\n  OAuth scopes advertised at the discovery endpoint; the API's resource-level\n  permission reference is behind the authenticated developer portal\n  (api.cyera.io/docs).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyera/refs/heads/main/scopes/cyera-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Company
- Cybersecurity
- Data Security
- DSPM
- Data Security Posture Management
- Data Classification
- Cloud Security
- Compliance
- MCP
- AI Security
token_urls:
- https://auth.cyera.io/oauth/token
---
