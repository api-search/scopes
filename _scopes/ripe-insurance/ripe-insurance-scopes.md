---
api_specs:
- filename: ripe-insurance-umbraco-content-delivery-openapi.json
  format: json
  label: Ripe Insurance Umbraco Content Delivery API
  slug: ripe-insurance-umbraco-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-umbraco-content-delivery-openapi.json
- filename: ripe-insurance-cycleplan-content-delivery-openapi.json
  format: json
  label: Cycleplan Umbraco Content Delivery API
  slug: ripe-insurance-cycleplan-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-cycleplan-content-delivery-openapi.json
authorization_urls:
- https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/authorize
description: ''
docs: https://docs.umbraco.com/umbraco-cms/reference/content-delivery-api#protected-content
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Ripe Insurance Scopes
name_suffix: OAuth Scopes
note: Neither harvested OpenAPI declares an oauth2 securityScheme, so the mechanical derivation (0-working/derive-oauth-scopes.py) returned nothing. The scopes below were read from the live OpenID Connect discovery document published by the Umbraco (OpenIddict) member-authentication server. This is the WEBSITE CUSTOMER LOGIN scope surface, not a partner or developer API scope surface — Ripe publishes no developer scopes because it publishes no developer API. Recorded because it is real and anonymously readable.
overview: 'Ripe Insurance publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ripe Insurance API on a user''s behalf.


  Tokens are issued from https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ripe Insurance
provider_slug: ripe-insurance
schemes:
- flows:
  - authorizationUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token
  - flow: clientCredentials
    tokenUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token
  - flow: refreshToken
    tokenUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token
  issuer: https://www.ripeinsurance.co.uk/
  name: umbraco-member-oidc
  source: well-known/ripe-insurance-openid-configuration.json
  type: openIdConnect
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: 'Standard OpenID Connect scope. Requests an ID token identifying the authenticated Ripe Insurance website member (claims: aud, exp, iat, iss, sub).'
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token so the member session can be renewed without re-authentication.
  flows:
  - authorizationCode
  scope: offline_access
slug: ripe-insurance-scopes
source_filename: ripe-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://www.ripeinsurance.co.uk/.well-known/openid-configuration (fetched 2026-07-25)\ndocs: https://docs.umbraco.com/umbraco-cms/reference/content-delivery-api#protected-content\nnote: >-\n  Neither harvested OpenAPI declares an oauth2 securityScheme, so the mechanical\n  derivation (0-working/derive-oauth-scopes.py) returned nothing. The scopes below were\n  read from the live OpenID Connect discovery document published by the Umbraco\n  (OpenIddict) member-authentication server. This is the WEBSITE CUSTOMER LOGIN scope\n  surface, not a partner or developer API scope surface — Ripe publishes no developer\n  scopes because it publishes no developer API. Recorded because it is real and\n  anonymously readable.\nschemes:\n- name: umbraco-member-oidc\n  type: openIdConnect\n  source: well-known/ripe-insurance-openid-configuration.json\n  issuer: https://www.ripeinsurance.co.uk/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token\n    pkce: [S256, plain]\n  - flow: clientCredentials\n    tokenUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token\n  - flow: refreshToken\n    tokenUrl: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope. Requests an ID token identifying the authenticated\n    Ripe Insurance website member (claims: aud, exp, iat, iss, sub).\n  flows: [authorizationCode]\n  sources: [well-known/ripe-insurance-openid-configuration.json]\n  standard: OpenID Connect Core 1.0\n- scope: offline_access\n  description: >-\n    Requests a refresh token so the member session can be renewed without\n    re-authentication.\n  flows: [authorizationCode]\n  sources: [well-known/ripe-insurance-openid-configuration.json]\n\
  \  standard: OpenID Connect Core 1.0\ncoverage:\n  scopes_total: 2\n  vendor_standard: 2\n  provider_specific: 0\n  note: >-\n    Zero provider-specific scopes. Every scope advertised is an unmodified OpenID\n    Connect standard scope emitted by the CMS default configuration — there is no\n    resource-scoped permission model (no read:policy, no quote:create, nothing\n    insurance-shaped) because no insurance API is exposed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/scopes/ripe-insurance-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Insurance
- United Kingdom
- Insurtech
- Managing General Agent
- Specialist Insurance
- Personal Lines
- Small Business Insurance
- Underwriting
- Direct to Consumer
- Brokers
token_urls:
- https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token
---
