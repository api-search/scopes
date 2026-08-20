---
authorization_urls:
- https://uniphore.us.auth0.com/authorize
description: ''
docs: https://uniphore.github.io/baic-docs/
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Uniphore Scopes
name_suffix: OAuth Scopes
note: Uniphore publishes no OpenAPI, so no product/API scopes could be derived from oauth2 securitySchemes. The scopes below are the ones actually advertised by Uniphore's dedicated Auth0 identity tenant in its anonymous OIDC discovery document (scopes_supported) — the standard OIDC identity scope set. Any Business AI Cloud resource-server scopes are provisioned per tenant/audience and are not published anonymously; do not assume additional scopes exist.
overview: 'Uniphore publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Uniphore API on a user''s behalf.


  Tokens are issued from https://uniphore.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uniphore
provider_slug: uniphore
schemes:
- flows:
  - authorizationUrl: https://uniphore.us.auth0.com/authorize
    flow: authorizationCode
    tokenUrl: https://uniphore.us.auth0.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://uniphore.us.auth0.com/oauth/token
  - deviceAuthorizationUrl: https://uniphore.us.auth0.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://uniphore.us.auth0.com/oauth/token
  issuer: https://uniphore.us.auth0.com/
  name: openIdConnect
  source: well-known/uniphore-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token and identify the authenticated end user (OIDC core).
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access the end user's default profile claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Issue a refresh token so the client can obtain new access tokens without user interaction.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: Access the end user's full name claim.
  flows:
  - authorizationCode
  scope: name
- description: Access the end user's given name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: Access the end user's family name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: Access the end user's nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: Access the end user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the end user's email verification status claim.
  flows:
  - authorizationCode
  scope: email_verified
- description: Access the end user's profile picture claim.
  flows:
  - authorizationCode
  scope: picture
- description: Access the end user's account creation timestamp claim.
  flows:
  - authorizationCode
  scope: created_at
- description: Access the end user's linked identity providers claim.
  flows:
  - authorizationCode
  scope: identities
- description: Access the end user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Access the end user's postal address claim.
  flows:
  - authorizationCode
  scope: address
slug: uniphore-scopes
source_filename: uniphore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://uniphore.us.auth0.com/.well-known/openid-configuration\ndocs: https://uniphore.github.io/baic-docs/\nnote: >-\n  Uniphore publishes no OpenAPI, so no product/API scopes could be derived from\n  oauth2 securitySchemes. The scopes below are the ones actually advertised by\n  Uniphore's dedicated Auth0 identity tenant in its anonymous OIDC discovery\n  document (scopes_supported) — the standard OIDC identity scope set. Any\n  Business AI Cloud resource-server scopes are provisioned per tenant/audience\n  and are not published anonymously; do not assume additional scopes exist.\nschemes:\n- name: openIdConnect\n  source: well-known/uniphore-openid-configuration.json\n  issuer: https://uniphore.us.auth0.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://uniphore.us.auth0.com/authorize\n    tokenUrl: https://uniphore.us.auth0.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://uniphore.us.auth0.com/oauth/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://uniphore.us.auth0.com/oauth/device/code\n    tokenUrl: https://uniphore.us.auth0.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token and identify the authenticated end user (OIDC core).\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: profile\n  description: Access the end user's default profile claims.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without user interaction.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: name\n  description: Access the end user's full name claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: given_name\n  description: Access the end\
  \ user's given name claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: family_name\n  description: Access the end user's family name claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: nickname\n  description: Access the end user's nickname claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: email\n  description: Access the end user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: email_verified\n  description: Access the end user's email verification status claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: picture\n  description: Access the end user's profile picture claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: created_at\n  description:\
  \ Access the end user's account creation timestamp claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: identities\n  description: Access the end user's linked identity providers claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: phone\n  description: Access the end user's phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\n- scope: address\n  description: Access the end user's postal address claim.\n  flows: [authorizationCode]\n  sources: [well-known/uniphore-openid-configuration.json]\nx-evidence:\n- url: https://uniphore.us.auth0.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniphore/refs/heads/main/scopes/uniphore-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Artificial Intelligence
- Agents
- Conversational AI
- Customer Data Platform
- Contact Center
- Machine-Learning
- Large Language Models
- Enterprise Software
- Automation
- Customer Experience
- Knowledge-Management
token_urls:
- https://uniphore.us.auth0.com/oauth/token
---
