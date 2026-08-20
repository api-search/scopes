---
api_specs:
- filename: steadfast-group-flood-risk-tracker-openapi.yml
  format: yaml
  label: Steadfast Flood Risk Tracker API
  slug: flood-risk-tracker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/openapi/steadfast-group-flood-risk-tracker-openapi.yml
authorization_urls:
- https://idp.steadfast.com.au/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- deviceCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Steadfast Group Scopes
name_suffix: OAuth Scopes
note: Scopes are read from the anonymously-published OpenID Connect discovery document of Steadfast Group's Okta identity provider. Steadfast publishes no scopes or permissions reference page - this is the complete advertised scope set for the tenant's default authorization server, not a documented API permission model. The public Flood Risk Tracker API uses no OAuth and therefore has no scopes.
overview: 'Steadfast Group publishes 7 OAuth 2.0 scopes via the authorizationCode, implicit, deviceCode, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Steadfast Group API on a user''s behalf.


  Tokens are issued from https://idp.steadfast.com.au/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Steadfast Group
provider_slug: steadfast-group
schemes:
- flows:
  - authorizationUrl: https://idp.steadfast.com.au/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://idp.steadfast.com.au/oauth2/v1/token
  - authorizationUrl: https://idp.steadfast.com.au/oauth2/v1/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://idp.steadfast.com.au/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://idp.steadfast.com.au/oauth2/v1/token
  - flow: password
    tokenUrl: https://idp.steadfast.com.au/oauth2/v1/token
  issuer: https://idp.steadfast.com.au
  name: SteadfastIdP
  source: well-known/steadfast-group-openid-configuration.json
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
- description: Required to obtain an ID token; identifies the request as an OpenID Connect request.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: openid
- description: Access to the end user's default profile claims - name, family_name, given_name, middle_name, nickname, preferred_username, picture, website, gender, birthdate, zoneinfo, locale, updated_at.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: profile
- description: Access to the end user's email and email_verified claims.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: email
- description: Access to the end user's address claim.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: address
- description: Access to the end user's phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: phone
- description: Requests a refresh token so the client can obtain new access tokens without user interaction.
  flows:
  - authorizationCode
  - deviceCode
  - password
  scope: offline_access
- description: Okta-specific scope returning the end user's group memberships as a claim. In a broker network this is the likely carrier of brokerage/role entitlement, though no documentation confirms how Steadfast populates it.
  flows:
  - authorizationCode
  - implicit
  - deviceCode
  - password
  scope: groups
slug: steadfast-group-scopes
source_filename: steadfast-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://idp.steadfast.com.au/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Scopes are read from the anonymously-published OpenID Connect discovery document of Steadfast\n  Group's Okta identity provider. Steadfast publishes no scopes or permissions reference page -\n  this is the complete advertised scope set for the tenant's default authorization server, not a\n  documented API permission model. The public Flood Risk Tracker API uses no OAuth and therefore\n  has no scopes.\nschemes:\n  - name: SteadfastIdP\n    type: openIdConnect\n    issuer: https://idp.steadfast.com.au\n    source: well-known/steadfast-group-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://idp.steadfast.com.au/oauth2/v1/authorize\n        tokenUrl: https://idp.steadfast.com.au/oauth2/v1/token\n      - flow: implicit\n        authorizationUrl: https://idp.steadfast.com.au/oauth2/v1/authorize\n\
  \      - flow: deviceCode\n        deviceAuthorizationUrl: https://idp.steadfast.com.au/oauth2/v1/device/authorize\n        tokenUrl: https://idp.steadfast.com.au/oauth2/v1/token\n      - flow: password\n        tokenUrl: https://idp.steadfast.com.au/oauth2/v1/token\nscopes:\n  - scope: openid\n    description: Required to obtain an ID token; identifies the request as an OpenID Connect request.\n    standard: OpenID Connect Core 1.0\n    flows: [authorizationCode, implicit, deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\n  - scope: profile\n    description: >-\n      Access to the end user's default profile claims - name, family_name, given_name,\n      middle_name, nickname, preferred_username, picture, website, gender, birthdate, zoneinfo,\n      locale, updated_at.\n    standard: OpenID Connect Core 1.0\n    flows: [authorizationCode, implicit, deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\n  -\
  \ scope: email\n    description: Access to the end user's email and email_verified claims.\n    standard: OpenID Connect Core 1.0\n    flows: [authorizationCode, implicit, deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\n  - scope: address\n    description: Access to the end user's address claim.\n    standard: OpenID Connect Core 1.0\n    flows: [authorizationCode, implicit, deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\n  - scope: phone\n    description: Access to the end user's phone_number and phone_number_verified claims.\n    standard: OpenID Connect Core 1.0\n    flows: [authorizationCode, implicit, deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\n  - scope: offline_access\n    description: Requests a refresh token so the client can obtain new access tokens without user interaction.\n    standard: OpenID Connect Core 1.0\n    flows: [authorizationCode,\
  \ deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\n  - scope: groups\n    description: >-\n      Okta-specific scope returning the end user's group memberships as a claim. In a broker\n      network this is the likely carrier of brokerage/role entitlement, though no documentation\n      confirms how Steadfast populates it.\n    standard: Okta extension\n    flows: [authorizationCode, implicit, deviceCode, password]\n    sources: [well-known/steadfast-group-openid-configuration.json]\nclaims_supported:\n  - iss\n  - ver\n  - sub\n  - aud\n  - iat\n  - exp\n  - jti\n  - auth_time\n  - amr\n  - idp\n  - nonce\n  - name\n  - nickname\n  - preferred_username\n  - given_name\n  - middle_name\n  - family_name\n  - email\n  - email_verified\n  - profile\n  - zoneinfo\n  - locale\n  - address\n  - phone_number\n  - picture\n  - website\n  - gender\n  - birthdate\n  - updated_at\n  - at_hash\n  - c_hash\ngaps:\n  - >-\n    No business/domain scopes (quote,\
  \ bind, policy, claim) are advertised on the default\n    authorization server. Any partner-facing API scopes would live on a custom Okta\n    authorization server whose discovery path is not publicly enumerable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steadfast-group/refs/heads/main/scopes/steadfast-group-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit/deviceCode/password
tags:
- Insurance
- Australia
- Brokers
- Insurance Broker Network
- General Insurance
- Property and Casualty
- Underwriting Agency
- Agency Management
- ACORD
- Partner Gated
- New Zealand
token_urls:
- https://idp.steadfast.com.au/oauth2/v1/token
---
