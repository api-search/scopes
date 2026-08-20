---
api_specs:
- filename: sequel-analytics-api-openapi.yml
  format: yaml
  label: Sequel Analytics API
  slug: sequel-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-analytics-api-openapi.yml
- filename: sequel-client-api-openapi.yml
  format: yaml
  label: Sequel Client API
  slug: sequel-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-client-api-openapi.yml
- filename: sequel-company-api-openapi.yml
  format: yaml
  label: Sequel company API
  slug: sequel-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-api-openapi.yml
- filename: sequel-company-theme-api-openapi.yml
  format: yaml
  label: Sequel company theme API
  slug: sequel-company-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-api-openapi.yml
- filename: sequel-company-theme-fonts-api-openapi.yml
  format: yaml
  label: Sequel company theme fonts API
  slug: sequel-company-theme-fonts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-fonts-api-openapi.yml
- filename: sequel-company-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel company theme overrides API
  slug: sequel-company-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-overrides-api-openapi.yml
- filename: sequel-event-api-openapi.yml
  format: yaml
  label: Sequel event API
  slug: sequel-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-api-openapi.yml
- filename: sequel-event-theme-api-openapi.yml
  format: yaml
  label: Sequel event theme API
  slug: sequel-event-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-api-openapi.yml
- filename: sequel-event-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel event theme overrides API
  slug: sequel-event-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-overrides-api-openapi.yml
- filename: sequel-media-api-openapi.yml
  format: yaml
  label: Sequel Media API
  slug: sequel-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-media-api-openapi.yml
- filename: sequel-networking-api-openapi.yml
  format: yaml
  label: Sequel networking API
  slug: sequel-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-networking-api-openapi.yml
- filename: sequel-platform-api-openapi.yml
  format: yaml
  label: Sequel platform API
  slug: sequel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-platform-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.introvoke.com/docs
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sequel Scopes
name_suffix: OAuth Scopes
note: The published OpenAPI declares NO oauth2 securityScheme (only http bearer + an apiKey Authorization header), so `derive-oauth-scopes.py` yields nothing for this provider. Everything below was read from the two RFC 8414 / RFC 9728 discovery documents the provider actually serves, and from the docs' authentication page. Nothing here is inferred.
overview: 'Sequel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sequel
provider_slug: sequel
schemes:
- audience: https://www.introvoke.com/api
  flow: clientCredentials
  name: api-client-credentials
  note: The REST API's own machine-to-machine flow is scope-free. Sequel's docs instruct clients to POST client_id + client_secret + audience + grant_type=client_credentials and use the returned JWT as a bearer token; no `scope` parameter is documented and no scope values are published. Authorization is therefore all-or-nothing per API client — an agent holding a Sequel token can reach every operation that client's company is entitled to, including destructive ones (deleteevent, deleteRegistrantById, postClearChat). There is no way to issue a read-only API credential.
  scopes: []
  scopes_published: false
  token_url: https://api.introvoke.com/api/oauth/token
  type: oauth2
- authorization_servers:
  - https://login.introvoke.com
  bearer_methods_supported:
  - header
  name: mcp-protected-resource
  note: These are the four standard OIDC scopes the Auth0 tenant advertises for the interactive user-login flow that fronts the MCP server. They authenticate the human; they do NOT describe or constrain what the MCP tools may read. There is no Sequel-specific scope (nothing like `transcripts:read` or `events:read`), so an MCP client's data access is bounded by the account's own permissions rather than by a consent-time grant the user can narrow.
  resource: https://prod-api-elb.sequelvideo.com/api/mcp
  resource_public_endpoint: https://api.introvoke.com/api/mcp
  scopes:
  - description: OpenID Connect — issue an ID token identifying the end user.
    scope: openid
    source: /.well-known/oauth-protected-resource
  - description: Access the end user's basic profile claims.
    scope: profile
    source: /.well-known/oauth-protected-resource
  - description: Access the end user's email address claim.
    scope: email
    source: /.well-known/oauth-protected-resource
  - description: Issue a refresh token so the MCP client can act without re-prompting.
    scope: offline_access
    source: /.well-known/oauth-protected-resource
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: sequel-scopes
source_filename: sequel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.introvoke.com/.well-known/oauth-protected-resource + https://api.introvoke.com/.well-known/oauth-authorization-server\ndocs: https://docs.introvoke.com/docs\nnote: >-\n  The published OpenAPI declares NO oauth2 securityScheme (only http bearer + an apiKey\n  Authorization header), so `derive-oauth-scopes.py` yields nothing for this provider.\n  Everything below was read from the two RFC 8414 / RFC 9728 discovery documents the\n  provider actually serves, and from the docs' authentication page. Nothing here is\n  inferred.\nschemes:\n- name: api-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.introvoke.com/api/oauth/token\n  audience: https://www.introvoke.com/api\n  scopes_published: false\n  scopes: []\n  note: >-\n    The REST API's own machine-to-machine flow is scope-free. Sequel's docs instruct\n    clients to POST client_id + client_secret + audience + grant_type=client_credentials\n\
  \    and use the returned JWT as a bearer token; no `scope` parameter is documented and\n    no scope values are published. Authorization is therefore all-or-nothing per API\n    client — an agent holding a Sequel token can reach every operation that client's\n    company is entitled to, including destructive ones (deleteevent, deleteRegistrantById,\n    postClearChat). There is no way to issue a read-only API credential.\n- name: mcp-protected-resource\n  type: oauth2\n  resource: https://prod-api-elb.sequelvideo.com/api/mcp\n  resource_public_endpoint: https://api.introvoke.com/api/mcp\n  authorization_servers:\n  - https://login.introvoke.com\n  bearer_methods_supported:\n  - header\n  scopes:\n  - scope: openid\n    description: OpenID Connect — issue an ID token identifying the end user.\n    source: /.well-known/oauth-protected-resource\n  - scope: profile\n    description: Access the end user's basic profile claims.\n    source: /.well-known/oauth-protected-resource\n  - scope:\
  \ email\n    description: Access the end user's email address claim.\n    source: /.well-known/oauth-protected-resource\n  - scope: offline_access\n    description: Issue a refresh token so the MCP client can act without re-prompting.\n    source: /.well-known/oauth-protected-resource\n  note: >-\n    These are the four standard OIDC scopes the Auth0 tenant advertises for the\n    interactive user-login flow that fronts the MCP server. They authenticate the human;\n    they do NOT describe or constrain what the MCP tools may read. There is no\n    Sequel-specific scope (nothing like `transcripts:read` or `events:read`), so an MCP\n    client's data access is bounded by the account's own permissions rather than by a\n    consent-time grant the user can narrow.\ndiscovery:\n- path: /.well-known/oauth-protected-resource\n  host: api.introvoke.com\n  status: 200\n  spec: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n  file: well-known/sequel-oauth-protected-resource.json\n- path: /.well-known/oauth-authorization-server\n\
  \  host: api.introvoke.com\n  status: 200\n  spec: RFC 8414 (OAuth 2.0 Authorization Server Metadata)\n  file: well-known/sequel-oauth-authorization-server.json\nauthorization_server:\n  issuer: https://login.introvoke.com\n  provider: Auth0\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\ncross_ref:\n  authentication: authentication/sequel-authentication.yml\n  mcp: mcp/sequel-mcp.yml\n  well_known: well-known/sequel-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/scopes/sequel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Webinars
- Virtual Events
- Live Streaming
- Video
- Networking
- Marketing
- Event
- Webhook
token_urls: []
---
