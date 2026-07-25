---
authorization_urls:
- https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Canadian Blue Cross Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blue Cross Canada publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blue Cross Canada API on a user''s behalf.


  Tokens are issued from https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blue Cross Canada
provider_slug: canadian-blue-cross
schemes:
- flows:
  - authorizationUrl: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    tokenUrl: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/token
  issuer: https://pac.bluecross.ca/
  name: pacific-blue-cross-member-oidc
  source: well-known/canadian-blue-cross-pac-openid-configuration.json
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the signed-in Pacific Blue Cross website member.
  flows:
  - authorizationCode
  scope: openid
- description: Requests a refresh token so the member session can be renewed without re-authentication; refresh_token is an advertised grant type.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: canadian-blue-cross-scopes
source_filename: canadian-blue-cross-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://pac.bluecross.ca/.well-known/openid-configuration\ndocs: null\nscope: >-\n  There is no Blue Cross Canada OAuth scope programme. The only published scopes_supported in\n  the federation come from the Pacific Blue Cross Umbraco member authorization server, and they\n  are the two generic OIDC scopes that server advertises. No benefits, claims, eligibility, or\n  policy scopes exist because no such API is published.\nschemes:\n- name: pacific-blue-cross-member-oidc\n  issuer: https://pac.bluecross.ca/\n  source: well-known/canadian-blue-cross-pac-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/token\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope requesting an ID token for the signed-in Pacific\
  \ Blue Cross\n    website member.\n  flows: [authorizationCode]\n  sources: [well-known/canadian-blue-cross-pac-openid-configuration.json]\n- scope: offline_access\n  description: >-\n    Requests a refresh token so the member session can be renewed without re-authentication;\n    refresh_token is an advertised grant type.\n  flows: [authorizationCode, refreshToken]\n  sources: [well-known/canadian-blue-cross-pac-openid-configuration.json]\nabsent:\n  domain_scopes: >-\n    No read/write scopes for claims, benefits, eligibility, providers, groups, or payments are\n    advertised on any host in the federation.\n  other_plans: >-\n    Alberta, Ontario/Quebec, Medavie, Saskatchewan and Manitoba Blue Cross serve no OAuth or\n    OIDC discovery document at all (404/NXDOMAIN), so they contribute no scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-blue-cross/refs/heads/main/scopes/canadian-blue-cross-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Insurance
- Canada
- Health Insurance
- Dental Benefits
- Travel Insurance
- Life Insurance
- Employee Benefits
- Group Benefits
- Claims
- Carrier
- Association
- No Public API
token_urls:
- https://pac.bluecross.ca/umbraco/delivery/api/v1/security/member/token
---
