---
api_specs:
- filename: shopmy-partners-openapi.yml
  format: yaml
  label: ShopMy Partners API
  slug: shopmy-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/openapi/shopmy-partners-openapi.yml
authorization_urls:
- https://shopmy.us/oauth
description: ''
docs: https://docs.shopmy.us/reference/getting-started-with-your-api-1
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Shopmy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ShopMy publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ShopMy API on a user''s behalf.


  Tokens are issued from https://api.shopmy.us/v1/Partners/oauth-exchange-token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ShopMy
provider_slug: shopmy
schemes:
- description: OAuth 2.0 authorization-code flow for acting on behalf of ShopMy users.
  flows:
  - authorizationUrl: https://shopmy.us/oauth
    flow: authorizationCode
    tokenUrl: https://api.shopmy.us/v1/Partners/oauth-exchange-token
  name: oauth2
  source: openapi/shopmy-partners-openapi.yml
scope_count: 5
scope_names:
- read_collections
- read_links
- read_profile
- write_collections
- write_links
scopes:
- description: View shelf collections.
  flows:
  - authorizationCode
  scope: read_collections
- description: View product links.
  flows:
  - authorizationCode
  scope: read_links
- description: View public profile information.
  flows:
  - authorizationCode
  scope: read_profile
- description: Create and edit collections.
  flows:
  - authorizationCode
  scope: write_collections
- description: View and edit product links.
  flows:
  - authorizationCode
  scope: write_links
slug: shopmy-scopes
source_filename: shopmy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/shopmy-partners-openapi.yml\ndocs: https://docs.shopmy.us/reference/getting-started-with-your-api-1\nschemes:\n- name: oauth2\n  source: openapi/shopmy-partners-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopmy.us/oauth\n    tokenUrl: https://api.shopmy.us/v1/Partners/oauth-exchange-token\n  description: OAuth 2.0 authorization-code flow for acting on behalf of ShopMy users.\nscopes:\n- scope: read_collections\n  description: View shelf collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n- scope: read_links\n  description: View product links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n- scope: read_profile\n  description: View public profile information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n- scope: write_collections\n  description: Create\
  \ and edit collections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n- scope: write_links\n  description: View and edit product links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shopmy-partners-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopmy/refs/heads/main/scopes/shopmy-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Commerce
- Creator Economy
- Creator Commerce
- Affiliate Marketing
- Influencer Marketing
- E-Commerce
- Retail
token_urls:
- https://api.shopmy.us/v1/Partners/oauth-exchange-token
---
