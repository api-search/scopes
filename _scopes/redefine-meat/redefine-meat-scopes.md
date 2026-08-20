---
api_specs:
- filename: redefine-meat-wc-store-v1-api-openapi.yml
  format: yaml
  label: Redefine Meat Wc/store/v1 API
  slug: redefine-meat-wc-store-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/openapi/redefine-meat-wc-store-v1-api-openapi.yml
- filename: redefine-meat-wp-v2-api-openapi.yml
  format: yaml
  label: Redefine Meat Wp/v2 API
  slug: redefine-meat-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/openapi/redefine-meat-wp-v2-api-openapi.yml
authorization_urls:
- https://www.redefinemeat.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Redefine Meat Scopes
name_suffix: OAuth Scopes
note: Redefine Meat publishes no scope reference page - it runs no developer program. The single scope below is read verbatim from the RFC 8414 authorization-server metadata the site serves for its Model Context Protocol endpoints. No OpenAPI on this host declares an oauth2 securityScheme, so nothing was derived from a spec.
overview: 'Redefine Meat publishes 1 OAuth 2.0 scope via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Redefine Meat API on a user''s behalf.


  Tokens are issued from https://www.redefinemeat.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Redefine Meat
provider_slug: redefine-meat
schemes:
- flows:
  - authorizationUrl: https://www.redefinemeat.com/oauth/authorize
    client_registration: client_id_metadata_document
    flow: authorizationCode
    pkce:
    - S256
    revocationUrl: https://www.redefinemeat.com/oauth/revoke
    tokenUrl: https://www.redefinemeat.com/oauth/token
    token_endpoint_auth_methods:
    - none
  - flow: refreshToken
    tokenUrl: https://www.redefinemeat.com/oauth/token
  issuer: https://www.redefinemeat.com
  name: mcp-oauth
  source: https://www.redefinemeat.com/.well-known/oauth-authorization-server
  spec: RFC 8414 OAuth 2.0 Authorization Server Metadata
scope_count: 1
scope_names:
- mcp
scopes:
- description: The only scope advertised by the authorization server. Required as a bearer token scope on the protected resource https://www.redefinemeat.com/wp-json/mcp/mcp-oauth-server. What it grants is not published; the tool set behind it returned HTTP 401 anonymously.
  flows:
  - authorizationCode
  - refreshToken
  scope: mcp
slug: redefine-meat-scopes
source_filename: redefine-meat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://www.redefinemeat.com/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  Redefine Meat publishes no scope reference page - it runs no developer program. The single\n  scope below is read verbatim from the RFC 8414 authorization-server metadata the site serves\n  for its Model Context Protocol endpoints. No OpenAPI on this host declares an oauth2\n  securityScheme, so nothing was derived from a spec.\nschemes:\n- name: mcp-oauth\n  source: https://www.redefinemeat.com/.well-known/oauth-authorization-server\n  spec: RFC 8414 OAuth 2.0 Authorization Server Metadata\n  issuer: https://www.redefinemeat.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.redefinemeat.com/oauth/authorize\n    tokenUrl: https://www.redefinemeat.com/oauth/token\n    revocationUrl: https://www.redefinemeat.com/oauth/revoke\n    pkce: [S256]\n    token_endpoint_auth_methods: [none]\n    client_registration:\
  \ client_id_metadata_document\n  - flow: refreshToken\n    tokenUrl: https://www.redefinemeat.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    The only scope advertised by the authorization server. Required as a bearer token scope on\n    the protected resource https://www.redefinemeat.com/wp-json/mcp/mcp-oauth-server. What it\n    grants is not published; the tool set behind it returned HTTP 401 anonymously.\n  flows: [authorizationCode, refreshToken]\n  sources:\n  - https://www.redefinemeat.com/.well-known/oauth-authorization-server\n  - https://www.redefinemeat.com/.well-known/oauth-protected-resource\nprotected_resources:\n- resource: https://www.redefinemeat.com/wp-json/mcp/mcp-oauth-server\n  authorization_servers: [https://www.redefinemeat.com]\n  bearer_methods_supported: [header]\n  scopes_supported: [mcp]\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://www.redefinemeat.com/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n  - url: https://www.redefinemeat.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redefine-meat/refs/heads/main/scopes/redefine-meat-scopes.yml
summary_line: 1 scope · authorizationCode/refreshToken
tags:
- Food and Beverage
- Alternative Protein
- Plant-Based
- Food Technology
- Manufacturing
- E-Commerce
- WooCommerce
- WordPress
- Retail
- MCP
token_urls:
- https://www.redefinemeat.com/oauth/token
---
