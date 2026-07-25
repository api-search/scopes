---
authorization_urls:
- https://login.talpartner.tal.com.au/oauth2/v1/authorize
- https://auth.acp.tal.com.au/oauth2/v1/authorize
- https://auth.claimsassist.tal.com.au/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Tal Australia Scopes
name_suffix: OAuth Scopes
note: TAL declares no OpenAPI, so these scopes come straight from the scopes_supported arrays of TAL's three live OpenID Connect discovery documents. They are the standard OIDC scope set — TAL publishes no business-domain scopes (no quote, policy, claim or underwriting scopes are advertised anonymously). Any partner-specific scopes live on custom Okta authorization servers that are not discoverable without a client.
overview: 'TAL publishes 7 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the TAL API on a user''s behalf.


  Tokens are issued from https://login.talpartner.tal.com.au/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TAL
provider_slug: tal-australia
schemes:
- flows:
  - authorizationUrl: https://login.talpartner.tal.com.au/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.talpartner.tal.com.au/oauth2/v1/token
  - deviceAuthorizationUrl: https://login.talpartner.tal.com.au/oauth2/v1/device/authorize
    flow: deviceCode
    tokenUrl: https://login.talpartner.tal.com.au/oauth2/v1/token
  issuer: https://login.talpartner.tal.com.au
  name: talpartner-oidc
  source: well-known/tal-australia-talpartner-openid-configuration.json
- flows:
  - authorizationUrl: https://auth.acp.tal.com.au/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://auth.acp.tal.com.au/oauth2/v1/token
  issuer: https://auth.acp.tal.com.au
  name: acp-oidc
  source: well-known/tal-australia-acp-openid-configuration.json
- flows:
  - authorizationUrl: https://auth.claimsassist.tal.com.au/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://auth.claimsassist.tal.com.au/oauth2/v1/token
  issuer: https://auth.claimsassist.tal.com.au
  name: claimsassist-oidc
  source: well-known/tal-australia-claimsassist-openid-configuration.json
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
- description: Request an ID token and authenticate the end user (OpenID Connect core).
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, preferred_username, locale, zoneinfo, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: address claim.
  flows:
  - authorizationCode
  scope: address
- description: phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Issue a refresh token so the partner application can act without the user present.
  flows:
  - authorizationCode
  scope: offline_access
- description: Group membership claim — the mechanism TAL's Okta tenants use to carry partner/role entitlement into the token.
  flows:
  - authorizationCode
  scope: groups
slug: tal-australia-scopes
source_filename: tal-australia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://login.talpartner.tal.com.au/.well-known/openid-configuration\ndocs: null\nnote: |\n  TAL declares no OpenAPI, so these scopes come straight from the\n  scopes_supported arrays of TAL's three live OpenID Connect discovery\n  documents. They are the standard OIDC scope set — TAL publishes no\n  business-domain scopes (no quote, policy, claim or underwriting scopes are\n  advertised anonymously). Any partner-specific scopes live on custom Okta\n  authorization servers that are not discoverable without a client.\nschemes:\n- name: talpartner-oidc\n  source: well-known/tal-australia-talpartner-openid-configuration.json\n  issuer: https://login.talpartner.tal.com.au\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.talpartner.tal.com.au/oauth2/v1/authorize\n    tokenUrl: https://login.talpartner.tal.com.au/oauth2/v1/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.talpartner.tal.com.au/oauth2/v1/device/authorize\n\
  \    tokenUrl: https://login.talpartner.tal.com.au/oauth2/v1/token\n- name: acp-oidc\n  source: well-known/tal-australia-acp-openid-configuration.json\n  issuer: https://auth.acp.tal.com.au\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.acp.tal.com.au/oauth2/v1/authorize\n    tokenUrl: https://auth.acp.tal.com.au/oauth2/v1/token\n- name: claimsassist-oidc\n  source: well-known/tal-australia-claimsassist-openid-configuration.json\n  issuer: https://auth.claimsassist.tal.com.au\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.claimsassist.tal.com.au/oauth2/v1/authorize\n    tokenUrl: https://auth.claimsassist.tal.com.au/oauth2/v1/token\nscopes:\n- scope: openid\n  description: Request an ID token and authenticate the end user (OpenID Connect\n    core).\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n\
  - scope: profile\n  description: Basic profile claims (name, given_name, family_name, preferred_username,\n    locale, zoneinfo, updated_at).\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n- scope: email\n  description: email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n- scope: address\n  description: address claim.\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n- scope: phone\n  description: phone_number\
  \ and phone_number_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the partner application can act without\n    the user present.\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n- scope: groups\n  description: Group membership claim — the mechanism TAL's Okta tenants use to\n    carry partner/role entitlement into the token.\n  flows: [authorizationCode]\n  sources: [well-known/tal-australia-talpartner-openid-configuration.json,\n    well-known/tal-australia-acp-openid-configuration.json,\n    well-known/tal-australia-claimsassist-openid-configuration.json]\n\
  gaps:\n- No business-domain scopes (quote / policy / claim / underwriting / member) are\n  published on any anonymously reachable authorization server.\n- The Okta stock \"default\" authorization server at\n  https://talpartner-au.okta.com/oauth2/default advertises only Okta platform\n  scopes (okta.myAccount.*, okta.users.*), which are vendor scopes rather than\n  TAL API scopes, so they are deliberately not listed here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tal-australia/refs/heads/main/scopes/tal-australia-scopes.yml
summary_line: 7 scopes · authorizationCode/deviceCode
tags:
- Insurance
- Australia
- Life Insurance
- Income Protection
- Group Insurance
- Superannuation
- Underwriting
- Claims
- Carrier
- Embedded Insurance
- Partner Gated
- No Public API
- OpenID Connect
- GraphQL
- Identity
token_urls:
- https://login.talpartner.tal.com.au/oauth2/v1/token
- https://auth.acp.tal.com.au/oauth2/v1/token
- https://auth.claimsassist.tal.com.au/oauth2/v1/token
---
