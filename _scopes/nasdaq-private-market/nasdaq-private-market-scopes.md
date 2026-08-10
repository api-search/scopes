---
authorization_urls:
- https://fe.login.secondmarket.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Nasdaq Private Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nasdaq Private Market publishes 7 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nasdaq Private Market API on a user''s behalf.


  Tokens are issued from https://fe.login.secondmarket.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nasdaq Private Market
provider_slug: nasdaq-private-market
schemes:
- flows:
  - authorizationUrl: https://fe.login.secondmarket.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://fe.login.secondmarket.com/oauth2/v1/token
  - authorizationUrl: https://fe.login.secondmarket.com/oauth2/v1/authorize
    flow: implicit
  name: NPM Platform OIDC (Okta)
  source: well-known/nasdaq-private-market-openid-configuration.json
scope_count: 7
scope_names:
- openid
- email
- profile
- address
- phone
- offline_access
- groups
scopes:
- description: Request an OpenID Connect ID token for the signed-in platform user.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Access to the user's email address and email_verified claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Access to basic profile claims (name, given_name, family_name, locale, picture, updated_at).
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Access to the user's address claim.
  flows:
  - authorizationCode
  - implicit
  scope: address
- description: Access to the user's phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Issue a refresh token so the client can renew access without user interaction.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access to the user's group memberships on the platform identity tenant.
  flows:
  - authorizationCode
  - implicit
  scope: groups
slug: nasdaq-private-market-scopes
source_filename: nasdaq-private-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://fe.login.secondmarket.com/.well-known/openid-configuration\nnotes: 'Nasdaq Private Market publishes no OAuth scope reference for its data or trading\n  APIs. The scopes recorded here are the ones actually advertised by the platform identity\n  host (an Okta tenant) in its live discovery documents. The OIDC scopes are standard\n  OpenID Connect identity scopes; the RFC 8414 document additionally advertises Okta''s\n  own org-management scope set (okta.*), which governs administration of the identity\n  tenant and is NOT an NPM business API scope surface. No scope maps to Tape D, NPM\n  Price, or any other NPM data product.'\nschemes:\n- name: NPM Platform OIDC (Okta)\n  source: well-known/nasdaq-private-market-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fe.login.secondmarket.com/oauth2/v1/authorize\n    tokenUrl: https://fe.login.secondmarket.com/oauth2/v1/token\n \
  \ - flow: implicit\n    authorizationUrl: https://fe.login.secondmarket.com/oauth2/v1/authorize\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for the signed-in platform user.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\n- scope: email\n  description: Access to the user's email address and email_verified claim.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\n- scope: profile\n  description: Access to basic profile claims (name, given_name, family_name, locale,\n    picture, updated_at).\n  flows: [authorizationCode, implicit]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\n- scope: address\n  description: Access to the user's address claim.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\n- scope: phone\n  description: Access to the user's\
  \ phone_number and phone_number_verified claims.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without user interaction.\n  flows: [authorizationCode]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\n- scope: groups\n  description: Access to the user's group memberships on the platform identity tenant.\n  flows: [authorizationCode, implicit]\n  sources: [well-known/nasdaq-private-market-openid-configuration.json]\nidentity_platform_scopes:\n  note: 'Advertised by /.well-known/oauth-authorization-server — Okta org-management\n    scopes for administering the identity tenant itself. Recorded for completeness;\n    these are not Nasdaq Private Market API scopes.'\n  source: well-known/nasdaq-private-market-oauth-authorization-server.json\n  count: 60+\n  examples:\n  - okta.users.read\n  - okta.users.manage\n\
  \  - okta.groups.read\n  - okta.apps.read\n  - okta.policies.manage\n  - okta.logs.read\n  - okta.sessions.manage\ngaps:\n- No scope or permission reference is published for the Tape D API or any NPM data\n  product.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-private-market/refs/heads/main/scopes/nasdaq-private-market-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit
tags:
- Company
- Private Markets
- Secondary Markets
- Market Data
- Financial Services
- Valuations
- Pre-IPO Equity
- Capital Markets
token_urls:
- https://fe.login.secondmarket.com/oauth2/v1/token
---
