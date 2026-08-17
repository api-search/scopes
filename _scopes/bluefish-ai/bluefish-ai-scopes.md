---
authorization_urls:
- https://platform.bluefishai.com/connected-apps/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Bluefish Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bluefish AI publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bluefish AI API on a user''s behalf.


  Tokens are issued from https://auth.bluefishai.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bluefish AI
provider_slug: bluefish-ai
schemes:
- flows:
  - authorizationUrl: https://platform.bluefishai.com/connected-apps/authorize
    flow: authorizationCode
    tokenUrl: https://auth.bluefishai.com/v1/oauth2/token
  issuer: https://auth.bluefishai.com
  name: BluefishOAuth2
  source: well-known/bluefish-ai-oauth-authorization-server.json
scope_count: 7
scope_names:
- mcp:connect
- full_access
- openid
- offline_access
- profile
- email
- phone
scopes:
- description: Bluefish-specific. Declared by the MCP endpoint's own RFC 9728 protected-resource metadata as a supported scope for the resource https://platform.bluefishai.com/mcp, so it is the scope that gates agent access to the MCP server. Bluefish publishes no prose definition of it.
  flows:
  - authorizationCode
  scope: mcp:connect
- description: Bluefish-specific. Advertised only by the OpenID Connect discovery document, not by the RFC 8414 document. No published definition; the name is recorded as served without inferring what it grants.
  flows:
  - authorizationCode
  scope: full_access
- description: Standard OIDC scope requesting an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope requesting a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Standard OIDC claim scope for basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC claim scope for the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC claim scope for the phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
slug: bluefish-ai-scopes
source_filename: bluefish-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.bluefishai.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Bluefish publishes no scopes or permissions reference page — there is no developer\n  portal, no docs host and no llms.txt. The scope list below is taken verbatim from\n  the scopes_supported arrays of the provider's own live RFC 8414 and OIDC discovery\n  documents. Descriptions are the standard OIDC/OAuth meanings for the registered\n  scope names; the two Bluefish-specific scopes (mcp:connect, full_access) are\n  recorded with the endpoint evidence for what they gate and are NOT given invented\n  descriptions.\nschemes:\n- name: BluefishOAuth2\n  source: well-known/bluefish-ai-oauth-authorization-server.json\n  issuer: https://auth.bluefishai.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.bluefishai.com/connected-apps/authorize\n    tokenUrl: https://auth.bluefishai.com/v1/oauth2/token\nscopes:\n\
  - scope: mcp:connect\n  description: >-\n    Bluefish-specific. Declared by the MCP endpoint's own RFC 9728 protected-resource\n    metadata as a supported scope for the resource\n    https://platform.bluefishai.com/mcp, so it is the scope that gates agent access\n    to the MCP server. Bluefish publishes no prose definition of it.\n  flows: [authorizationCode]\n  sources:\n  - well-known/bluefish-ai-oauth-protected-resource.json\n  - well-known/bluefish-ai-oauth-authorization-server.json\n  - well-known/bluefish-ai-openid-configuration.json\n  gates: https://platform.bluefishai.com/mcp\n- scope: full_access\n  description: >-\n    Bluefish-specific. Advertised only by the OpenID Connect discovery document, not\n    by the RFC 8414 document. No published definition; the name is recorded as served\n    without inferring what it grants.\n  flows: [authorizationCode]\n  sources: [well-known/bluefish-ai-openid-configuration.json]\n- scope: openid\n  description: Standard OIDC scope requesting\
  \ an ID token.\n  flows: [authorizationCode]\n  sources:\n  - well-known/bluefish-ai-oauth-protected-resource.json\n  - well-known/bluefish-ai-oauth-authorization-server.json\n  - well-known/bluefish-ai-openid-configuration.json\n- scope: offline_access\n  description: Standard OIDC scope requesting a refresh token for long-lived access.\n  flows: [authorizationCode]\n  sources:\n  - well-known/bluefish-ai-oauth-protected-resource.json\n  - well-known/bluefish-ai-oauth-authorization-server.json\n  - well-known/bluefish-ai-openid-configuration.json\n- scope: profile\n  description: Standard OIDC claim scope for basic profile claims.\n  flows: [authorizationCode]\n  sources:\n  - well-known/bluefish-ai-oauth-authorization-server.json\n  - well-known/bluefish-ai-openid-configuration.json\n- scope: email\n  description: Standard OIDC claim scope for the email and email_verified claims.\n  flows: [authorizationCode]\n  sources:\n  - well-known/bluefish-ai-oauth-authorization-server.json\n \
  \ - well-known/bluefish-ai-openid-configuration.json\n- scope: phone\n  description: Standard OIDC claim scope for the phone_number and phone_number_verified claims.\n  flows: [authorizationCode]\n  sources:\n  - well-known/bluefish-ai-oauth-authorization-server.json\n  - well-known/bluefish-ai-openid-configuration.json\nscope_count: 7\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: 'https://auth.bluefishai.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://auth.bluefishai.com/.well-known/openid-configuration', status: 200}\n  - {url: 'https://platform.bluefishai.com/.well-known/oauth-protected-resource/mcp', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluefish-ai/refs/heads/main/scopes/bluefish-ai-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Marketing
- Artificial Intelligence
- Generative Engine Optimization
- Brand Safety
- Agentic Commerce
- Analytics
- MCP
- Agents
token_urls:
- https://auth.bluefishai.com/v1/oauth2/token
---
