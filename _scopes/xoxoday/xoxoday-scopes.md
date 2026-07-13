---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Xoxoday Plum Rewards API
  slug: plum-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoxoday/refs/heads/main/openapi/openapi.yml
authorization_urls: []
description: ''
docs: https://xoxoday.gitbook.io/plum/developer-resources/storefront-integration/api-endpoints/authorization
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Xoxoday Scopes
name_suffix: OAuth Scopes
note: Scopes apply to Xoxoday's StoreFront authorization-code OAuth flow; the Rewards API client-credentials flow (https://developers.xoxoday.com/docs/authentication-2) documents no scopes, with access controlled by client credentials and IP whitelisting.
overview: 'Xoxoday publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xoxoday API on a user''s behalf.


  Tokens are issued from https://accounts.xoxoday.com/chef/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xoxoday
provider_slug: xoxoday
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.xoxoday.com/chef/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/openapi.yml
scope_count: 2
scope_names:
- user_session
- company_session
scopes:
- description: Company scope used only for the case of Company access_token generation; compulsory when the authorization request is for company session generation.
  flows: []
  scope: user_session
- description: Company scope for StoreFront OAuth authorization requests.
  flows: []
  scope: company_session
slug: xoxoday-scopes
source_filename: xoxoday-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/openapi.yml\ndocs: https://xoxoday.gitbook.io/plum/developer-resources/storefront-integration/api-endpoints/authorization\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.xoxoday.com/chef/v1/oauth/token\nscopes:\n- scope: user_session\n  description: Company scope used only for the case of Company access_token generation;\n    compulsory when the authorization request is for company session generation.\n  sources:\n  - https://xoxoday.gitbook.io/plum/developer-resources/storefront-integration/api-endpoints/authorization\n- scope: company_session\n  description: Company scope for StoreFront OAuth authorization requests.\n  sources:\n  - https://xoxoday.gitbook.io/plum/developer-resources/storefront-integration/api-endpoints/authorization\nnote: Scopes apply to Xoxoday's StoreFront authorization-code OAuth flow; the Rewards\n\
  \  API client-credentials flow (https://developers.xoxoday.com/docs/authentication-2)\n  documents no scopes, with access controlled by client credentials and IP whitelisting.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xoxoday/refs/heads/main/scopes/xoxoday-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Rewards
- Employee Engagement
- Gift Cards
- Incentives
- Loyalty
- Recognition
- Digital Rewards
- Points Programs
- Redemption
- Fintech
token_urls:
- https://accounts.xoxoday.com/chef/v1/oauth/token
---
