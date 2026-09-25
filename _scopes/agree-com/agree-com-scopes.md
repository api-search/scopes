---
api_specs:
- filename: agree-com-agreements-api-openapi.yml
  format: yaml
  label: Agree.com Agreements API
  slug: agree-com-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-agreements-api-openapi.yml
- filename: agree-com-contacts-api-openapi.yml
  format: yaml
  label: Agree.com Contacts API
  slug: agree-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-contacts-api-openapi.yml
- filename: agree-com-customers-api-openapi.yml
  format: yaml
  label: Agree.com Customers API
  slug: agree-com-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-customers-api-openapi.yml
- filename: agree-com-invoices-api-openapi.yml
  format: yaml
  label: Agree.com Invoices API
  slug: agree-com-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-invoices-api-openapi.yml
- filename: agree-com-reports-api-openapi.yml
  format: yaml
  label: Agree.com Reports API
  slug: agree-com-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-reports-api-openapi.yml
- filename: agree-com-webhooks-api-openapi.yml
  format: yaml
  label: Agree.com Webhooks API
  slug: agree-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-webhooks-api-openapi.yml
authorization_urls: []
description: Agree.com's OAuth 2.1 authorization server advertises exactly one scope. It governs the hosted MCP server and nothing else - the REST API uses an unscoped bearer API key and has no OAuth surface at all.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agree Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agree.com uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agree.com
provider_slug: agree-com
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agree-com-scopes
source_filename: agree-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://secure.agree.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  No scopes or permissions reference page is published. agree.com/developers does not mention\n  OAuth scopes, and the API documentation at secure.agree.com/documentation covers only the\n  bearer API key. The scope list below is read from the authorization server's own RFC 8414\n  metadata document, which is the only place Agree.com publishes it.\nname: Agree.com OAuth Scopes\ndescription: >-\n  Agree.com's OAuth 2.1 authorization server advertises exactly one scope. It governs the\n  hosted MCP server and nothing else - the REST API uses an unscoped bearer API key and has\n  no OAuth surface at all.\nauthorization_server:\n  issuer: https://secure.agree.com\n  metadata: https://secure.agree.com/.well-known/oauth-authorization-server\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  -\
  \ code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  dynamic_client_registration: https://secure.agree.com/oauth/register\n  revocation_endpoint: https://secure.agree.com/oauth/revoke\n  op_policy_uri: https://agree.com/privacy\nscope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    Access to the Agree MCP server at https://secure.agree.com/mcp. Declared in\n    scopes_supported in the authorization server metadata.\n  grants: unknown\n  grants_note: >-\n    NOT DOCUMENTED. Agree.com publishes no statement of what this scope permits. Because the\n    MCP tool list is itself OAuth-gated, the set of actions a holder of this scope can take -\n    including whether it can create and send invoices, send agreements for signature, or read\n    revenue reporting - cannot be established from any public source. This is the single\n    largest agent-readiness gap on this provider: a consent\
  \ screen backed by one opaque,\n    undocumented scope gives a user no basis to decide what they are authorizing.\n  resource: https://secure.agree.com/mcp\n  source: https://secure.agree.com/.well-known/oauth-authorization-server\nfindings:\n- >-\n  One coarse scope for an entire contract-and-payments surface. There is no read-only scope\n  and no separation between signing authority and money movement.\n- >-\n  Dynamic client registration is open at /oauth/register with token_endpoint_auth_method\n  \"none\" supported, which is the correct posture for public MCP clients and is what lets an\n  agent connect without a preregistered client ID.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/scopes/agree-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Agreements
- Electronic Signature
- Contract Management
- Invoicing
- Billing
- Payments
- Accounts Receivable
- Fintech
- Financial Services
- Webhook
- MCP
- Agent-Native
token_urls: []
---
