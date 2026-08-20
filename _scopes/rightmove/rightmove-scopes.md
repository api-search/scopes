---
api_specs:
- filename: rightmove-commercial-listings-openapi.yml
  format: yaml
  label: Rightmove Commercial Listings API
  slug: rightmove-commercial-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightmove/refs/heads/main/openapi/rightmove-commercial-listings-openapi.yml
authorization_urls:
- /oauth/token
description: ''
docs: https://api-docs.rightmove.co.uk/authentication
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Rightmove Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rightmove publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rightmove API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rightmove
provider_slug: rightmove
schemes:
- description: This API uses OAuth2 client credentials flow for server to server authentication
  flows:
  - authorizationUrl: /oauth/token
    flow: implicit
    note: Declared flow does not match the documented grant — see authentication/rightmove-authentication.yml for the defect note.
    scopes: {}
  grant_documented: client_credentials
  name: OAuth2
  source: openapi/rightmove-commercial-listings-openapi.yml
  token_url: /oauth/token
scope_count: 1
scope_names:
- client Grants read and write access
scopes:
- description: 'Appears as the sole entry in the security requirement of getCommercialPropertiesByBranch (security: [{OAuth2: ["client Grants read and write access"]}]). It is a concatenation of a scope name and its description that was never split, and no scopes map declares it. Do not send it as a scope parameter.'
  flows: []
  scope: client Grants read and write access
slug: rightmove-scopes
source_filename: rightmove-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/rightmove-commercial-listings-openapi.yml\ndocs: https://api-docs.rightmove.co.uk/authentication\nsummary: >-\n  Rightmove does NOT operate an OAuth scope model. The portal authentication page\n  states that scopes \"are not currently required or implemented\", and the\n  securityScheme in the published OpenAPI carries an empty scopes map. The single\n  entry below is not a real scope — it is a malformed free-text string that leaked\n  into the `security` requirement of one operation, recorded verbatim rather than\n  dressed up as a permission model.\nscopes_implemented: false\nschemes:\n- name: OAuth2\n  source: openapi/rightmove-commercial-listings-openapi.yml\n  grant_documented: client_credentials\n  token_url: /oauth/token\n  flows:\n  - flow: implicit\n    authorizationUrl: /oauth/token\n    scopes: {}\n    note: >-\n      Declared flow does not match the documented grant — see\n      authentication/rightmove-authentication.yml\
  \ for the defect note.\n  description: This API uses OAuth2 client credentials flow for server to server authentication\nscopes:\n- scope: client Grants read and write access\n  real_scope: false\n  description: >-\n    Appears as the sole entry in the security requirement of\n    getCommercialPropertiesByBranch (security: [{OAuth2: [\"client Grants read and\n    write access\"]}]). It is a concatenation of a scope name and its description\n    that was never split, and no scopes map declares it. Do not send it as a scope\n    parameter.\n  operations: [getCommercialPropertiesByBranch]\n  sources:\n  - openapi/rightmove-commercial-listings-openapi.yml\nauthorization_model:\n  actual: >-\n    Authorization is entitlement-based, not scope-based. A ClientId/ClientKey pair\n    is bound by Rightmove to specific agents and branches; calling outside that\n    entitlement returns 403. The Real Time Data Feed enforces the same idea with\n    Network_ID and Branch_ID carried in the payload.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightmove/refs/heads/main/scopes/rightmove-scopes.yml
summary_line: 1 scope · implicit
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Commercial Real Estate
- Data Feed
token_urls: []
---
