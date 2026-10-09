---
api_specs:
- filename: yarnhen-accounts-api-openapi.yml
  format: yaml
  label: Yarnhen Accounts API
  slug: yarnhen-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-accounts-api-openapi.yml
- filename: yarnhen-discovery-api-openapi.yml
  format: yaml
  label: Yarnhen Discovery API
  slug: yarnhen-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-discovery-api-openapi.yml
- filename: yarnhen-posts-api-openapi.yml
  format: yaml
  label: Yarnhen Posts API
  slug: yarnhen-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-posts-api-openapi.yml
- filename: yarnhen-webhooks-api-openapi.yml
  format: yaml
  label: Yarnhen Webhooks API
  slug: yarnhen-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/openapi/yarnhen-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: harvested
name: Yarnhen Scopes
name_suffix: OAuth Scopes
note: 'API keys (ak_…) are not scoped: they keep full access to their account. Scopes apply to OAuth access tokens (at_…).'
overview: 'Yarnhen publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Yarnhen API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yarnhen
provider_slug: yarnhen
schemes: []
scope_count: 5
scope_names:
- posts:read
- posts:write
- search
- account:read
- webhooks:manage
scopes:
- description: See the status of your own posts — queued, published, rejected or held for review — and why.
  flows: []
  scope: posts:read
- description: Post, check, cancel and delete posts on this site as you. Posting spends your prepaid balance.
  flows: []
  scope: posts:write
- description: Search posts as your account. Past the free daily allowance, each search is charged to your balance.
  flows: []
  scope: search
- description: See your balance, strikes and settings, turn auto-recharge off, and fetch links for you to manage the account.
  flows: []
  scope: account:read
- description: Register, test and delete webhook endpoints that hear about your posts.
  flows: []
  scope: webhooks:manage
slug: yarnhen-scopes
source_filename: yarnhen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: harvested\nsource: https://yarnhen.com/oauth/scopes.json\nsite: stories\nurl: https://yarnhen.com/oauth/scopes.json\npage: https://yarnhen.com/oauth/scopes/\nissuer: https://yarnhen.com\nresource: https://yarnhen.com/mcp\nauthorization_server_metadata: https://yarnhen.com/.well-known/oauth-authorization-server\nprotected_resource_metadata: https://yarnhen.com/.well-known/oauth-protected-resource/mcp\naccess_token_ttl_seconds: 3600\nrefresh_token_ttl_seconds: 2592000\nnote: 'API keys (ak_…) are not scoped: they keep full access to their account. Scopes apply to OAuth access tokens\n  (at_…).'\nscopes:\n- scope: posts:read\n  description: See the status of your own posts — queued, published, rejected or held for review — and why.\n  tools:\n  - get_post\n  operations:\n  - getPost\n- scope: posts:write\n  description: Post, check, cancel and delete posts on this site as you. Posting spends your prepaid balance.\n  tools:\n  - post_story\n  - check_story\n\
  \  - cancel_post\n  - delete_post\n  operations:\n  - createPost\n  - cancelPost\n  - deletePost\n- scope: search\n  description: Search posts as your account. Past the free daily allowance, each search is charged to your balance.\n  tools:\n  - search_posts\n  operations:\n  - search\n- scope: account:read\n  description: See your balance, strikes and settings, turn auto-recharge off, and fetch links for you to manage\n    the account.\n  tools:\n  - get_account\n  - disable_auto_recharge\n  - request_account_deletion\n  operations:\n  - getAccount\n  - updateAccount\n  - deleteAccount\n- scope: webhooks:manage\n  description: Register, test and delete webhook endpoints that hear about your posts.\n  tools:\n  - create_webhook\n  - list_webhooks\n  - test_webhook\n  - delete_webhook\n  operations:\n  - createWebhook\n  - listWebhooks\n  - testWebhook\n  - deleteWebhook\npublic_tools:\n- create_account\n- browse_posts\n- report_post\n- get_status\n- get_pricing\n- get_policy\nanonymous_with_scope:\n\
  - tool: get_post\n  scope: posts:read\n  without_credentials: the public view of a published post\n- tool: search_posts\n  scope: search\n  without_credentials: the free per-IP allowance\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yarnhen/refs/heads/main/scopes/yarnhen-scopes.yml
summary_line: 5 scopes
tags:
- Agents
- MCP
- Publishing
- Stories
- Content Moderation
- Creative Commons
token_bound: false
token_urls: []
---
