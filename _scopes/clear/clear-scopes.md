---
api_specs:
- filename: clear-verification-openapi.json
  format: json
  label: CLEAR1 Verification Sessions API
  slug: clear1-verification-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear/refs/heads/main/openapi/clear-verification-openapi.json
authorization_urls:
- https://verified.clearme.com/integrations/oauth2/auth
description: ''
docs: https://docs.clearme.com/docs/oidc-identity-token
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Clear Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CLEAR publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CLEAR API on a user''s behalf.


  Tokens are issued from https://verified.clearme.com/integrations/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CLEAR
provider_slug: clear
schemes:
- flows:
  - authorizationUrl: https://verified.clearme.com/integrations/oauth2/auth
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://verified.clearme.com/integrations/oauth2/token
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  name: OIDC
  source: https://verified.clearme.com/integrations/.well-known/openid-configuration
  token_endpoint_auth:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
scope_count: 3
scope_names:
- openid
- offline
- offline_access
scopes:
- description: OpenID Connect authentication; returns an identity token with verified member claims
  flows:
  - authorizationCode
  scope: openid
- description: Grants offline access (long-lived) to the verification session
  flows:
  - authorizationCode
  scope: offline
- description: Issues a refresh token for renewing access without user re-interaction
  flows:
  - authorizationCode
  scope: offline_access
slug: clear-scopes
source_filename: clear-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clear-verification-openapi.json\ndocs: https://docs.clearme.com/docs/oidc-identity-token\ndiscovery: well-known/clear-openid-configuration.json\nschemes:\n- name: OIDC\n  source: https://verified.clearme.com/integrations/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://verified.clearme.com/integrations/oauth2/auth\n    tokenUrl: https://verified.clearme.com/integrations/oauth2/token\n    pkce: S256\n  grant_types:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  token_endpoint_auth:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - none\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an identity token with verified member claims\n  flows:\n  - authorizationCode\n- scope: offline\n  description: Grants offline access (long-lived)\
  \ to the verification session\n  flows:\n  - authorizationCode\n- scope: offline_access\n  description: Issues a refresh token for renewing access without user re-interaction\n  flows:\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear/refs/heads/main/scopes/clear-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Identity
- Identity Verification
- Authentication
- KYC
- Biometrics
- OAuth
- OpenID Connect
- Healthcare
- Financial Services
token_urls:
- https://verified.clearme.com/integrations/oauth2/token
---
