---
api_specs:
- filename: antavo-events-openapi.yml
  format: yaml
  label: Antavo Events API
  slug: antavo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-events-openapi.yml
- filename: antavo-async-events-openapi.yml
  format: yaml
  label: Antavo Async Events API
  slug: antavo-async-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-async-events-openapi.yml
- filename: antavo-customer-openapi.yml
  format: yaml
  label: Antavo Customer API
  slug: antavo-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-customer-openapi.yml
- filename: antavo-display-openapi.yml
  format: yaml
  label: Antavo Display API
  slug: antavo-display-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-display-openapi.yml
- filename: antavo-entities-openapi.yml
  format: yaml
  label: Antavo Entities API
  slug: antavo-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-entities-openapi.yml
- filename: antavo-rewards-openapi.yml
  format: yaml
  label: Antavo Rewards API
  slug: antavo-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-rewards-openapi.yml
- filename: antavo-coupons-openapi.yml
  format: yaml
  label: Antavo Coupons and Coupon Pools API
  slug: antavo-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-coupons-openapi.yml
- filename: antavo-offers-openapi.yml
  format: yaml
  label: Antavo Offers API
  slug: antavo-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-offers-openapi.yml
- filename: antavo-points-preview-openapi.yml
  format: yaml
  label: Antavo Points Preview API
  slug: antavo-points-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-points-preview-openapi.yml
- filename: antavo-leaderboard-openapi.yml
  format: yaml
  label: Antavo Leaderboard API
  slug: antavo-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-leaderboard-openapi.yml
- filename: antavo-bulk-operations-openapi.yml
  format: yaml
  label: Antavo Bulk Operations API
  slug: antavo-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-bulk-operations-openapi.yml
- filename: antavo-clubs-openapi.yml
  format: yaml
  label: Antavo Clubs API
  slug: antavo-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-clubs-openapi.yml
- filename: antavo-promotion-engine-openapi.yml
  format: yaml
  label: Antavo Promotion Engine API
  slug: antavo-promotion-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-promotion-engine-openapi.yml
- filename: antavo-authentication-openapi.yml
  format: yaml
  label: Antavo Authentication API
  slug: antavo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-authentication-openapi.yml
- filename: antavo-faq-openapi.yml
  format: yaml
  label: Antavo FAQ API
  slug: antavo-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-faq-openapi.yml
- filename: antavo-loyalty-read-openapi.yml
  format: yaml
  label: Antavo Loyalty Read API
  slug: antavo-loyalty-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-loyalty-read-openapi.yml
- filename: antavo-social-share-campaigns-openapi.yml
  format: yaml
  label: Antavo Social Share Campaigns API
  slug: antavo-social-share-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-social-share-campaigns-openapi.yml
authorization_urls: []
description: Antavo's OAuth 2.0 surface is deliberately narrow. Token-based authentication exists on exactly one API today (Async Events) and exactly one scope is supported. The derive-oauth-scopes pass returned nothing because Antavo models the token endpoint as an ordinary operation with a `scope` form field rather than as an OpenAPI `oauth2` securityScheme - the scope is real and documented, but it is invisible to a spec-only scope extraction. This file is written from the token endpoint's own request schema plus the Management UI documentation.
docs: https://docs.antavo.com/docs/api-settings
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Antavo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Antavo publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Antavo API on a user''s behalf.


  Tokens are issued from /v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Antavo
provider_slug: antavo
schemes:
- flows:
  - authorizationUrl: null
    flow: clientCredentials
    note: The base host is per-environment; the published server in the spec is https://api.staging.antavo.com and the production base is https://api.antavo.com.
    tokenUrl: /v1/auth/token
    token_endpoint_auth_method: client_secret_basic
    token_lifetime_seconds:
      maximum: 3600
      minimum: 300
    token_type: Bearer
  name: oauth2-client-credentials
  source: openapi/antavo-authentication-openapi.yml
  spec_representation: Not declared as an OpenAPI oauth2 securityScheme. The token endpoint (POST /v1/auth/token) is secured with `basicAuth` (client_id / client_secret) and takes `grant_type` + `scope` as application/x-www-form-urlencoded fields; protected endpoints then declare `bearerAuth` (http bearer, JWT).
scope_count: 1
scope_names:
- loyalty.async_events
scopes:
- description: Grants access to the Async Events API endpoints (POST /v1/async/events and GET /v1/async/events/{correlation_id}).
  flows:
  - clientCredentials
  scope: loyalty.async_events
slug: antavo-scopes
source_filename: antavo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/antavo-authentication-openapi.yml\ndocs: https://docs.antavo.com/docs/api-settings\ndocs_secondary: https://developers.antavo.com/docs/api-security\ndescription: >-\n  Antavo's OAuth 2.0 surface is deliberately narrow. Token-based authentication\n  exists on exactly one API today (Async Events) and exactly one scope is\n  supported. The derive-oauth-scopes pass returned nothing because Antavo models\n  the token endpoint as an ordinary operation with a `scope` form field rather\n  than as an OpenAPI `oauth2` securityScheme - the scope is real and documented,\n  but it is invisible to a spec-only scope extraction. This file is written from\n  the token endpoint's own request schema plus the Management UI documentation.\nschemes:\n- name: oauth2-client-credentials\n  spec_representation: >-\n    Not declared as an OpenAPI oauth2 securityScheme. The token endpoint\n    (POST /v1/auth/token) is secured with `basicAuth`\
  \ (client_id / client_secret)\n    and takes `grant_type` + `scope` as application/x-www-form-urlencoded fields;\n    protected endpoints then declare `bearerAuth` (http bearer, JWT).\n  source: openapi/antavo-authentication-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\n    authorizationUrl: null\n    token_endpoint_auth_method: client_secret_basic\n    token_type: Bearer\n    token_lifetime_seconds: {minimum: 300, maximum: 3600}\n    note: >-\n      The base host is per-environment; the published server in the spec is\n      https://api.staging.antavo.com and the production base is\n      https://api.antavo.com.\nscopes:\n- scope: loyalty.async_events\n  description: >-\n    Grants access to the Async Events API endpoints\n    (POST /v1/async/events and GET /v1/async/events/{correlation_id}).\n  flows: [clientCredentials]\n  sources:\n  - openapi/antavo-authentication-openapi.yml\n  - https://docs.antavo.com/docs/api-settings\n  evidence: >-\n    Spec:\
  \ `scope` property description reads \"Use `loyalty.async_events` scope to\n    get access to the Async Events API endpoints.\" Management UI: \"Scope -\n    Defines which APIs the generated access tokens can be used for. Currently,\n    only the `loyalty.async_events` scope is supported.\"\nscope_count: 1\ncompleteness:\n  exhaustive: true\n  note: >-\n    Antavo's own documentation states this is the complete set: \"Currently, only\n    the `loyalty.async_events` scope is supported.\" Every other Antavo API is\n    authorised by workspace API key + Escher signature, which has no scope\n    dimension at all - authorisation there is a per-endpoint IP filter and a\n    per-endpoint signature-enforcement toggle in the Management UI, not a scope.\nclient_model:\n  managed_in: Management UI > API settings > Authentication Manager\n  client_attributes: [name, purpose, expiration_date, token_issuer, scope, token_audience]\n  secret_visibility: displayed once at creation, never retrievable afterwards\n\
  \  statuses: [active, revoked, expired]\n  revocation: irreversible\n  audit_log: >-\n    The Authentication Manager records client creation, revocation, and every\n    access token issued or rejected by the token endpoint.\n  source: https://docs.antavo.com/docs/api-settings\nerrors:\n  scope_related:\n  - error: invalid_scope\n    status: 400\n    note: Returned by POST /v1/auth/token in the OAuth error envelope.\n  - error: unauthorized_client\n    status: 400\n  see: errors/antavo-problem-types.yml\ncross_links:\n  authentication: authentication/antavo-authentication.yml\n  conventions: conventions/antavo-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/scopes/antavo-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Loyalty
- Customer Loyalty
- Rewards
- Enterprise
- Headless
- Retail
- Marketing
- Engagement
- Promotions
- Gamification
- Event
- E-Commerce
- Coupons
- Points
- Membership
token_urls:
- /v1/auth/token
---
