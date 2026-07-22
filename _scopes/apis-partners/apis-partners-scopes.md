---
authorization_urls:
- https://www.apis.pe/umbraco/delivery/api/v1/security/member/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Apis Partners Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the Umbraco Delivery API member OIDC discovery document at apis.pe. This is the CMS member-auth surface, not a business API of Apis Partners.
overview: 'Apis Partners publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apis Partners API on a user''s behalf.


  Tokens are issued from https://www.apis.pe/umbraco/delivery/api/v1/security/member/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apis Partners
provider_slug: apis-partners
schemes:
- flows:
  - authorizationUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    tokenUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token
  name: oauth2
  source: well-known/apis-partners-openid-configuration.json
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the member.
  flows:
  - authorizationCode
  scope: openid
- description: Issues a refresh token so the client can obtain new access tokens without re-authentication.
  flows:
  - authorizationCode
  scope: offline_access
slug: apis-partners-scopes
source_filename: apis-partners-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://apis.pe/.well-known/openid-configuration\nnote: >-\n  Scopes advertised by the Umbraco Delivery API member OIDC discovery document at apis.pe.\n  This is the CMS member-auth surface, not a business API of Apis Partners.\nschemes:\n- name: oauth2\n  source: well-known/apis-partners-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://www.apis.pe/umbraco/delivery/api/v1/security/member/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the member.\n  flows: [authorizationCode]\n  sources: [well-known/apis-partners-openid-configuration.json]\n- scope: offline_access\n  description: Issues a refresh token so the client can obtain new access tokens without re-authentication.\n  flows: [authorizationCode]\n  sources: [well-known/apis-partners-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-partners/refs/heads/main/scopes/apis-partners-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Venture
- Private Equity
- Fintech
- Financial Services
- Payments
- Investor
- Emerging Markets
token_urls:
- https://www.apis.pe/umbraco/delivery/api/v1/security/member/token
---
