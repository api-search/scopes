---
api_specs:
- filename: google-ads-ad-groups-api-openapi.yml
  format: yaml
  label: Google Ads Ad Groups API
  slug: google-ads-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-ad-groups-api-openapi.yml
- filename: google-ads-ads-api-openapi.yml
  format: yaml
  label: Google Ads Ads API
  slug: google-ads-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-ads-api-openapi.yml
- filename: google-ads-bidding-strategies-api-openapi.yml
  format: yaml
  label: Google Ads Bidding Strategies API
  slug: google-ads-bidding-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-bidding-strategies-api-openapi.yml
- filename: google-ads-campaigns-api-openapi.yml
  format: yaml
  label: Google Ads Campaigns API
  slug: google-ads-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-campaigns-api-openapi.yml
- filename: google-ads-customers-api-openapi.yml
  format: yaml
  label: Google Ads Customers API
  slug: google-ads-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-customers-api-openapi.yml
- filename: google-ads-keywords-api-openapi.yml
  format: yaml
  label: Google Ads Keywords API
  slug: google-ads-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-keywords-api-openapi.yml
- filename: google-ads-reporting-api-openapi.yml
  format: yaml
  label: Google Ads Reporting API
  slug: google-ads-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-reporting-api-openapi.yml
- filename: google-ads-api-v25-openapi.yml
  format: yaml
  label: Google Ads API
  slug: google-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/openapi/google-ads-api-v25-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: 'The Google Ads API has exactly ONE OAuth scope, and it is all-or-nothing. There is no read-only scope, no per-resource scope, and no way for a user to grant an application reporting access without also granting it the ability to change campaigns and spend. For anyone delegating this API to an agent, that is the single most important fact on this page: least privilege is not expressible in the token. It has to be enforced outside it — by the tools you expose, by the customer IDs you allow, and by review before mutate.'
docs: https://developers.google.com/google-ads/api/docs/oauth/overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Ads Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Ads publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Ads API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Ads
provider_slug: google-ads
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  note: The per-resource v18 specs in openapi/ declare the same single scope with the older https://accounts.google.com/o/oauth2/auth authorization URL. The OIDC discovery document at accounts.google.com names /o/oauth2/v2/auth as current.
  source: discovery/google-ads-api-v25-discovery.json
  type: oauth2
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/adwords
scopes:
- description: See, edit, create, and delete your Google Ads accounts and data.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/adwords
slug: google-ads-scopes
source_filename: google-ads-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://googleads.googleapis.com/$discovery/rest?version=v25 (auth.oauth2.scopes, read\n  live 2026-08-13) and https://developers.google.com/google-ads/api/docs/oauth/overview\ndocs: https://developers.google.com/google-ads/api/docs/oauth/overview\nprovider: Google Ads\nproviderId: google-ads\ndescription: >-\n  The Google Ads API has exactly ONE OAuth scope, and it is all-or-nothing. There is no\n  read-only scope, no per-resource scope, and no way for a user to grant an application\n  reporting access without also granting it the ability to change campaigns and spend.\n  For anyone delegating this API to an agent, that is the single most important fact on\n  this page: least privilege is not expressible in the token. It has to be enforced\n  outside it — by the tools you expose, by the customer IDs you allow, and by review\n  before mutate.\nscope_count: 1\nschemes:\n  - name: oauth2\n    type: oauth2\n    source: discovery/google-ads-api-v25-discovery.json\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n    note: >-\n      The per-resource v18 specs in openapi/ declare the same single scope with the older\n      https://accounts.google.com/o/oauth2/auth authorization URL. The OIDC discovery\n      document at accounts.google.com names /o/oauth2/v2/auth as current.\nscopes:\n  - scope: https://www.googleapis.com/auth/adwords\n    description: See, edit, create, and delete your Google Ads accounts and data.\n    grants:\n      - read\n      - write\n      - delete\n    flows:\n      - authorizationCode\n    applies_to: every one of the 174 operations in the v25 surface\n    sources:\n      - discovery/google-ads-api-v25-discovery.json\n      - openapi/google-ads-api-v25-openapi.yml\n    note: >-\n      Description is Google's own wording from the discovery document's auth block, not a\n      paraphrase.\nadditional_credentials:\n\
  \  - name: developer-token\n    kind: header\n    required: true\n    note: >-\n      Not an OAuth scope, but the second half of authorization on this API. Its access\n      level (Test / Explorer / Basic / Standard) determines the daily operation quota. A\n      valid OAuth token with the adwords scope still fails against production accounts if\n      the developer token is at Test access.\n    docs: https://developers.google.com/google-ads/api/docs/access-levels\n  - name: login-customer-id\n    kind: header\n    required: conditional\n    note: Required when acting on a client account through a manager account.\n  - name: linked-customer-id\n    kind: header\n    required: conditional\n    note: Used by third-party app analytics providers acting on a linked account.\ngranularity:\n  read_only_scope: false\n  per_resource_scopes: false\n  note: >-\n    Access scoping in Google Ads is done at the ACCOUNT level (which customer IDs the\n    authenticating user can reach, and the user-access\
  \ role held on each) rather than at\n    the scope level. CustomerUserAccess exposes roles such as read-only, standard and\n    admin — but those are properties of the Google Ads user, not of the OAuth grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-ads/refs/heads/main/scopes/google-ads-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Advertising
- Campaign Management
- Digital Advertising
- Google
- Marketing
- PPC
token_urls:
- https://oauth2.googleapis.com/token
---
