---
api_specs:
- filename: a2-biotherapeutics-wp-rest-openapi.yml
  format: yaml
  label: A2 Biotherapeutics WordPress REST API
  slug: a2-biotherapeutics-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/openapi/a2-biotherapeutics-wp-rest-openapi.yml
authorization_urls:
- https://www.a2bio.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: A2 Biotherapeutics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'A2 Biotherapeutics publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the A2 Biotherapeutics API on a user''s behalf.


  Tokens are issued from https://www.a2bio.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: A2 Biotherapeutics
provider_slug: a2-biotherapeutics
schemes:
- description: OAuth 2.1 authorization-code + PKCE, as advertised by the provider's RFC 8414 metadata at https://www.a2bio.com/.well-known/oauth-authorization-server (fetched 2026-08-02, HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names https://www.a2bio.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://www.a2bio.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.a2bio.com/oauth/token
  name: mcpOAuth2
  source: openapi/a2-biotherapeutics-wp-rest-openapi.yml
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the site's Model Context Protocol server.
  flows:
  - authorizationCode
  scope: mcp
slug: a2-biotherapeutics-scopes
source_filename: a2-biotherapeutics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/a2-biotherapeutics-wp-rest-openapi.yml\nschemes:\n- name: mcpOAuth2\n  source: openapi/a2-biotherapeutics-wp-rest-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.a2bio.com/oauth/authorize\n    tokenUrl: https://www.a2bio.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE, as advertised by the provider's RFC 8414\n    metadata at https://www.a2bio.com/.well-known/oauth-authorization-server (fetched 2026-08-02,\n    HTTP 200). Guards the `mcp` namespace; the protected-resource metadata (RFC 9728) names\n    https://www.a2bio.com/wp-json/mcp/mcp-oauth-server.\nscopes:\n- scope: mcp\n  description: Access the site's Model Context Protocol server.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/a2-biotherapeutics-wp-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a2-biotherapeutics/refs/heads/main/scopes/a2-biotherapeutics-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Immuno-Oncology
- Oncology
- Pharmaceuticals
- Clinical Trials
- Healthcare
- Model Context Protocol
- WordPress
token_urls:
- https://www.a2bio.com/oauth/token
---
