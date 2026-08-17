---
api_specs:
- filename: konbiniapi-instagram-api-openapi.yml
  format: yaml
  label: KonbiniAPI Instagram API
  slug: konbiniapi-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-instagram-api-openapi.yml
- filename: konbiniapi-tiktok-api-openapi.yml
  format: yaml
  label: KonbiniAPI TikTok API
  slug: konbiniapi-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-tiktok-api-openapi.yml
- filename: konbiniapi-x-api-openapi.yml
  format: yaml
  label: KonbiniAPI X API
  slug: konbiniapi-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-x-api-openapi.yml
- filename: konbiniapi-reddit-api-openapi.yml
  format: yaml
  label: KonbiniAPI Reddit API
  slug: konbiniapi-reddit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-reddit-api-openapi.yml
- filename: konbiniapi-linkedin-api-openapi.yml
  format: yaml
  label: KonbiniAPI LinkedIn API
  slug: konbiniapi-linkedin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/openapi/konbiniapi-linkedin-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.konbiniapi.com/reference/mcp/overview
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Konbiniapi Scopes
name_suffix: OAuth Scopes
note: These scopes govern the hosted MCP server only. The REST API at api.konbiniapi.com uses a static Bearer API key with NO scopes at all — one key carries the whole surface, all 67 operations, with no way to issue a read-only or platform-restricted credential. The OpenAPI declares no oauth2 securityScheme, so `derive-oauth-scopes.py` correctly found nothing; every scope below was read from live authorization-server metadata instead.
overview: 'KonbiniAPI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: KonbiniAPI
provider_slug: konbiniapi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: konbiniapi-scopes
source_filename: konbiniapi-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.konbiniapi.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.konbiniapi.com/.well-known/oauth-authorization-server\nsources:\n  - https://mcp.konbiniapi.com/.well-known/oauth-authorization-server\n  - https://mcp.konbiniapi.com/.well-known/oauth-protected-resource\n  - https://app.konbiniapi.com/.well-known/openid-configuration/api/auth\ndocs: https://docs.konbiniapi.com/reference/mcp/overview\nnote: >-\n  These scopes govern the hosted MCP server only. The REST API at api.konbiniapi.com uses a static\n  Bearer API key with NO scopes at all — one key carries the whole surface, all 67 operations, with\n  no way to issue a read-only or platform-restricted credential. The OpenAPI declares no oauth2\n  securityScheme, so `derive-oauth-scopes.py` correctly found nothing; every scope below was read\n  from live authorization-server metadata instead.\nauthorization_server: https://app.konbiniapi.com/api/auth\nprotected_resource: https://mcp.konbiniapi.com\nscope_count: 5\nscopes:\n\
  \  - name: api_key\n    description: >-\n      Authorizes the MCP server to call KonbiniAPI on the account's behalf using its API key, and to\n      spend that account's credits. This is the only scope that grants data access, and it grants all\n      of it — there is no per-platform or read-only subdivision.\n    resource: https://mcp.konbiniapi.com\n    granted_by: protected-resource metadata\n    consequence: read\n  - name: offline_access\n    description: >-\n      Issues a refresh token so an agent can keep calling without the user present. Required for\n      unattended automation (Zapier, n8n, Make, Pipedream).\n    resource: https://mcp.konbiniapi.com\n    granted_by: protected-resource metadata\n    consequence: read\n  - name: openid\n    description: Standard OIDC scope; requests an ID token identifying the signed-in KonbiniAPI account.\n    resource: https://app.konbiniapi.com/api/auth\n    granted_by: authorization-server metadata\n    consequence: identity\n  - name: profile\n\
  \    description: Standard OIDC scope; releases name, picture, given_name and family_name claims.\n    resource: https://app.konbiniapi.com/api/auth\n    granted_by: authorization-server metadata\n    consequence: identity\n  - name: email\n    description: Standard OIDC scope; releases the email and email_verified claims.\n    resource: https://app.konbiniapi.com/api/auth\n    granted_by: authorization-server metadata\n    consequence: identity\ngrants:\n  - authorization_code\n  - client_credentials\n  - refresh_token\npkce:\n  - S256\nclaims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - sid\n  - scope\n  - azp\n  - email\n  - email_verified\n  - name\n  - picture\n  - family_name\n  - given_name\ngaps:\n  - >-\n    No read-only scope. Every KonbiniAPI operation is a read, so this costs nothing today, but it\n    also means a consumer cannot narrow a delegated token below \"all five platforms\".\n  - >-\n    No per-platform scope (e.g. tiktok:read). An agent granted api_key\
  \ can call LinkedIn and Reddit\n    even if it was authorized for a TikTok task.\n  - >-\n    No spend-limiting scope. api_key implies the ability to consume the account's entire credit\n    balance; the only ceiling is the plan.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konbiniapi/refs/heads/main/scopes/konbiniapi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API
- Social Media
- Instagram
- TikTok
- X
- Reddit
- LinkedIn
- ActivityStreams 2.0
- Scraping
- Data Extraction
- Public Data
- Influencer Marketing
- Social Listening
- Creator Tools
- MCP
- Model Context Protocol
- Agent Skills
- Agents
token_urls: []
---
