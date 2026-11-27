---
api_specs:
- filename: cherami-to-access-api-openapi.yml
  format: yaml
  label: Cherami Access API
  slug: cherami-to-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-access-api-openapi.yml
- filename: cherami-to-drafts-api-openapi.yml
  format: yaml
  label: Cherami Drafts API
  slug: cherami-to-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-drafts-api-openapi.yml
- filename: cherami-to-feedback-api-openapi.yml
  format: yaml
  label: Cherami Feedback API
  slug: cherami-to-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-feedback-api-openapi.yml
- filename: cherami-to-inboxes-api-openapi.yml
  format: yaml
  label: Cherami Inboxes API
  slug: cherami-to-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-inboxes-api-openapi.yml
- filename: cherami-to-labels-api-openapi.yml
  format: yaml
  label: Cherami Labels API
  slug: cherami-to-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-labels-api-openapi.yml
- filename: cherami-to-messages-api-openapi.yml
  format: yaml
  label: Cherami Messages API
  slug: cherami-to-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-messages-api-openapi.yml
- filename: cherami-to-sending-api-openapi.yml
  format: yaml
  label: Cherami Sending API
  slug: cherami-to-sending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-sending-api-openapi.yml
- filename: cherami-to-threads-api-openapi.yml
  format: yaml
  label: Cherami Threads API
  slug: cherami-to-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-threads-api-openapi.yml
- filename: cherami-to-trash-api-openapi.yml
  format: yaml
  label: Cherami Trash API
  slug: cherami-to-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-trash-api-openapi.yml
- filename: cherami-to-webhooks-api-openapi.yml
  format: yaml
  label: Cherami Webhooks API
  slug: cherami-to-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cherami-to/openapi/cherami-to-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://cherami.to/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cherami Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cherami publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cherami API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cherami
provider_slug: cherami-to
schemes: []
scope_count: 1
scope_names:
- cherami_mail:full
scopes:
- description: OAuth mail scope for the Cherami MCP server (docs table "OAuth mail scope").
  flows: []
  scope: cherami_mail:full
slug: cherami-to-scopes
source_filename: cherami-to-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://cherami.to/docs/mcp\ndocs: https://cherami.to/docs/mcp\napplies_to: Hosted MCP server at https://cherami.to/mcp (OAuth via CIMD or DCR). The HTTP API itself accepts only Cherami API keys; per its OpenAPI, MCP OAuth tokens are not accepted there.\nscopes:\n- name: cherami_mail:full\n  description: OAuth mail scope for the Cherami MCP server (docs table \"OAuth mail scope\").\n"
source_yaml_url: https://artifacts.apis.io/cherami-to/scopes/cherami-to-scopes.yml
summary_line: 1 scope
tags:
- Company
- Email
- AI Agents
- MCP
- Webhook
- Messaging
- Email API
token_bound: false
token_urls: []
---
