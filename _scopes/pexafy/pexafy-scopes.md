---
api_specs:
- filename: pexafy-collections-api-openapi.yml
  format: yaml
  label: Pexafy Collections API
  slug: pexafy-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-collections-api-openapi.yml
- filename: pexafy-facets-api-openapi.yml
  format: yaml
  label: Pexafy Facets API
  slug: pexafy-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-facets-api-openapi.yml
- filename: pexafy-photos-api-openapi.yml
  format: yaml
  label: Pexafy Photos API
  slug: pexafy-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-photos-api-openapi.yml
- filename: pexafy-search-api-openapi.yml
  format: yaml
  label: Pexafy Search API
  slug: pexafy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-search-api-openapi.yml
- filename: pexafy-usage-api-openapi.yml
  format: yaml
  label: Pexafy Usage API
  slug: pexafy-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-usage-api-openapi.yml
authorization_urls:
- https://pexafy.com/oauth/authorize/
description: ''
docs: https://pexafy.com/.well-known/api-onboarding
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Pexafy Scopes
name_suffix: OAuth Scopes
note: '0-working/derive-oauth-scopes.py found nothing: neither published OpenAPI declares an oauth2 securityScheme, so the scope surface is invisible to a spec-only derivation. It is real all the same — RFC 8414 metadata on pexafy.com advertises the authorization server, RFC 9728 metadata on mcp.pexafy.com names the scope the MCP resource requires, and the provider''s api-onboarding descriptor documents the role model behind the two scopes.'
overview: 'Pexafy publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pexafy API on a user''s behalf.


  Tokens are issued from https://pexafy.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pexafy
provider_slug: pexafy
schemes:
- dynamic_client_registration: https://pexafy.com/oauth/register
  flows:
  - authorizationUrl: https://pexafy.com/oauth/authorize/
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://pexafy.com/oauth/token/
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://pexafy.com/
  name: PexafyOAuth
  source: https://pexafy.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Search, photo lookups and facets. The api-onboarding descriptor states dashboard keys carry read and write; read covers everything that does not mutate a collection.
  flows:
  - authorizationCode
  scope: read
- description: The caller's own collections — create, delete, add and remove photos. The versioned OpenAPI description says a read-scoped key gets a 403 on anything under /collections.
  flows:
  - authorizationCode
  scope: write
slug: pexafy-scopes
source_filename: pexafy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: https://pexafy.com/.well-known/oauth-authorization-server\ndocs: https://pexafy.com/.well-known/api-onboarding\nnote: >-\n  0-working/derive-oauth-scopes.py found nothing: neither published OpenAPI declares an\n  oauth2 securityScheme, so the scope surface is invisible to a spec-only derivation. It is\n  real all the same — RFC 8414 metadata on pexafy.com advertises the authorization server,\n  RFC 9728 metadata on mcp.pexafy.com names the scope the MCP resource requires, and the\n  provider's api-onboarding descriptor documents the role model behind the two scopes.\nschemes:\n- name: PexafyOAuth\n  source: https://pexafy.com/.well-known/oauth-authorization-server\n  issuer: https://pexafy.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://pexafy.com/oauth/authorize/\n    tokenUrl: https://pexafy.com/oauth/token/\n    code_challenge_methods: [S256]\n  dynamic_client_registration: https://pexafy.com/oauth/register\n\
  \  token_endpoint_auth_methods: [none, client_secret_post]\n  grant_types: [authorization_code, refresh_token]\nscopes:\n- scope: read\n  description: >-\n    Search, photo lookups and facets. The api-onboarding descriptor states dashboard keys\n    carry read and write; read covers everything that does not mutate a collection.\n  flows: [authorizationCode]\n  sources:\n  - https://pexafy.com/.well-known/oauth-authorization-server\n  - https://pexafy.com/.well-known/api-onboarding\n- scope: write\n  description: >-\n    The caller's own collections — create, delete, add and remove photos. The versioned\n    OpenAPI description says a read-scoped key gets a 403 on anything under /collections.\n  flows: [authorizationCode]\n  sources:\n  - https://pexafy.com/.well-known/oauth-authorization-server\n  - openapi/pexafy-api-v1-openapi.json\nresources:\n- resource: https://mcp.pexafy.com/mcp\n  authorization_servers: [https://pexafy.com/]\n  scopes_supported: [read]\n  bearer_methods_supported:\
  \ [header]\n  resource_name: Pexafy MCP\n  source: https://mcp.pexafy.com/.well-known/oauth-protected-resource\n  note: The MCP server requests read only — its three tools are all read-only, so it never asks for write.\ninternal_roles_not_granted:\n  note: >-\n    Verbatim from the api-onboarding descriptor: \"Admin and crawler roles are internal and\n    are never granted to user keys.\"\n  roles: [admin, crawler]\ngaps:\n- Neither OpenAPI document declares the oauth2 scheme or attaches scopes to operations, so scope requirements cannot be read per-operation from the contract.\n- There is no human-readable scopes/permissions reference page in the docs; the scope model is only discoverable from the two well-known documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/scopes/pexafy-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- images
- photos
- stock photos
- image search
- semantic search
- computer vision
- embeddings
- mcp
- agent-native
- content licensing
token_urls:
- https://pexafy.com/oauth/token/
---
