---
api_specs:
- filename: 1komma5-offer-tool-openapi-original.json
  format: json
  label: 1KOMMA5° Offer Tool API
  slug: 1komma5-offer-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1komma5/refs/heads/main/openapi/1komma5-offer-tool-openapi-original.json
authorization_urls:
- https://auth.1komma5grad.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: 1Komma5 Scopes
name_suffix: OAuth Scopes
note: 1KOMMA5° declares no API scopes in any published OpenAPI (the Offer Tool spec has no securitySchemes at all) and publishes no scopes/permissions reference page. The scopes below are the ones its Auth0 authorization server advertises anonymously in OIDC discovery — standard OIDC/Auth0 identity scopes, not product-resource scopes. No 1KOMMA5°-specific API scope (e.g. read:sites, write:systems) is publicly discoverable.
overview: '1KOMMA5° publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1KOMMA5° API on a user''s behalf.


  Tokens are issued from https://auth.1komma5grad.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1KOMMA5°
provider_slug: 1komma5
schemes:
- flows:
  - authorizationUrl: https://auth.1komma5grad.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.1komma5grad.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.1komma5grad.com/oauth/token
  - deviceAuthorizationUrl: https://auth.1komma5grad.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.1komma5grad.com/oauth/token
  issuer: https://auth.1komma5grad.com/
  name: auth0-oidc
  source: well-known/1komma5-openid-configuration.json
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
- description: Issue an OIDC ID token for the authenticated end user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token so the client can renew access without re-prompting.
  flows:
  - authorizationCode
  scope: offline_access
- description: The end user's full name claim.
  flows:
  - authorizationCode
  scope: name
- description: The end user's given name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: The end user's family name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: The end user's nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: The end user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Whether the end user's email address has been verified.
  flows:
  - authorizationCode
  scope: email_verified
- description: The end user's profile picture URL claim.
  flows:
  - authorizationCode
  scope: picture
- description: Auth0 account creation timestamp claim.
  flows:
  - authorizationCode
  scope: created_at
- description: Auth0 linked-identity records for the end user.
  flows:
  - authorizationCode
  scope: identities
- description: The end user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: The end user's address claim.
  flows:
  - authorizationCode
  scope: address
slug: 1komma5-scopes
source_filename: 1komma5-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://auth.1komma5grad.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  1KOMMA5° declares no API scopes in any published OpenAPI (the Offer Tool spec has no\n  securitySchemes at all) and publishes no scopes/permissions reference page. The scopes\n  below are the ones its Auth0 authorization server advertises anonymously in OIDC\n  discovery — standard OIDC/Auth0 identity scopes, not product-resource scopes. No\n  1KOMMA5°-specific API scope (e.g. read:sites, write:systems) is publicly discoverable.\nschemes:\n- name: auth0-oidc\n  source: well-known/1komma5-openid-configuration.json\n  issuer: https://auth.1komma5grad.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.1komma5grad.com/authorize\n    tokenUrl: https://auth.1komma5grad.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.1komma5grad.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl:\
  \ https://auth.1komma5grad.com/oauth/device/code\n    tokenUrl: https://auth.1komma5grad.com/oauth/token\nscopes:\n- scope: openid\n  description: Issue an OIDC ID token for the authenticated end user.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture).\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without re-prompting.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: name\n  description: The end user's full name claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: given_name\n  description: The end user's given name claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n\
  - scope: family_name\n  description: The end user's family name claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: nickname\n  description: The end user's nickname claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: email\n  description: The end user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: email_verified\n  description: Whether the end user's email address has been verified.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: picture\n  description: The end user's profile picture URL claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: created_at\n  description: Auth0 account creation timestamp claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: identities\n\
  \  description: Auth0 linked-identity records for the end user.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: phone\n  description: The end user's phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\n- scope: address\n  description: The end user's address claim.\n  flows: [authorizationCode]\n  sources: [well-known/1komma5-openid-configuration.json]\ncoverage:\n  scopes_total: 14\n  product_resource_scopes: 0\n  identity_scopes: 14\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://auth.1komma5grad.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1komma5/refs/heads/main/scopes/1komma5-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Energy
- Solar
- Renewable Energy
- Smart Home
- Electric Vehicles
- Heat Pumps
- Virtual Power Plant
- Energy Management
- Germany
token_urls:
- https://auth.1komma5grad.com/oauth/token
---
