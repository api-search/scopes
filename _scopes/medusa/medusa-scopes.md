---
api_specs:
- filename: medusa-store-openapi.yaml
  format: yaml
  label: Medusa Store API
  slug: medusa-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/openapi/medusa-store-openapi.yaml
- filename: medusa-admin-openapi.yaml
  format: yaml
  label: Medusa Admin API
  slug: medusa-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/openapi/medusa-admin-openapi.yaml
authorization_urls: []
description: Medusa's Store and Admin REST APIs declare NO oauth2 security scheme — they authenticate with a JWT bearer token, a session cookie or an Admin secret API key, none of which carry scopes. The only OAuth surface Medusa operates is the one in front of the remote MCP server, and it publishes RFC 8414 authorization-server metadata anonymously. The three scopes below are what that document advertises; they are identity scopes for a Medusa Cloud login, not commerce permissions.
docs: https://docs.medusajs.com/learn/introduction/build-with-llms-ai/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Medusa Scopes
name_suffix: OAuth Scopes
note: There is no per-tool or per-resource scope. Access to the MCP server is all-or-nothing on a Medusa Cloud account, so an agent cannot be granted the documentation-search tool without also being granted the feedback-submission tool.
overview: 'Medusa uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Medusa
provider_slug: medusa
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: medusa-scopes
source_filename: medusa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://docs.medusajs.com/.well-known/oauth-authorization-server and\n  https://docs.medusajs.com/.well-known/oauth-protected-resource, fetched anonymously\n  2026-08-26 and saved verbatim to well-known/.\ndocs: https://docs.medusajs.com/learn/introduction/build-with-llms-ai/mcp-server\ndescription: >-\n  Medusa's Store and Admin REST APIs declare NO oauth2 security scheme — they authenticate\n  with a JWT bearer token, a session cookie or an Admin secret API key, none of which carry\n  scopes. The only OAuth surface Medusa operates is the one in front of the remote MCP\n  server, and it publishes RFC 8414 authorization-server metadata anonymously. The three\n  scopes below are what that document advertises; they are identity scopes for a Medusa\n  Cloud login, not commerce permissions.\napplies_to:\n  - medusa:medusa-mcp-server\ndoes_not_apply_to:\n  - medusa:medusa-store-api\n  - medusa:medusa-admin-api\nauthorization_server:\n\
  \  issuer: https://docs.medusajs.com\n  authorization_endpoint: https://cloud.medusajs.com/oauth/authorize\n  token_endpoint: https://api.prod.medusajs.cloud/v1/oauth/token\n  registration_endpoint: https://docs.medusajs.com/oauth/register\n  jwks_uri: https://api.prod.medusajs.cloud/.well-known/jwks.json\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [none]\n  code_challenge_methods_supported: [S256]\n  dynamic_client_registration: true\nprotected_resource:\n  resource: https://docs.medusajs.com\n  authorization_servers: [https://docs.medusajs.com]\nscopes:\n  - name: openid\n    description: OpenID Connect — issue an ID token identifying the Medusa Cloud account.\n    source: oauth-authorization-server scopes_supported\n  - name: email\n    description: Access to the account's email address claim.\n    source: oauth-authorization-server scopes_supported\n  - name: profile\n    description: Access\
  \ to the account's basic profile claims.\n    source: oauth-authorization-server scopes_supported\nscope_count: 3\nalternative_credential:\n  type: personal access key\n  usage: Bearer token in the Authorization header, in place of the OAuth flow.\n  source: https://docs.medusajs.com/learn/introduction/build-with-llms-ai/mcp-server\nnote: >-\n  There is no per-tool or per-resource scope. Access to the MCP server is all-or-nothing on\n  a Medusa Cloud account, so an agent cannot be granted the documentation-search tool\n  without also being granted the feedback-submission tool.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/scopes/medusa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- E-Commerce
- Headless Commerce
- Open-Source
- Commerce
- Storefront
- Order Management
- Node.js
- GraphQL
- Agentic Commerce
- MCP
token_urls: []
---
