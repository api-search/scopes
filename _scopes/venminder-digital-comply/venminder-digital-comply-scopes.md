---
api_specs:
- filename: venminder-digital-comply-openapi-original.json
  format: json
  label: Venminder API
  slug: venminder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/venminder-digital-comply/refs/heads/main/openapi/venminder-digital-comply-openapi-original.json
authorization_urls: []
description: ''
docs: https://developers.venminder.com/318218fb2/p/9845ac-the-venminder-apis/b/30923a
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Venminder Digital Comply Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Venminder (Digital Comply) publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Venminder (Digital Comply) API on a user''s behalf.


  Tokens are issued from https://login.venminder.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Venminder (Digital Comply)
provider_slug: venminder-digital-comply
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.venminder.com/connect/token
  name: OAuth2 client credentials
  source: https://login.venminder.com/.well-known/openid-configuration
scope_count: 1
scope_names:
- venminderApi
scopes:
- description: Access to the customer-facing Venminder API (rsd.venminder.com/api/v1 and /scim/v2).
  flows:
  - clientCredentials
  scope: venminderApi
slug: venminder-digital-comply-scopes
source_filename: venminder-digital-comply-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.venminder.com/ (Venminder Token page) + https://login.venminder.com/.well-known/openid-configuration\ndocs: https://developers.venminder.com/318218fb2/p/9845ac-the-venminder-apis/b/30923a\nnotes: 'The customer-facing Venminder API uses the OAuth 2.0 client-credentials grant against the IdentityServer\n  at login.venminder.com with the venminderApi scope (documented curl: grant_type=client_credentials&scope=venminderApi).\n  The OpenAPI itself declares only a Bearer apiKey header scheme, so this scope surface comes from the\n  docs and the OIDC discovery document.'\nschemes:\n- name: OAuth2 client credentials\n  source: https://login.venminder.com/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.venminder.com/connect/token\nscopes:\n- scope: venminderApi\n  description: Access to the customer-facing Venminder API (rsd.venminder.com/api/v1 and /scim/v2).\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - https://developers.venminder.com/ Token page FAQ curl example\nissuer_advertised_scopes:\n  notes: Full scopes_supported list advertised by the login.venminder.com OIDC discovery document; most\n    are internal/partner scopes not offered to API customers.\n  scopes:\n  - openid\n  - profile\n  - venminderUser\n  - internalApi\n  - venminderApi\n  - exchangeApi\n  - controlAssessmentsApi\n  - internalControlAssessmentsApi\n  - internalControlAssessmentsApiClient\n  - riskratings-partners-webapi\n  - venminderFlexBillingApi\n  - offline_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venminder-digital-comply/refs/heads/main/scopes/venminder-digital-comply-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Third-Party Risk Management
- Vendor Management
- Risk
- Compliance
- Contracts
- Financial Services
- Due Diligence
- SCIM
token_urls:
- https://login.venminder.com/connect/token
---
