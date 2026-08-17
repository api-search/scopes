---
api_specs:
- filename: loops-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-api-key-api-openapi.yml
- filename: loops-audience-segments-api-openapi.yml
  format: yaml
  label: Loops Audience segments API
  slug: loops-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-audience-segments-api-openapi.yml
- filename: loops-campaign-groups-api-openapi.yml
  format: yaml
  label: Loops Campaign groups API
  slug: loops-campaign-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaign-groups-api-openapi.yml
- filename: loops-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaigns-api-openapi.yml
- filename: loops-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-components-api-openapi.yml
- filename: loops-configuration-api-openapi.yml
  format: yaml
  label: Loops Configuration API
  slug: loops-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-configuration-api-openapi.yml
- filename: loops-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contact-properties-api-openapi.yml
- filename: loops-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contacts-api-openapi.yml
- filename: loops-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-email-messages-api-openapi.yml
- filename: loops-event-patterns-api-openapi.yml
  format: yaml
  label: Loops Event patterns API
  slug: loops-event-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-event-patterns-api-openapi.yml
- filename: loops-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-events-api-openapi.yml
- filename: loops-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-mailing-lists-api-openapi.yml
- filename: loops-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-themes-api-openapi.yml
- filename: loops-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-emails-api-openapi.yml
- filename: loops-transactional-groups-api-openapi.yml
  format: yaml
  label: Loops Transactional groups API
  slug: loops-transactional-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-groups-api-openapi.yml
- filename: loops-uploads-api-openapi.yml
  format: yaml
  label: Loops Uploads API
  slug: loops-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-uploads-api-openapi.yml
- filename: loops-workflow-nodes-api-openapi.yml
  format: yaml
  label: Loops Workflow nodes API
  slug: loops-workflow-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-workflow-nodes-api-openapi.yml
- filename: loops-workflows-api-openapi.yml
  format: yaml
  label: Loops Workflows API
  slug: loops-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-workflows-api-openapi.yml
- filename: loops-webhooks-asyncapi.yml
  format: yaml
  label: Loops Webhooks
  slug: loops-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/asyncapi/loops-webhooks-asyncapi.yml
authorization_urls: []
description: ''
docs: https://loops.so/docs/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Loops Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Loops uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Loops
provider_slug: loops
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: loops-scopes
source_filename: loops-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.loops.so/.well-known/oauth-authorization-server\ndocs: https://loops.so/docs/mcp-server\nsummary: >-\n  Loops runs exactly one OAuth 2.0 authorization server and it exists to\n  authorize the MCP server, not the REST API. The REST API has no OAuth surface\n  at all — it is API-key only, and a Loops API key is unscoped. So the entire\n  scope vocabulary for this provider is a single opaque scope, `mcp`, which\n  grants an MCP client the same reach the signed-in user has.\nauthorization_server:\n  issuer: https://app.loops.so\n  metadata: https://app.loops.so/.well-known/oauth-authorization-server\n  metadata_spec: RFC 8414\n  http_status: 200\n  authorization_endpoint: https://app.loops.so/oauth/authorize\n  token_endpoint: https://app.loops.so/oauth/token\n  revocation_endpoint: https://app.loops.so/oauth/revoke\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n  response_types_supported:\n\
  \    - code\n  response_modes_supported:\n    - query\n  code_challenge_methods_supported:\n    - S256\n  token_endpoint_auth_methods_supported:\n    - none\n  client_id_metadata_document_supported: true\n  dynamic_client_registration: false\nprotected_resource:\n  resource: https://mcp.loops.so/\n  metadata: https://mcp.loops.so/.well-known/oauth-protected-resource\n  metadata_spec: RFC 9728\n  http_status: 200\n  authorization_servers:\n    - https://app.loops.so\n  bearer_methods_supported:\n    - header\nscopes:\n  - name: mcp\n    description: >-\n      Grants an MCP client access to the Loops MCP server at\n      https://mcp.loops.so. Advertised in both the authorization-server and\n      protected-resource metadata and returned in the WWW-Authenticate challenge\n      on an unauthenticated request.\n    resource: https://mcp.loops.so/\n    granularity: coarse\n    read_write: both\n    documented_effect: >-\n      The MCP server exposes search, describe, execute and teams. `execute`\
  \ can\n      run any operation in the Loops REST API for any team the signed-in user\n      can reach, which includes writes — creating and updating contacts,\n      sending events, and sending transactional email. Loops' own FAQ asks \"Can\n      the MCP server change data or send email?\" on its MCP page.\nscope_count: 1\ngranularity: single-scope\nobservations:\n  - >-\n    There is no read-only scope. Consenting to `mcp` is consenting to the full\n    write surface of every team the user belongs to; an agent cannot be granted\n    a narrower grant.\n  - >-\n    Public-client posture is correct for an MCP server —\n    `token_endpoint_auth_methods_supported: [\"none\"]` with PKCE S256 required —\n    but client identity comes from Client ID Metadata Documents or\n    pre-registration rather than RFC 7591 dynamic registration, so an arbitrary\n    new client cannot self-register.\n  - Refresh tokens and a revocation endpoint are both supported.\n  - >-\n    The REST API declares one\
  \ securityScheme (`apiKey`, http bearer) applied to\n    all 64 operations, with no scopes. See\n    authentication/loops-authentication.yml.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/scopes/loops-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Email
- Email API
- Marketing Automation
- Transactional Email
- Lifecycle Email
- Webhooks
- SaaS
- Communications
- Developer Tools
- MCP
- Agents
- Campaigns
token_urls: []
---
