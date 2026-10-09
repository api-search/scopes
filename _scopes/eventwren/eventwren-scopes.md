---
api_specs:
- filename: eventwren-accounts-api-openapi.yml
  format: yaml
  label: Eventwren Accounts API
  slug: eventwren-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-accounts-api-openapi.yml
- filename: eventwren-discovery-api-openapi.yml
  format: yaml
  label: Eventwren Discovery API
  slug: eventwren-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-discovery-api-openapi.yml
- filename: eventwren-posts-api-openapi.yml
  format: yaml
  label: Eventwren Posts API
  slug: eventwren-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-posts-api-openapi.yml
- filename: eventwren-webhooks-api-openapi.yml
  format: yaml
  label: Eventwren Webhooks API
  slug: eventwren-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/openapi/eventwren-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: harvested
name: Eventwren Scopes
name_suffix: OAuth Scopes
note: 'API keys (ak_…) are not scoped: they keep full access to their account. Scopes apply to OAuth access tokens (at_…).'
overview: 'Eventwren publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Eventwren API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eventwren
provider_slug: eventwren
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
slug: eventwren-scopes
source_filename: eventwren-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: harvested\nsource: https://eventwren.com/oauth/scopes.json\nsite: events\nurl: https://eventwren.com/oauth/scopes.json\npage: https://eventwren.com/oauth/scopes/\nissuer: https://eventwren.com\nresource: https://eventwren.com/mcp\nauthorization_server_metadata: https://eventwren.com/.well-known/oauth-authorization-server\nprotected_resource_metadata: https://eventwren.com/.well-known/oauth-protected-resource/mcp\naccess_token_ttl_seconds: 3600\nrefresh_token_ttl_seconds: 2592000\nnote: 'API keys (ak_…) are not scoped: they keep full access to their account. Scopes apply to OAuth access tokens\n  (at_…).'\nscopes:\n- scope: posts:read\n  description: See the status of your own posts — queued, published, rejected or held for review — and why.\n  tools:\n  - get_post\n  operations:\n  - getPost\n- scope: posts:write\n  description: Post, check, cancel and delete posts on this site as you. Posting spends your prepaid balance.\n  tools:\n  - post_event\n\
  \  - check_event\n  - cancel_post\n  - delete_post\n  operations:\n  - createPost\n  - cancelPost\n  - deletePost\n- scope: search\n  description: Search posts as your account. Past the free daily allowance, each search is charged to your balance.\n  tools:\n  - search_posts\n  operations:\n  - search\n- scope: account:read\n  description: See your balance, strikes and settings, turn auto-recharge off, and fetch links for you to manage\n    the account.\n  tools:\n  - get_account\n  - disable_auto_recharge\n  - request_account_deletion\n  operations:\n  - getAccount\n  - updateAccount\n  - deleteAccount\n- scope: webhooks:manage\n  description: Register, test and delete webhook endpoints that hear about your posts.\n  tools:\n  - create_webhook\n  - list_webhooks\n  - test_webhook\n  - delete_webhook\n  operations:\n  - createWebhook\n  - listWebhooks\n  - testWebhook\n  - deleteWebhook\npublic_tools:\n- create_account\n- browse_posts\n- report_post\n- get_status\n- get_pricing\n- get_policy\n\
  anonymous_with_scope:\n- tool: get_post\n  scope: posts:read\n  without_credentials: the public view of a published post\n- tool: search_posts\n  scope: search\n  without_credentials: the free per-IP allowance\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventwren/refs/heads/main/scopes/eventwren-scopes.yml
summary_line: 5 scopes
tags:
- Agents
- MCP
- Event
- Calendar
- Content Moderation
- Publishing
token_bound: false
token_urls: []
---
