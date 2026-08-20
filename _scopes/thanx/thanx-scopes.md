---
api_specs:
- filename: thanx-account-api-openapi.yml
  format: yaml
  label: Thanx Account API
  slug: thanx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-account-api-openapi.yml
- filename: thanx-auth-api-openapi.yml
  format: yaml
  label: Thanx Auth API
  slug: thanx-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-auth-api-openapi.yml
- filename: thanx-baskets-api-openapi.yml
  format: yaml
  label: Thanx Baskets API
  slug: thanx-baskets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-baskets-api-openapi.yml
- filename: thanx-campaigns-api-openapi.yml
  format: yaml
  label: Thanx Campaigns API
  slug: thanx-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-campaigns-api-openapi.yml
- filename: thanx-cards-api-openapi.yml
  format: yaml
  label: Thanx Cards API
  slug: thanx-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-cards-api-openapi.yml
- filename: thanx-gift-cards-api-openapi.yml
  format: yaml
  label: Thanx Gift Cards API
  slug: thanx-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-gift-cards-api-openapi.yml
- filename: thanx-issuance-jobs-api-openapi.yml
  format: yaml
  label: Thanx Issuance Jobs API
  slug: thanx-issuance-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-issuance-jobs-api-openapi.yml
- filename: thanx-locations-api-openapi.yml
  format: yaml
  label: Thanx Locations API
  slug: thanx-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-locations-api-openapi.yml
- filename: thanx-metadata-api-openapi.yml
  format: yaml
  label: Thanx Metadata API
  slug: thanx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-metadata-api-openapi.yml
- filename: thanx-points-api-openapi.yml
  format: yaml
  label: Thanx Points API
  slug: thanx-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-points-api-openapi.yml
- filename: thanx-purchases-api-openapi.yml
  format: yaml
  label: Thanx Purchases API
  slug: thanx-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-purchases-api-openapi.yml
- filename: thanx-rewards-api-openapi.yml
  format: yaml
  label: Thanx Rewards API
  slug: thanx-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-rewards-api-openapi.yml
- filename: thanx-subscribers-api-openapi.yml
  format: yaml
  label: Thanx Subscribers API
  slug: thanx-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-subscribers-api-openapi.yml
- filename: thanx-users-api-openapi.yml
  format: yaml
  label: Thanx Users API
  slug: thanx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/openapi/thanx-users-api-openapi.yml
authorization_urls: []
description: 'Thanx''s Partner API is scope-limited: each API credential is provisioned with an agreed-upon set of scopes granting access to a subset of endpoints, and every Partner endpoint page names the scope it requires. The scopes are NOT declared in an OpenAPI oauth2 securityScheme — running derive-oauth-scopes.py against openapi/ found zero oauth2 schemes and therefore zero scopes — so this catalog is read from the documentation, endpoint by endpoint. Scopes are introspectable at runtime: GET /partner/scopes returns the list the calling credential holds.'
docs: https://docs.thanx.com/partner/metadata/get-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Thanx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Thanx uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thanx
provider_slug: thanx
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: thanx-scopes
source_filename: thanx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://docs.thanx.com/partner/metadata/get-scopes\nsource: >-\n  Read from the \"Scope required\" callout published on every Partner API endpoint page across\n  https://docs.thanx.com (Auth, Campaigns, Feedbacks, Issuance Jobs, Promotions, Purchases,\n  Reward Templates, Subscribers, Tags, Users), plus\n  https://docs.thanx.com/partner/overview (scope model) and\n  https://docs.thanx.com/consumer/sso/overview (consumer OAuth scope).\ndescription: >-\n  Thanx's Partner API is scope-limited: each API credential is provisioned with an agreed-upon\n  set of scopes granting access to a subset of endpoints, and every Partner endpoint page names\n  the scope it requires. The scopes are NOT declared in an OpenAPI oauth2 securityScheme —\n  running derive-oauth-scopes.py against openapi/ found zero oauth2 schemes and therefore zero\n  scopes — so this catalog is read from the documentation, endpoint by endpoint. Scopes are\n  introspectable\
  \ at runtime: GET /partner/scopes returns the list the calling credential holds.\nmodel:\n  grant: Assigned by Thanx per API credential during partnership onboarding; not self-serve.\n  introspection:\n    operation: getScopes\n    path: GET /partner/scopes\n    returns: '{\"scopes\": [\"subscribers.write\"]}'\n    docs: https://docs.thanx.com/partner/metadata/get-scopes\n  naming: '<resource>.<action> — read / write, plus the resource-specific issue and create verbs'\n  enforcement_status: 403 Forbidden when the credential lacks the required scope\n  consumer_api: >-\n    The Consumer API does not use these scopes. Thanx SSO issues user access tokens through the\n    OAuth 2.0 authorization code grant with the scope value \"passwordless\"; authorization is by\n    user identity, not by scope.\nscopes:\n  - name: auth.create\n    description: Mint privileged end-user access tokens on behalf of a merchant's users.\n    operations: [createToken]\n    endpoints: ['POST /partner/oauth/token']\n\
  \    docs: https://docs.thanx.com/partner/auth/create-token\n  - name: rewards.issue\n    description: >-\n      Create and read campaigns and reward templates, and issue or revoke rewards against a\n      campaign variant. The broadest Partner scope — it spans the whole issuance flow.\n    operations: [createCampaign, listCampaigns, getCampaign, issueRewards, getIssuanceJob, revokeIssuanceJob]\n    endpoints:\n      - 'POST /partner/campaigns'\n      - 'GET /partner/campaigns'\n      - 'GET /partner/campaigns/{id}'\n      - 'POST /partner/campaigns/issue'\n      - 'GET /partner/issuance_jobs/{id}'\n      - 'POST /partner/issuance_jobs/{id}/revoke'\n      - 'GET /partner/reward_templates'\n      - 'GET /partner/reward_templates/{id}'\n    docs: https://docs.thanx.com/partner/campaigns/issue-rewards\n  - name: subscribers.write\n    description: Ingest subscribers (email/SMS marketing opt-ins) for a merchant.\n    operations: [createSubscriber]\n    endpoints: ['POST /partner/subscribers']\n\
  \    docs: https://docs.thanx.com/partner/subscribers/create-subscriber\n  - name: purchases.write\n    description: Submit purchases to Thanx for processing so loyalty points accrue.\n    operations: [createPurchase]\n    endpoints: ['POST /partner/purchases']\n    docs: https://docs.thanx.com/partner/purchases/create-purchase\n  - name: users.read\n    description: Read the users of a merchant, individually or as a collection.\n    operations: [getPartnerUser, getPartnerUsers]\n    endpoints: ['GET /partner/users', 'GET /partner/users/{id}']\n    docs: https://docs.thanx.com/partner/users/get-users\n  - name: users.write\n    description: Update a merchant's user records.\n    operations: []\n    endpoints: ['PUT /partner/users/{id}']\n    docs: https://docs.thanx.com/partner/users/update-user\n    note: Documented endpoint not yet captured in openapi/.\n  - name: tags.read\n    description: Read attribute tags on a merchant's users.\n    operations: []\n    endpoints: ['GET /partner/tags']\n\
  \    docs: https://docs.thanx.com/partner/tags/get-tags\n    note: Documented endpoint not yet captured in openapi/.\n  - name: tags.write\n    description: Create, update and delete attribute tags.\n    operations: []\n    endpoints: ['PUT /partner/tags', 'DELETE /partner/tags']\n    docs: https://docs.thanx.com/partner/tags/upsert-tags\n    note: Documented endpoints not yet captured in openapi/.\n  - name: feedbacks.read\n    description: Read guest feedback records for a merchant.\n    operations: []\n    endpoints: ['GET /partner/feedbacks']\n    docs: https://docs.thanx.com/partner/feedbacks/get-feedbacks\n    note: Documented endpoint not yet captured in openapi/.\n  - name: feedbacks.write\n    description: Respond to a guest feedback record.\n    operations: []\n    endpoints: ['POST /partner/feedbacks/{id}/response']\n    docs: https://docs.thanx.com/partner/feedbacks/feedback-response\n    note: Documented endpoint not yet captured in openapi/.\n  - name: promos.read\n    description:\
  \ Read promotions and the codes in a promotion's active pool.\n    operations: []\n    endpoints: ['GET /partner/promotions', 'GET /partner/promotions/{id}', 'GET /partner/promotions/{id}/codes']\n    docs: https://docs.thanx.com/partner/promotions/overview\n    note: Documented endpoints not yet captured in openapi/.\n  - name: promos.write\n    description: Create promotions and generate batches of single-use promotion codes.\n    operations: []\n    endpoints: ['POST /partner/promotions', 'POST /partner/promotions/{id}/codes']\n    docs: https://docs.thanx.com/partner/promotions/create-promotion\n    note: >-\n      Documented endpoints not yet captured in openapi/. Both accept X-Idempotency-Key — see\n      conventions/thanx-conventions.yml.\nconsumer_oauth:\n  grant_type: authorization_code\n  spec: RFC 6749 §4.1\n  scope_value: passwordless\n  endpoints:\n    - 'POST /oauth/authorize — passwordless flow, emails an auth code link'\n    - 'POST /oauth/authorize-cross-domain — issues\
  \ a code for an already-authenticated user, no email'\n    - 'POST /oauth/token — exchange authorization code for access token'\n    - 'POST /oauth/revoke — revoke an access token'\n  docs: https://docs.thanx.com/consumer/sso/overview\nsummary:\n  scope_count: 12\n  scopes_in_openapi: 0\n  scopes_documented: 12\n  gap: >-\n    Every Partner scope is documented in prose but none is declared in an OpenAPI\n    securityScheme, so no generated client or agent can enforce or discover them from the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thanx/refs/heads/main/scopes/thanx-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Restaurant
- Loyalty
- Guest Engagement
- Marketing
- CRM
- Online Ordering
- Webhook
- Points
- Rewards
- Campaigns
token_urls: []
---
