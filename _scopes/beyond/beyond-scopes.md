---
api_specs:
- filename: beyond-openapi-original.yml
  format: yaml
  label: Beyond Pricing Public API
  slug: beyond-pricing-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/openapi/beyond-openapi-original.yml
authorization_urls: []
description: ''
docs: https://developers.beyondpricing.com/getting-started/authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Beyond Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Beyond publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beyond API on a user''s behalf.


  Tokens are issued from https://developers.beyondpricing.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beyond
provider_slug: beyond
schemes:
- authorizationUrl: https://v2.beyondpricing.com/oauth/authorize
  description: Use OAuth2 client credentials to mint an application token, or add `user_id` and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://developers.beyondpricing.com/o/token/
  introspectionUrl: https://developers.beyondpricing.com/o/introspect/
  name: oauth2
  registrationUrl: https://developers.beyondpricing.com/o/register/
  revocationUrl: https://developers.beyondpricing.com/o/revoke/
  source: openapi/beyond-openapi-original.yml
  tokenUrl: https://developers.beyondpricing.com/o/token/
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
slug: beyond-scopes
source_filename: beyond-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/beyond-openapi-original.yml\ndocs: https://developers.beyondpricing.com/getting-started/authentication/\nauthorization_server_metadata: well-known/beyond-oauth-authorization-server.json\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- urn:ietf:params:oauth:grant-type:device_code\n- refresh_token\npkce: S256\nschemes:\n- name: oauth2\n  source: openapi/beyond-openapi-original.yml\n  authorizationUrl: https://v2.beyondpricing.com/oauth/authorize\n  tokenUrl: https://developers.beyondpricing.com/o/token/\n  introspectionUrl: https://developers.beyondpricing.com/o/introspect/\n  registrationUrl: https://developers.beyondpricing.com/o/register/\n  revocationUrl: https://developers.beyondpricing.com/o/revoke/\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://developers.beyondpricing.com/o/token/\n  description: Use OAuth2 client credentials to mint an application token, or add `user_id`\n\
  \    and optional `credential_id` in the Authorize dialog to request a user- or credential-scoped\n    token.\nscopes:\n- scope: accounts:read\n  description: Read account information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: compsets:read\n  description: Read competitive set data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: insights:read\n  description: Read market insights\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: listings:read\n  description: Read listings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: listings:write\n  description: Modify listings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: neyoba:ask\n  description: Ask Neyoba\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: reservations:read\n\
  \  description: Read reservations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: user:read\n  description: Read user information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n- scope: user:write\n  description: Create and modify users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/beyond-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beyond/refs/heads/main/scopes/beyond-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Company
- Consumer
- Travel
- Hospitality
- Short-Term Rentals
- Vacation Rentals
- Revenue Management
- Dynamic Pricing
- Pricing
- Real Estate
- Market Intelligence
- API
token_urls:
- https://developers.beyondpricing.com/o/token/
---
