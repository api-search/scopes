---
api_specs:
- filename: spekit-openapi.yml
  format: yaml
  label: Spekit API
  slug: spekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/openapi/spekit-openapi.yml
authorization_urls:
- https://mcp.spekit.co/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Spekit Scopes
name_suffix: OAuth Scopes
note: The OAuth surface is the MCP connector, not the REST API — the published OpenAPI declares only an apiKey scheme and no oauth2 flows, so derive-oauth-scopes.py found nothing. These scopes come from Spekit's own RFC 8414 and RFC 9728 discovery documents, fetched anonymously. Spekit publishes no scopes/permissions reference page in its help center; the scope set below is what the authorization server itself advertises.
overview: 'Spekit publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spekit API on a user''s behalf.


  Tokens are issued from https://mcp.spekit.co/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spekit
provider_slug: spekit
schemes:
- flows:
  - authorizationUrl: https://mcp.spekit.co/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://mcp.spekit.co/register
    tokenUrl: https://mcp.spekit.co/token
  issuer: https://mcp.spekit.co/
  name: mcp-oauth2
  resource: https://mcp.spekit.co/mcp
  source: https://mcp.spekit.co/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- read
scopes:
- description: OpenID Connect — issue an ID token identifying the signing-in Spekit user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated Spekit user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address of the authenticated Spekit user.
  flows:
  - authorizationCode
  scope: email
- description: The only Spekit-specific scope advertised. Note the asymmetry — the connector ships 7 write tools (create topic/content/company/deal room, create content from template, update content, create deal room content) but the authorization server advertises no corresponding write scope. Write authority is not carried in the OAuth scope at all; it is decided server-side from the signed-in user's Spekit role, and Spekit states there is no setting that forces the connector read-only independent of that role. A client cannot request a read-only grant.
  flows:
  - authorizationCode
  scope: read
slug: spekit-scopes
source_filename: spekit-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.spekit.co/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.spekit.co/.well-known/oauth-authorization-server\nsources:\n- https://mcp.spekit.co/.well-known/oauth-authorization-server\n- https://mcp.spekit.co/.well-known/oauth-protected-resource/mcp\nnote: >-\n  The OAuth surface is the MCP connector, not the REST API — the published OpenAPI declares only\n  an apiKey scheme and no oauth2 flows, so derive-oauth-scopes.py found nothing. These scopes come\n  from Spekit's own RFC 8414 and RFC 9728 discovery documents, fetched anonymously. Spekit\n  publishes no scopes/permissions reference page in its help center; the scope set below is what\n  the authorization server itself advertises.\nschemes:\n- name: mcp-oauth2\n  source: https://mcp.spekit.co/.well-known/oauth-authorization-server\n  issuer: https://mcp.spekit.co/\n  resource: https://mcp.spekit.co/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.spekit.co/authorize\n    tokenUrl: https://mcp.spekit.co/token\n\
  \    registrationUrl: https://mcp.spekit.co/register\n    code_challenge_methods: [S256]\nscopes:\n- scope: openid\n  description: OpenID Connect — issue an ID token identifying the signing-in Spekit user.\n  flows: [authorizationCode]\n  sources: [https://mcp.spekit.co/.well-known/oauth-authorization-server]\n- scope: profile\n  description: Basic profile claims for the authenticated Spekit user.\n  flows: [authorizationCode]\n  sources: [https://mcp.spekit.co/.well-known/oauth-authorization-server]\n- scope: email\n  description: Email address of the authenticated Spekit user.\n  flows: [authorizationCode]\n  sources: [https://mcp.spekit.co/.well-known/oauth-authorization-server]\n- scope: read\n  description: >-\n    The only Spekit-specific scope advertised. Note the asymmetry — the connector ships 7 write\n    tools (create topic/content/company/deal room, create content from template, update content,\n    create deal room content) but the authorization server advertises no corresponding\
  \ write\n    scope. Write authority is not carried in the OAuth scope at all; it is decided server-side\n    from the signed-in user's Spekit role, and Spekit states there is no setting that forces the\n    connector read-only independent of that role. A client cannot request a read-only grant.\n  flows: [authorizationCode]\n  sources: [https://mcp.spekit.co/.well-known/oauth-authorization-server]\nscope_count: 4\ndocs: null\ndocs_note: No scopes or permissions reference page is published; scopes are only discoverable from the AS metadata document.\nchecked: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spekit/refs/heads/main/scopes/spekit-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Software-as-a-Service
- Sales Enablement
- Revenue Enablement
- Digital Adoption
- Knowledge-Management
- MCP
- Artificial Intelligence
- Analytics
- Sales
- Content Management
- Agents
- Authentication
token_urls:
- https://mcp.spekit.co/token
---
