---
api_specs:
- filename: engrail-therapeutics-content-openapi.yml
  format: yaml
  label: Engrail Therapeutics Site Content API
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrail-therapeutics/refs/heads/main/openapi/engrail-therapeutics-content-openapi.yml
authorization_urls:
- https://www.engrail.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Engrail Therapeutics Scopes
name_suffix: OAuth Scopes
note: Not derivable from OpenAPI — the content API declares no oauth2 security scheme. The single scope below is published verbatim in the provider's own RFC 8414 Authorization Server Metadata and corroborated by its RFC 9728 Protected Resource Metadata. Engrail publishes no scopes/permissions reference page; `mcp` is the entire scope surface as advertised.
overview: 'Engrail Therapeutics publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Engrail Therapeutics API on a user''s behalf.


  Tokens are issued from https://www.engrail.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Engrail Therapeutics
provider_slug: engrail-therapeutics
schemes:
- flows:
  - authorizationUrl: https://www.engrail.com/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    revocationUrl: https://www.engrail.com/oauth/revoke
    tokenUrl: https://www.engrail.com/oauth/token
  issuer: https://www.engrail.com
  name: mcpOAuth
  source: well-known/engrail-therapeutics-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants a bearer token access to the site's Model Context Protocol servers at https://www.engrail.com/wp-json/mcp/mcp-oauth-server. This is a single coarse-grained scope — the provider publishes no finer-grained read/write split, so what a token can actually do is determined server-side by the underlying WordPress capability model rather than by scope.
  flows:
  - authorizationCode
  scope: mcp
slug: engrail-therapeutics-scopes
source_filename: engrail-therapeutics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://www.engrail.com/.well-known/oauth-authorization-server\nnote: >-\n  Not derivable from OpenAPI — the content API declares no oauth2 security scheme. The single scope\n  below is published verbatim in the provider's own RFC 8414 Authorization Server Metadata and\n  corroborated by its RFC 9728 Protected Resource Metadata. Engrail publishes no scopes/permissions\n  reference page; `mcp` is the entire scope surface as advertised.\nschemes:\n- name: mcpOAuth\n  source: well-known/engrail-therapeutics-oauth-authorization-server.json\n  issuer: https://www.engrail.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.engrail.com/oauth/authorize\n    tokenUrl: https://www.engrail.com/oauth/token\n    revocationUrl: https://www.engrail.com/oauth/revoke\n    code_challenge_methods_supported:\n    - S256\nscopes:\n- scope: mcp\n  description: >-\n    Grants a bearer token access to the site's Model Context\
  \ Protocol servers at\n    https://www.engrail.com/wp-json/mcp/mcp-oauth-server. This is a single coarse-grained scope — the\n    provider publishes no finer-grained read/write split, so what a token can actually do is\n    determined server-side by the underlying WordPress capability model rather than by scope.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/engrail-therapeutics-oauth-authorization-server.json\n  - well-known/engrail-therapeutics-oauth-protected-resource.json\nobservations:\n- Only one scope is advertised, so scope-based least privilege is not achievable by a client.\n- token_endpoint_auth_methods_supported is [\"none\"] — public clients only, PKCE S256 required.\n- client_id_metadata_document_supported is true, so clients are identified by a URL-dereferenceable\n  metadata document instead of dynamic client registration.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://www.engrail.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type:\
  \ application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engrail-therapeutics/refs/heads/main/scopes/engrail-therapeutics-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Neuroscience
- Clinical Trials
- Drug Development
- Healthcare
- Mental Health
- Model Context Protocol
token_urls:
- https://www.engrail.com/oauth/token
---
