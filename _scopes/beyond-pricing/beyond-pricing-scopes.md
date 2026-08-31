---
api_specs:
- filename: beyond-pricing-accounts-api-openapi.yml
  format: yaml
  label: Beyond Pricing Accounts API
  slug: beyond-pricing-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-accounts-api-openapi.yml
- filename: beyond-pricing-compsets-api-openapi.yml
  format: yaml
  label: Beyond Pricing Compsets API
  slug: beyond-pricing-compsets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-compsets-api-openapi.yml
- filename: beyond-pricing-customizations-api-openapi.yml
  format: yaml
  label: Beyond Pricing Customizations API
  slug: beyond-pricing-customizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-customizations-api-openapi.yml
- filename: beyond-pricing-insights-api-openapi.yml
  format: yaml
  label: Beyond Pricing Insights API
  slug: beyond-pricing-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-insights-api-openapi.yml
- filename: beyond-pricing-listings-api-openapi.yml
  format: yaml
  label: Beyond Pricing Listings API
  slug: beyond-pricing-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-listings-api-openapi.yml
- filename: beyond-pricing-oauth2-api-openapi.yml
  format: yaml
  label: Beyond Pricing OAuth2 API
  slug: beyond-pricing-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-oauth2-api-openapi.yml
- filename: beyond-pricing-users-api-openapi.yml
  format: yaml
  label: Beyond Pricing Users API
  slug: beyond-pricing-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-users-api-openapi.yml
- filename: beyond-pricing-webhooks-api-openapi.yml
  format: yaml
  label: Beyond Pricing Webhooks API
  slug: beyond-pricing-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/openapi/beyond-pricing-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.beyondpricing.com/getting-started/authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Beyond Pricing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beyond Pricing publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beyond Pricing API on a user''s behalf.


  Tokens are issued from https://developers.beyondpricing.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beyond Pricing
provider_slug: beyond-pricing
schemes:
- description: Use OAuth2 client credentials to mint an application token, or add `user_id` and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developers.beyondpricing.com/o/token/
  name: oauth2
  source: openapi/beyond-pricing-openapi-original.yml
scope_count: 9
scope_names:
- accounts:read
- compsets:read
- insights:read
- listings:read
- listings:write
- neyoba:ask
- reservations:read
- user:read
- user:write
scopes:
- description: Read account information
  flows:
  - clientCredentials
  scope: accounts:read
- description: Read competitive set data
  flows:
  - clientCredentials
  scope: compsets:read
- description: Read market insights
  flows:
  - clientCredentials
  scope: insights:read
- description: Read listings
  flows:
  - clientCredentials
  scope: listings:read
- description: Modify listings
  flows:
  - clientCredentials
  scope: listings:write
- description: Ask Neyoba
  flows:
  - clientCredentials
  scope: neyoba:ask
- description: Read reservations
  flows:
  - clientCredentials
  scope: reservations:read
- description: Read user information
  flows:
  - clientCredentials
  scope: user:read
- description: Create and modify users
  flows:
  - clientCredentials
  scope: user:write
slug: beyond-pricing-scopes
source_filename: beyond-pricing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beyond-pricing-openapi-original.yml\ndocs: https://developers.beyondpricing.com/getting-started/authentication/\nauthorization_server_metadata: https://developers.beyondpricing.com/.well-known/oauth-authorization-server\nnotes: >-\n  Scopes must first be enabled for the OAuth application, then token-tier rules\n  apply. App-level scope (user:write) may only be used on an application-level\n  token (no user_id); user-level scopes (listings:read, listings:write,\n  reservations:read, accounts:read, insights:read) require a user-scoped token\n  when the app has require_user_scoped_tokens enabled. PATs (bpat_...) reuse the\n  same scope names at runtime even though OpenAPI cannot encode scopes for the\n  non-oauth bearer scheme.\nscope_tiers:\n  app_level:\n  - user:write\n  user_level:\n  - listings:read\n  - listings:write\n  - reservations:read\n  - accounts:read\n  - insights:read\n  cross_tier:\n  - user:read\nschemes:\n\
  - name: oauth2\n  source: openapi/beyond-pricing-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developers.beyondpricing.com/o/token/\n  description: Use OAuth2 client credentials to mint an application token, or add `user_id`\n    and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped\n    token.\nscopes:\n- scope: accounts:read\n  description: Read account information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: compsets:read\n  description: Read competitive set data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: insights:read\n  description: Read market insights\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: listings:read\n  description: Read listings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n\
  - scope: listings:write\n  description: Modify listings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: neyoba:ask\n  description: Ask Neyoba\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: reservations:read\n  description: Read reservations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: user:read\n  description: Read user information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n- scope: user:write\n  description: Create and modify users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-pricing-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond-pricing/refs/heads/main/scopes/beyond-pricing-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Company
- Short-Term Rentals
- Vacation Rentals
- Revenue Management
- Dynamic Pricing
- Hospitality
- Property Management
- Travel
- Pricing
- JSON:API
token_urls:
- https://developers.beyondpricing.com/o/token/
---
