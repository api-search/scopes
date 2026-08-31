---
api_specs:
- filename: endeavor-biomedicines-mcp-api-openapi.yml
  format: yaml
  label: Endeavor BioMedicines MCP API
  slug: endeavor-biomedicines-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-mcp-api-openapi.yml
- filename: endeavor-biomedicines-oembed-1-0-api-openapi.yml
  format: yaml
  label: Endeavor BioMedicines Oembed/1.0 API
  slug: endeavor-biomedicines-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-oembed-1-0-api-openapi.yml
- filename: endeavor-biomedicines-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Endeavor BioMedicines Wp Abilities/v1 API
  slug: endeavor-biomedicines-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-wp-abilities-v1-api-openapi.yml
- filename: endeavor-biomedicines-wp-block-editor-v1-api-openapi.yml
  format: yaml
  label: Endeavor BioMedicines Wp Block Editor/v1 API
  slug: endeavor-biomedicines-wp-block-editor-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-wp-block-editor-v1-api-openapi.yml
- filename: endeavor-biomedicines-wp-site-health-v1-api-openapi.yml
  format: yaml
  label: Endeavor BioMedicines Wp Site Health/v1 API
  slug: endeavor-biomedicines-wp-site-health-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-wp-site-health-v1-api-openapi.yml
- filename: endeavor-biomedicines-wp-v2-api-openapi.yml
  format: yaml
  label: Endeavor BioMedicines Wp/v2 API
  slug: endeavor-biomedicines-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-wp-v2-api-openapi.yml
authorization_urls:
- https://endeavorbiomedicines.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Endeavor Biomedicines Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Endeavor BioMedicines publishes 1 OAuth 2.0 scope via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Endeavor BioMedicines API on a user''s behalf.


  Tokens are issued from https://endeavorbiomedicines.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Endeavor BioMedicines
provider_slug: endeavor-biomedicines
schemes:
- flows:
  - authorizationUrl: https://endeavorbiomedicines.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://endeavorbiomedicines.com/oauth/revoke
    tokenUrl: https://endeavorbiomedicines.com/oauth/token
    token_endpoint_auth_methods:
    - none
  - flow: refreshToken
    tokenUrl: https://endeavorbiomedicines.com/oauth/token
  issuer: https://endeavorbiomedicines.com
  name: OAuth 2.1 (WordPress MCP adapter)
  source: well-known/endeavor-biomedicines-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope advertised by both the authorization server and the protected resource. It gates the MCP endpoint at https://endeavorbiomedicines.com/wp-json/mcp/mcp-oauth-server. The provider publishes no description of what the scope grants; nothing further is asserted.
  flows:
  - authorizationCode
  - refreshToken
  scope: mcp
slug: endeavor-biomedicines-scopes
source_filename: endeavor-biomedicines-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://endeavorbiomedicines.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Endeavor BioMedicines publishes no OAuth or scopes documentation. Everything below\n  was read directly from the RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata that the host serves anonymously.\nschemes:\n- name: OAuth 2.1 (WordPress MCP adapter)\n  source: well-known/endeavor-biomedicines-oauth-authorization-server.json\n  issuer: https://endeavorbiomedicines.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://endeavorbiomedicines.com/oauth/authorize\n    tokenUrl: https://endeavorbiomedicines.com/oauth/token\n    revocationUrl: https://endeavorbiomedicines.com/oauth/revoke\n    pkce: S256\n    token_endpoint_auth_methods:\n    - none\n  - flow: refreshToken\n    tokenUrl: https://endeavorbiomedicines.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n   \
  \ The single scope advertised by both the authorization server and the protected\n    resource. It gates the MCP endpoint at\n    https://endeavorbiomedicines.com/wp-json/mcp/mcp-oauth-server. The provider\n    publishes no description of what the scope grants; nothing further is asserted.\n  flows:\n  - authorizationCode\n  - refreshToken\n  sources:\n  - well-known/endeavor-biomedicines-oauth-authorization-server.json\n  - well-known/endeavor-biomedicines-oauth-protected-resource.json\nprotected_resources:\n- resource: https://endeavorbiomedicines.com/wp-json/mcp/mcp-oauth-server\n  authorization_servers:\n  - https://endeavorbiomedicines.com\n  bearer_methods_supported:\n  - header\n  scopes_supported:\n  - mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/scopes/endeavor-biomedicines-scopes.yml
summary_line: 1 scope · authorizationCode/refreshToken
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Clinical Trials
- Healthcare
- Drug Development
- Content
- WordPress
token_urls:
- https://endeavorbiomedicines.com/oauth/token
---
