---
authorization_urls:
- https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coast Capital Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by the member-authentication OIDC discovery document (scopes_supported). These govern member sign-in / identity, not a public data API. No scope reference page is published in developer docs (there is no public developer portal).
overview: 'Coast Capital Savings publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coast Capital Savings API on a user''s behalf.


  Tokens are issued from https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coast Capital Savings
provider_slug: coast-capital
schemes:
- flows:
  - authorizationUrl: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    tokenUrl: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/token
  name: memberOIDC
  source: well-known/coast-capital-openid-configuration.json
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect authentication; returns an ID token for the signed-in member.
  flows:
  - authorizationCode
  scope: openid
- description: Issues a refresh token so the member session can be renewed without re-authentication.
  flows:
  - authorizationCode
  scope: offline_access
slug: coast-capital-scopes
source_filename: coast-capital-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.coastcapitalsavings.com/.well-known/openid-configuration\nnote: >-\n  Scopes advertised by the member-authentication OIDC discovery document\n  (scopes_supported). These govern member sign-in / identity, not a public\n  data API. No scope reference page is published in developer docs (there is\n  no public developer portal).\nschemes:\n- name: memberOIDC\n  source: well-known/coast-capital-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the signed-in member.\n  flows: [authorizationCode]\n  sources: [well-known/coast-capital-openid-configuration.json]\n- scope: offline_access\n  description: Issues\
  \ a refresh token so the member session can be renewed without re-authentication.\n  flows: [authorizationCode]\n  sources: [well-known/coast-capital-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coast-capital/refs/heads/main/scopes/coast-capital-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Cooperative
- Consumer-Driven Banking
- Data Aggregation
token_urls:
- https://www.coastcapitalsavings.com/umbraco/delivery/api/v1/security/member/token
---
