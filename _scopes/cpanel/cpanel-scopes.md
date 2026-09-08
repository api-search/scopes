---
api_specs:
- filename: cpanel-uapi-openapi.yml
  format: yaml
  label: cPanel UAPI
  slug: uapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/openapi/cpanel-uapi-openapi.yml
- filename: cpanel-whm-api-openapi.yml
  format: yaml
  label: WHM API 1
  slug: whm-api-1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/openapi/cpanel-whm-api-openapi.yml
authorization_urls: []
description: 'OAuth scopes cPanel''s surfaces actually advertise. IMPORTANT SCOPE OF THIS FILE: neither the cPanel UAPI nor the WHM API uses OAuth. Both declare a single `BasicAuth` http securityScheme and authenticate with HTTP Basic or an `Authorization: cpanel|whm user:TOKEN` header, and cPanel''s authorization model is PRIVILEGES on an API token, not OAuth scopes — so there is no scope vocabulary for the 1,282 REST operations and none is invented here. The scopes below belong to the two OAuth-protected AGENT surfaces in cPanel''s orbit, both discovered from documents the providers serve.'
docs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cpanel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'cPanel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: cPanel
provider_slug: cpanel
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cpanel-scopes
source_filename: cpanel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://mcp.webpros.com/.well-known/oauth-protected-resource and\n  https://login.webpros.com/.well-known/openid-configuration and\n  https://api.docs.cpanel.net/.well-known/oauth-authorization-server, fetched anonymously 2026-09-05\ndocs: https://api.docs.cpanel.net/guides/guide-to-api-authentication/\nprovider: cPanel\nproviderId: cpanel\ndescription: >-\n  OAuth scopes cPanel's surfaces actually advertise. IMPORTANT SCOPE OF THIS FILE: neither the\n  cPanel UAPI nor the WHM API uses OAuth. Both declare a single `BasicAuth` http securityScheme\n  and authenticate with HTTP Basic or an `Authorization: cpanel|whm user:TOKEN` header, and\n  cPanel's authorization model is PRIVILEGES on an API token, not OAuth scopes — so there is no\n  scope vocabulary for the 1,282 REST operations and none is invented here. The scopes below\n  belong to the two OAuth-protected AGENT surfaces in cPanel's orbit, both discovered from\n  documents\
  \ the providers serve.\nsurfaces:\n  - name: WebPros MCP\n    resource: https://mcp.webpros.com/api/mcp\n    authorization_servers: [https://login.webpros.com/]\n    discovery: https://mcp.webpros.com/.well-known/oauth-protected-resource\n    http_status: 200\n    reached_from: >-\n      cPanel UAPI operation /WebProsMCP/get_connection_config, which returns this endpoint to a\n      cPanel user as their MCP connection snippet.\n    scopes:\n      - name: openid\n        description: OpenID Connect authentication; issues an id_token identifying the WebPros account.\n        standard: true\n      - name: profile\n        description: Standard OIDC profile claims for the linked WebPros account.\n        standard: true\n      - name: email\n        description: Standard OIDC email claim for the linked WebPros account.\n        standard: true\n      - name: offline_access\n        description: Refresh-token issuance so an agent can hold a session beyond the access-token lifetime.\n        standard:\
  \ true\n      - name: mcp\n        description: >-\n          The provider-specific scope that authorizes MCP tool invocation on\n          https://mcp.webpros.com/api/mcp. Its tool-level meaning is not published; tools/list\n          returns {\"type\":\"unauthorized\"} (HTTP 401) without it, so the granular permissions\n          behind this scope require an authenticated introspection to enumerate and are NOT\n          guessed here.\n        standard: false\n  - name: cPanel & WHM Developer Portal MCP\n    resource: https://api.docs.cpanel.net/mcp\n    authorization_servers: [https://auth.cloud.redocly.com]\n    discovery: https://api.docs.cpanel.net/.well-known/oauth-authorization-server\n    http_status: 200\n    note: >-\n      Documentation-portal OAuth supplied by the Redocly platform cPanel runs the portal on.\n      Anonymous callers already receive the full public tool set, so these scopes gate\n      non-public documentation teams rather than the API surface.\n    scopes:\n\
  \      - name: openid\n        description: OpenID Connect authentication against auth.cloud.redocly.com.\n        standard: true\n      - name: profile\n        description: Standard OIDC profile claims.\n        standard: true\n      - name: email\n        description: Standard OIDC email claim.\n        standard: true\n      - name: offline_access\n        description: Refresh-token issuance.\n        standard: true\nrest_api_authorization:\n  model: api-token-privileges\n  note: >-\n    UAPI and WHM API 1 authorize by ACCOUNT and by API-token privileges, not by OAuth scope. A\n    cPanel API token is created with full access via UAPI Tokens-create_full_access, and WHM\n    tokens are created and revoked via WHM API 1 Tokens-api_token_create and\n    Tokens-api_token_revoke; restriction is expressed as the privileges attached to the token\n    and the reseller/root permission model, plus server-profile roles which DISABLE whole\n    modules. See authentication/cpanel-authentication.yml.\n\
  \  references:\n    - https://api.docs.cpanel.net/cpanel/tokens/\n    - https://api.docs.cpanel.net/whm/tokens/\n    - https://api.docs.cpanel.net/guides/guide-to-api-privilege-escalation/\nsummary:\n  oauth_surfaces: 2\n  scope_count: 5\n  rest_operations_under_oauth: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cpanel/refs/heads/main/scopes/cpanel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Control Panel
- DNS
- Domains
- Email
- Hosting
- Reseller
- Server Administration
- Web Hosting
- WHM
token_urls: []
---
