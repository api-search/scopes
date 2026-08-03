---
authorization_urls:
- https://deepwatch.okta.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Deepwatch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deepwatch publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deepwatch API on a user''s behalf.


  Tokens are issued from https://deepwatch.okta.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deepwatch
provider_slug: deepwatch
schemes:
- flows:
  - authorizationUrl: https://deepwatch.okta.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://deepwatch.okta.com/oauth2/v1/token
  - authorizationUrl: https://deepwatch.okta.com/oauth2/v1/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://deepwatch.okta.com/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://deepwatch.okta.com/oauth2/v1/token
  issuer: https://deepwatch.okta.com
  name: OktaOIDC
  source: well-known/deepwatch-openid-configuration.json
  type: openIdConnect
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
scopes:
- description: Request an OpenID Connect ID token for the authenticating user.
  flows: []
  scope: openid
- description: Access the user's default profile claims (name, preferred_username, locale, picture and related).
  flows: []
  scope: profile
- description: Access the user's email address and email_verified claim.
  flows: []
  scope: email
- description: Access the user's address claim.
  flows: []
  scope: address
- description: Access the user's phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Request a refresh token so the client can renew access without user interaction.
  flows: []
  scope: offline_access
- description: Okta-specific scope returning the user's group memberships, used for role mapping in the Security Center console.
  flows: []
  scope: groups
slug: deepwatch-scopes
source_filename: deepwatch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://deepwatch.okta.com/.well-known/openid-configuration\ndocs: null\ndocs_note: 'Deepwatch publishes no API scope or permission reference. The scopes below\n  are the OIDC scopes advertised by the org authorization server that fronts the Security\n  Center console — they are standard OpenID Connect scopes plus Okta''s groups scope,\n  not Deepwatch product scopes. No product-level authorization scopes are publicly\n  documented.'\nschemes:\n- name: OktaOIDC\n  type: openIdConnect\n  issuer: https://deepwatch.okta.com\n  source: well-known/deepwatch-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://deepwatch.okta.com/oauth2/v1/authorize\n    tokenUrl: https://deepwatch.okta.com/oauth2/v1/token\n  - flow: implicit\n    authorizationUrl: https://deepwatch.okta.com/oauth2/v1/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://deepwatch.okta.com/oauth2/v1/device/authorize\n\
  \    tokenUrl: https://deepwatch.okta.com/oauth2/v1/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for the authenticating user.\n  standard: true\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n- scope: profile\n  description: Access the user's default profile claims (name, preferred_username,\n    locale, picture and related).\n  standard: true\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n- scope: email\n  description: Access the user's email address and email_verified claim.\n  standard: true\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n- scope: address\n  description: Access the user's address claim.\n  standard: true\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n- scope: phone\n  description: Access the user's phone_number and phone_number_verified claims.\n  standard: true\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n- scope: offline_access\n  description:\
  \ Request a refresh token so the client can renew access without user\n    interaction.\n  standard: true\n  sources:\n  - well-known/deepwatch-openid-configuration.json\n- scope: groups\n  description: Okta-specific scope returning the user's group memberships, used for\n    role mapping in the Security Center console.\n  standard: false\n  vendor: Okta\n  sources:\n  - well-known/deepwatch-openid-configuration.json\nsummary:\n  scope_count: 7\n  product_scopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepwatch/refs/heads/main/scopes/deepwatch-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/deviceCode
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- Security Operations
- Threat Intelligence
- Vulnerability Management
- Managed Security Services
- Agentic AI
token_urls:
- https://deepwatch.okta.com/oauth2/v1/token
---
