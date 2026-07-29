---
authorization_urls:
- https://id.syd.com.au:443/am/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sydney Airport Scopes
name_suffix: OAuth Scopes
note: Derived from the scopes_supported array of the ForgeRock Access Management OpenID Connect Discovery document at https://id.syd.com.au/am/oauth2/.well-known/openid-configuration (HTTP 200, harvested 2026-07-28), plus the scope string observed on the live InfoSYD authorize redirect. Sydney Airport publishes no scope or permission reference page - these are the values the identity provider itself advertises, not documented product scopes.
overview: 'Sydney Airport publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sydney Airport API on a user''s behalf.


  Tokens are issued from https://id.syd.com.au:443/am/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sydney Airport
provider_slug: sydney-airport
schemes:
- flows:
  - authorizationUrl: https://id.syd.com.au:443/am/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token
  issuer: https://id.syd.com.au:443/am/oauth2
  name: SYDOAuth2
  source: authentication/sydney-airport-openid-configuration.json
scope_count: 8
scope_names:
- openid
- profile
- email
- address
- phone
- fr:idm:*
- am-introspect-all-tokens
- infosyd
scopes:
- description: OpenID Connect authentication; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect profile claims for the authenticated partner user.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OpenID Connect email claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OpenID Connect address claim.
  flows:
  - authorizationCode
  scope: address
- description: Standard OpenID Connect phone_number claims.
  flows:
  - authorizationCode
  scope: phone
- description: ForgeRock Identity Management platform scope advertised by the realm. Vendor-default, not a Sydney Airport product scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: fr:idm:*
- description: ForgeRock Access Management scope permitting introspection of all tokens. Vendor-default administrative scope.
  flows:
  - clientCredentials
  scope: am-introspect-all-tokens
- description: Application scope for the InfoSYD airline / ground-handler / on-airport-tenant portal. Not present in scopes_supported; observed on the live authorize request issued by client_id INFOSYD_APP_Client.
  flows:
  - authorizationCode
  scope: infosyd
slug: sydney-airport-scopes
source_filename: sydney-airport-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: authentication/sydney-airport-openid-configuration.json\ndocs: null\nnote: >-\n  Derived from the scopes_supported array of the ForgeRock Access Management\n  OpenID Connect Discovery document at https://id.syd.com.au/am/oauth2/.well-known/openid-configuration\n  (HTTP 200, harvested 2026-07-28), plus the scope string observed on the live\n  InfoSYD authorize redirect. Sydney Airport publishes no scope or permission\n  reference page - these are the values the identity provider itself advertises,\n  not documented product scopes.\nschemes:\n- name: SYDOAuth2\n  source: authentication/sydney-airport-openid-configuration.json\n  issuer: https://id.syd.com.au:443/am/oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.syd.com.au:443/am/oauth2/authorize\n    tokenUrl: https://id.syd.com.au:443/am/oauth2/access_token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; requests an ID\
  \ token.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: true\n- scope: profile\n  description: Standard OpenID Connect profile claims for the authenticated partner\n    user.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: true\n- scope: email\n  description: Standard OpenID Connect email claims.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: true\n- scope: address\n  description: Standard OpenID Connect address claim.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: false\n- scope: phone\n  description: Standard\
  \ OpenID Connect phone_number claims.\n  standard: OpenID Connect Core 1.0\n  flows: [authorizationCode]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: false\n- scope: fr:idm:*\n  description: ForgeRock Identity Management platform scope advertised by the realm.\n    Vendor-default, not a Sydney Airport product scope.\n  standard: ForgeRock platform\n  flows: [authorizationCode, clientCredentials]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: false\n- scope: am-introspect-all-tokens\n  description: ForgeRock Access Management scope permitting introspection of all tokens.\n    Vendor-default administrative scope.\n  standard: ForgeRock platform\n  flows: [clientCredentials]\n  sources: [authentication/sydney-airport-openid-configuration.json]\n  observed_in_infosyd_request: false\n- scope: infosyd\n  description: Application scope for the InfoSYD airline / ground-handler / on-airport-tenant\n\
  \    portal. Not present in scopes_supported; observed on the live authorize request\n    issued by client_id INFOSYD_APP_Client.\n  standard: null\n  flows: [authorizationCode]\n  sources: ['observed: https://www.sydneyairport.com.au/infosyd authorize redirect,\n      2026-07-28']\n  observed_in_infosyd_request: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sydney-airport/refs/heads/main/scopes/sydney-airport-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Travel
- Australia
- Airports
- Aviation
- Airport Infrastructure
- Transportation
- Flight Information
- Passenger Experience
token_urls:
- https://id.syd.com.au:443/am/oauth2/access_token
---
