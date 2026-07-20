---
authorization_urls:
- https://helios.cohesity.com/oauth2/authorize
description: ''
docs: https://developer.cohesity.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cohesity Global Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cohesity Global publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cohesity Global API on a user''s behalf.


  Tokens are issued from https://helios.cohesity.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cohesity Global
provider_slug: cohesity-global
schemes:
- flows:
  - authorizationUrl: https://helios.cohesity.com/oauth2/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    revocationUrl: https://helios.cohesity.com/oauth2/revoke
    tokenUrl: https://helios.cohesity.com/oauth2/token
    token_endpoint_auth:
    - client_secret_basic
  name: HeliosOAuth2
  source: https://helios.cohesity.com/.well-known/openid-configuration
scope_count: 6
scope_names:
- openid
- email
- profile
- cohesity_user
- cohesity_viewer
- cohesity_gaia_viewer
scopes:
- description: OpenID Connect authentication; issue an ID token for the authenticated user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Cohesity user-level access to the Helios API.
  flows:
  - authorizationCode
  scope: cohesity_user
- description: Cohesity read/viewer access to the Helios API.
  flows:
  - authorizationCode
  scope: cohesity_viewer
- description: Cohesity Gaia (AI assistant) viewer access.
  flows:
  - authorizationCode
  scope: cohesity_gaia_viewer
slug: cohesity-global-scopes
source_filename: cohesity-global-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://helios.cohesity.com/.well-known/openid-configuration\ndocs: https://developer.cohesity.com/\nschemes:\n- name: HeliosOAuth2\n  source: https://helios.cohesity.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://helios.cohesity.com/oauth2/authorize\n    tokenUrl: https://helios.cohesity.com/oauth2/token\n    revocationUrl: https://helios.cohesity.com/oauth2/revoke\n    grant_types: [authorization_code, refresh_token]\n    pkce: [S256]\n    token_endpoint_auth: [client_secret_basic]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the authenticated user.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email address claim.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: cohesity_user\n  description:\
  \ Cohesity user-level access to the Helios API.\n  flows: [authorizationCode]\n- scope: cohesity_viewer\n  description: Cohesity read/viewer access to the Helios API.\n  flows: [authorizationCode]\n- scope: cohesity_gaia_viewer\n  description: Cohesity Gaia (AI assistant) viewer access.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cohesity-global/refs/heads/main/scopes/cohesity-global-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Data Security
- Data Management
- Backup and Recovery
- Cyber Resilience
- Data Protection
- Disaster Recovery
- Cloud
token_urls:
- https://helios.cohesity.com/oauth2/token
---
