---
api_specs:
- filename: splitwise-comments-api-openapi.yml
  format: yaml
  label: Splitwise comments API
  slug: splitwise-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-comments-api-openapi.yml
- filename: splitwise-expenses-api-openapi.yml
  format: yaml
  label: Splitwise expenses API
  slug: splitwise-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-expenses-api-openapi.yml
- filename: splitwise-friends-api-openapi.yml
  format: yaml
  label: Splitwise friends API
  slug: splitwise-friends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-friends-api-openapi.yml
- filename: splitwise-groups-api-openapi.yml
  format: yaml
  label: Splitwise groups API
  slug: splitwise-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-groups-api-openapi.yml
- filename: splitwise-notifications-api-openapi.yml
  format: yaml
  label: Splitwise notifications API
  slug: splitwise-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-notifications-api-openapi.yml
- filename: splitwise-other-api-openapi.yml
  format: yaml
  label: Splitwise other API
  slug: splitwise-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-other-api-openapi.yml
- filename: splitwise-users-api-openapi.yml
  format: yaml
  label: Splitwise users API
  slug: splitwise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/openapi/splitwise-users-api-openapi.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Splitwise Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Splitwise uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Splitwise
provider_slug: splitwise
schemes:
- description: 'Splitwise uses OAuth 2 with the authorization code flow. To connect via OAuth 2, you''ll need to [register your app](https://secure.splitwise.com/apps). When you register, you''ll be given a key and secret.


    **Note**: OAuth can be a very confusing protocol to implement correctly, and we **strongly** recommend

    that you use an existing OAuth library to connect to Splitwise. You can find a list of OAuth client libraries at the

    [OAuth community site](https://oauth.net/code/#client-libraries).


    For more information on using OAuth, check out the following resources:


    - The OAuth community [getting started guide](https://oauth.net/getting-started/)

    - The oauth.com [OAuth 2.0 playground](https://www.oauth.com/playground/) (great for debugging authorization issues)

    - This [old Splitwise blog post](https://blog.splitwise.com/2013/07/15/setting-up-oauth-for-the-splitwise-api/) about OAuth'
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: OAuth
  source: openapi/splitwise-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: splitwise-scopes
source_filename: splitwise-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/splitwise-openapi.json\nschemes:\n- name: OAuth\n  source: openapi/splitwise-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  description: |-\n    Splitwise uses OAuth 2 with the authorization code flow. To connect via OAuth 2, you'll need to [register your app](https://secure.splitwise.com/apps). When you register, you'll be given a key and secret.\n\n    **Note**: OAuth can be a very confusing protocol to implement correctly, and we **strongly** recommend\n    that you use an existing OAuth library to connect to Splitwise. You can find a list of OAuth client libraries at the\n    [OAuth community site](https://oauth.net/code/#client-libraries).\n\n    For more information on using OAuth, check out the following resources:\n\n    - The OAuth community [getting started guide](https://oauth.net/getting-started/)\n    - The oauth.com [OAuth 2.0 playground](https://www.oauth.com/playground/)\
  \ (great for debugging authorization issues)\n    - This [old Splitwise blog post](https://blog.splitwise.com/2013/07/15/setting-up-oauth-for-the-splitwise-api/) about OAuth\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitwise/refs/heads/main/scopes/splitwise-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Expense Management
- Personal Finance
- Bill Splitting
- Payments
- REST API
- Authentication
token_urls:
- /oauth/token
---
