---
api_specs:
- filename: xquik-rest-api-openapi.yml
  format: yaml
  label: Xquik REST API
  slug: xquik-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xquik-api/refs/heads/main/openapi/xquik-rest-api-openapi.yml
authorization_urls:
- https://xquik.com/api/oauth/authorize
description: Xquik's OAuth 2.1 scope surface, read from the provider's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata rather than from the OpenAPI (the spec declares the OAuth credential as an http bearer scheme, so it carries no oauth2 flow or scope map — deriving from the spec alone yields nothing). The live MCP 401 challenge advertises the same single scope, and the A2A agent card declares it too, so all three provider-published surfaces agree.
docs: https://docs.xquik.com/oauth/overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Xquik Scopes
name_suffix: OAuth Scopes
note: One scope, not a granular permission model. An mcp:tools token inherits whatever the underlying account may do; read/write separation is enforced by the credential type (guest paid_reads key vs full account key) rather than by scope. The agent card carried read/write scopes when this repo was first profiled on 2026-08-01; the live card now carries mcp:tools, matching the authorization server.
overview: 'Xquik publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xquik API on a user''s behalf.


  Tokens are issued from https://xquik.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xquik
provider_slug: xquik-api
schemes:
- flows:
  - authorizationUrl: https://xquik.com/api/oauth/authorize
    client_id_metadata_document_supported: true
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://xquik.com/api/oauth/register
    revocationUrl: https://xquik.com/api/oauth/revoke
    tokenUrl: https://xquik.com/api/oauth/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  issuer: https://xquik.com
  name: oauth2
  sources:
  - https://xquik.com/.well-known/oauth-authorization-server
  - https://xquik.com/.well-known/oauth-protected-resource/mcp
  - a2a/xquik-agent-card.json
  spec: OAuth 2.1 with PKCE (S256)
  type: oauth2
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Run approved Xquik MCP tools.
  flows:
  - authorizationCode
  scope: mcp:tools
slug: xquik-scopes
source_filename: xquik-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://xquik.com/.well-known/oauth-authorization-server\ndocs: https://docs.xquik.com/oauth/overview\ndescription: >-\n  Xquik's OAuth 2.1 scope surface, read from the provider's own RFC 8414 authorization-server\n  metadata and RFC 9728 protected-resource metadata rather than from the OpenAPI (the spec\n  declares the OAuth credential as an http bearer scheme, so it carries no oauth2 flow or\n  scope map — deriving from the spec alone yields nothing). The live MCP 401 challenge\n  advertises the same single scope, and the A2A agent card declares it too, so all three\n  provider-published surfaces agree.\nschemes:\n- name: oauth2\n  type: oauth2\n  spec: OAuth 2.1 with PKCE (S256)\n  issuer: https://xquik.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://xquik.com/api/oauth/authorize\n    tokenUrl: https://xquik.com/api/oauth/token\n    revocationUrl: https://xquik.com/api/oauth/revoke\n    registrationUrl:\
  \ https://xquik.com/api/oauth/register\n    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [none, client_secret_post]\n    client_id_metadata_document_supported: true\n  sources:\n  - https://xquik.com/.well-known/oauth-authorization-server\n  - https://xquik.com/.well-known/oauth-protected-resource/mcp\n  - a2a/xquik-agent-card.json\nscopes:\n- scope: mcp:tools\n  description: Run approved Xquik MCP tools.\n  flows: [authorizationCode]\n  resources: [https://xquik.com/mcp]\n  sources:\n  - https://xquik.com/.well-known/oauth-authorization-server\n  - https://xquik.com/.well-known/oauth-protected-resource/mcp\n  - https://xquik.com/mcp (WWW-Authenticate challenge, scope=\"mcp:tools\")\nprotected_resources:\n- resource: https://xquik.com/mcp\n  name: Xquik MCP Server\n  authorization_servers: [https://xquik.com]\n  bearer_methods_supported: [header]\n  scopes_supported: [mcp:tools]\n  documentation: https://docs.xquik.com/mcp/overview\n\
  note: >-\n  One scope, not a granular permission model. An mcp:tools token inherits whatever the\n  underlying account may do; read/write separation is enforced by the credential type\n  (guest paid_reads key vs full account key) rather than by scope. The agent card carried\n  read/write scopes when this repo was first profiled on 2026-08-01; the live card now\n  carries mcp:tools, matching the authorization server.\nx-evidence:\n  fetched: '2026-08-13'\n  urls:\n  - url: https://xquik.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://xquik.com/.well-known/oauth-protected-resource/mcp\n    status: 200\n  - url: https://xquik.com/mcp\n    status: 401\n    www_authenticate: Bearer realm=\"OAuth\", resource_metadata=\"https://xquik.com/.well-known/oauth-protected-resource/mcp\", scope=\"mcp:tools\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xquik-api/refs/heads/main/scopes/xquik-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- social media data
- X / Twitter
- social listening
- data extraction
- automation
- webhooks
- MCP
- developer API
token_urls:
- https://xquik.com/api/oauth/token
---
