---
api_specs:
- filename: goodlord-referencing-api-openapi.json
  format: json
  label: Goodlord Referencing API
  slug: goodlord-referencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-referencing-api-openapi.json
- filename: goodlord-referencing-api-sandbox-openapi.json
  format: json
  label: Goodlord Referencing API (Sandbox)
  slug: goodlord-referencing-api-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-referencing-api-sandbox-openapi.json
- filename: goodlord-insurance-app-api-openapi.json
  format: json
  label: Goodlord Insurance App API
  slug: goodlord-insurance-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/openapi/goodlord-insurance-app-api-openapi.json
authorization_urls: []
description: ''
docs: https://portal.goodlord.co/portal/catalogue-products/referencing-product-1
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Goodlord Scopes
name_suffix: OAuth Scopes
note: Goodlord publishes no scopes or permissions reference page. The OpenAPI declares an OAuth 2.0 clientCredentials flow with an EMPTY scopes object in both the live and sandbox documents, so a client cannot discover any scope from the contract. The two scopes below are taken verbatim from the example token response Goodlord publishes in its own Authentication walkthrough, where the granted scope string is "free_plan referencing_product". They are observed at runtime, not declared — nothing else is asserted about them, and no request-time scope parameter is documented.
overview: 'Goodlord publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Goodlord API on a user''s behalf.


  Tokens are issued from https://api.goodoverlord.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Goodlord
provider_slug: goodlord
schemes:
- api: Goodlord Referencing API
  description: 'This API uses OAuth2 to authenticate requests. You must use your client credentials to obtain a token.

    Read [Obtain a JWT Token](./operations/getAuthToken) for more information.'
  flows:
  - declared_scopes: {}
    flow: clientCredentials
    tokenUrl: https://api.goodoverlord.com/auth/token
  name: OAuth2
  source: openapi/goodlord-referencing-api-openapi.json
- api: Goodlord Referencing API (Sandbox)
  description: 'This API uses OAuth2 to authenticate requests. You must use your client credentials to obtain a token.

    Read [Obtain a JWT Token](./operations/getAuthToken) for more information.'
  flows:
  - declared_scopes: {}
    flow: clientCredentials
    tokenUrl: https://api-sandbox.goodlord.co/auth/token
  name: OAuth2
  source: openapi/goodlord-referencing-api-sandbox-openapi.json
scope_count: 2
scope_names:
- free_plan
- referencing_product
scopes:
- description: Observed in the granted scope string of the documented example token response. Reads as a plan/entitlement marker rather than a resource permission. Goodlord publishes no definition, and no other plan value has been observed.
  flows:
  - clientCredentials
  scope: free_plan
- description: Observed in the granted scope string of the documented example token response. Grants access to the Referencing product surface. Product-level rather than operation-level — no read/write or per-resource split is published.
  flows:
  - clientCredentials
  scope: referencing_product
slug: goodlord-scopes
source_filename: goodlord-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/goodlord-referencing-api-openapi.json, openapi/goodlord-referencing-api-sandbox-openapi.json\ndocs: https://portal.goodlord.co/portal/catalogue-products/referencing-product-1\nnote: >-\n  Goodlord publishes no scopes or permissions reference page. The OpenAPI declares an OAuth 2.0\n  clientCredentials flow with an EMPTY scopes object in both the live and sandbox documents, so\n  a client cannot discover any scope from the contract. The two scopes below are taken verbatim\n  from the example token response Goodlord publishes in its own Authentication walkthrough,\n  where the granted scope string is \"free_plan referencing_product\". They are observed at\n  runtime, not declared — nothing else is asserted about them, and no request-time scope\n  parameter is documented.\nschemes:\n- name: OAuth2\n  source: openapi/goodlord-referencing-api-openapi.json\n  api: Goodlord Referencing API\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://api.goodoverlord.com/auth/token\n    declared_scopes: {}\n  description: |-\n    This API uses OAuth2 to authenticate requests. You must use your client credentials to obtain a token.\n    Read [Obtain a JWT Token](./operations/getAuthToken) for more information.\n- name: OAuth2\n  source: openapi/goodlord-referencing-api-sandbox-openapi.json\n  api: Goodlord Referencing API (Sandbox)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.goodlord.co/auth/token\n    declared_scopes: {}\n  description: |-\n    This API uses OAuth2 to authenticate requests. You must use your client credentials to obtain a token.\n    Read [Obtain a JWT Token](./operations/getAuthToken) for more information.\nscopes:\n- scope: free_plan\n  description: >-\n    Observed in the granted scope string of the documented example token response. Reads as a\n    plan/entitlement marker rather than a resource permission. Goodlord publishes no\n    definition, and no other plan\
  \ value has been observed.\n  flows: [clientCredentials]\n  observed_at_runtime: true\n  declared_in_spec: false\n  sources: [https://portal.goodlord.co/portal/catalogue-products/referencing-product-1]\n- scope: referencing_product\n  description: >-\n    Observed in the granted scope string of the documented example token response. Grants\n    access to the Referencing product surface. Product-level rather than operation-level —\n    no read/write or per-resource split is published.\n  flows: [clientCredentials]\n  observed_at_runtime: true\n  declared_in_spec: false\n  sources: [https://portal.goodlord.co/portal/catalogue-products/referencing-product-1]\ntenant_scoping:\n  mechanism: Company-ID request header\n  note: >-\n    The real access boundary on this API is not the OAuth scope, it is the issued Company-ID\n    header carried on every request. Scope selects the product; Company-ID selects the letting\n    agency whose data you can see. The header is documented only in the portal\
  \ and is not\n    declared anywhere in the OpenAPI.\nnot_applicable:\n- api: Goodlord Insurance App API\n  reason: >-\n    Declares a single JWT bearer scheme modelled as apiKey with no OAuth flow, no token\n    endpoint and no scope surface. Authorisation is enforced by the agent's roles and role\n    groups (GET /api/v1/roles, /api/v1/role_groups) rather than by token scopes.\nend_user_platform:\n  issuer: https://login.goodlord.co/7ddbafdc-ee33-46fb-968a-3011e2a0a825/v2.0/\n  scopes_supported: [openid]\n  resource_scope_prefix: https://vouchauth.onmicrosoft.com/gl-api\n  source: well-known/goodlord-openid-configuration.json\n  note: >-\n    The Azure AD B2C discovery document for the letting-agent and tenant platform login\n    advertises only the openid scope. This is the end-user login, not the developer API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodlord/refs/heads/main/scopes/goodlord-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Real Estate
- United Kingdom
- PropTech
- Property Management
- Rentals
- Lettings
- Tenant Referencing
- Tenancy Management
- Insurance
- Payments
token_urls:
- https://api.goodoverlord.com/auth/token
- https://api-sandbox.goodlord.co/auth/token
---
