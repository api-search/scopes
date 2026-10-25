---
api_specs:
- filename: envato-market-api-openapi.yml
  format: yaml
  label: Envato Market API
  slug: envato-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-market-api-openapi.yml
- filename: envato-search-api-openapi.yml
  format: yaml
  label: Envato Search API
  slug: envato-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-search-api-openapi.yml
authorization_urls:
- https://api.envato.com/authorization
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Envato Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Envato publishes 18 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Envato API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Envato
provider_slug: envato
schemes:
- flows:
  - authorizationUrl: https://api.envato.com/authorization
    flow: implicit
  name: oauth2
  source: openapi/envato-openapi.yml
scope_count: 18
scope_names:
- default
- purchase:download
- purchase:history
- purchase:list
- purchase:verify
- sale:history
- sale:verify
- stat:total_community_earnings
- stat:total_items
- stat:total_items_sold
- stat:total_users
- user:account
- user:collections
- user:email
- user:favourite_collection_add
- user:financial
- user:statement
- user:username
scopes:
- description: View and search Envato sites
  flows:
  - implicit
  scope: default
- description: Download my purchased items
  flows:
  - implicit
  scope: purchase:download
- description: View my purchases of the app creator's items
  flows:
  - implicit
  scope: purchase:history
- description: List purchases I've made
  flows:
  - implicit
  scope: purchase:list
- description: Verify purchases I've made
  flows:
  - implicit
  scope: purchase:verify
- description: View my items' sales history
  flows:
  - implicit
  scope: sale:history
- description: Verify purchases of my items
  flows:
  - implicit
  scope: sale:verify
- description: Shows the total amount of community earnings on Envato Market
  flows:
  - implicit
  scope: stat:total_community_earnings
- description: Shows the total number of items available on Envato Market
  flows:
  - implicit
  scope: stat:total_items
- description: Shows the total number of items sold on Envato Market
  flows:
  - implicit
  scope: stat:total_items_sold
- description: View the total number of subscribed users to Envato Market
  flows:
  - implicit
  scope: stat:total_users
- description: View my account profile details
  flows:
  - implicit
  scope: user:account
- description: View my public and private collections
  flows:
  - implicit
  scope: user:collections
- description: View my email address
  flows:
  - implicit
  scope: user:email
- description: Add item to favourite collection
  flows:
  - implicit
  scope: user:favourite_collection_add
- description: View my account financial history
  flows:
  - implicit
  scope: user:financial
- description: View my statement transactions
  flows:
  - implicit
  scope: user:statement
- description: View my Envato Account username
  flows:
  - implicit
  scope: user:username
slug: envato-scopes
source_filename: envato-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: derived\nsource: openapi/envato-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/envato-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.envato.com/authorization\nscopes:\n- scope: default\n  description: View and search Envato sites\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: purchase:download\n  description: Download my purchased items\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: purchase:history\n  description: View my purchases of the app creator's items\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: purchase:list\n  description: List purchases I've made\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: purchase:verify\n  description: Verify purchases I've made\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: sale:history\n  description: View my items'\
  \ sales history\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: sale:verify\n  description: Verify purchases of my items\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: stat:total_community_earnings\n  description: Shows the total amount of community earnings on Envato Market\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: stat:total_items\n  description: Shows the total number of items available on Envato Market\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: stat:total_items_sold\n  description: Shows the total number of items sold on Envato Market\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: stat:total_users\n  description: View the total number of subscribed users to Envato Market\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:account\n  description: View my account profile details\n  flows:\n  -\
  \ implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:collections\n  description: View my public and private collections\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:email\n  description: View my email address\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:favourite_collection_add\n  description: Add item to favourite collection\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:financial\n  description: View my account financial history\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:statement\n  description: View my statement transactions\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n- scope: user:username\n  description: View my Envato Account username\n  flows:\n  - implicit\n  sources:\n  - openapi/envato-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/scopes/envato-scopes.yml
summary_line: 18 scopes · implicit
tags:
- Stock Media
- Marketplace
- Themes
- Audio
- Video
- Graphics
- Subscription
- Australia
token_bound: false
token_urls: []
---
