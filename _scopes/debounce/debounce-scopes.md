---
api_specs:
- filename: debounce-validation-api-openapi.yml
  format: yaml
  label: DeBounce Validation API
  slug: debounce-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-validation-api-openapi.yml
- filename: debounce-bulk-api-openapi.yml
  format: yaml
  label: DeBounce Bulk API
  slug: debounce-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-bulk-api-openapi.yml
- filename: debounce-data-api-openapi.yml
  format: yaml
  label: DeBounce Data API
  slug: debounce-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-data-api-openapi.yml
- filename: debounce-account-api-openapi.yml
  format: yaml
  label: DeBounce Account API
  slug: debounce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-account-api-openapi.yml
- filename: debounce-disposable-api-openapi.yml
  format: yaml
  label: DeBounce Disposable Detector API
  slug: debounce-disposable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/openapi/debounce-disposable-api-openapi.yml
authorization_urls:
- https://debounce.com/wp-admin/admin.php?page=novamira-oauth-authorize
description: DeBounce's REST validation API declares NO oauth2 security scheme — it is an api-key-in-query surface end to end (see authentication/). The one OAuth authorization server DeBounce operates is bound to the WordPress-hosted MCP endpoint on the marketing site, and it publishes exactly one scope. This file records that scope surface as probed from the provider's own RFC 8414 metadata; no scope reference page is published, and none is invented here.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Debounce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DeBounce publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DeBounce API on a user''s behalf.


  Tokens are issued from https://debounce.com/wp-json/novamira/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DeBounce
provider_slug: debounce
schemes:
- flows:
  - authorizationUrl: https://debounce.com/wp-admin/admin.php?page=novamira-oauth-authorize
    flow: authorizationCode
    refreshUrl: https://debounce.com/wp-json/novamira/v1/oauth/token
    tokenUrl: https://debounce.com/wp-json/novamira/v1/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://debounce.com/wp-json/novamira/v1/oauth/introspect
  issuer: https://debounce.com
  name: novamira-oauth
  pkce:
  - S256
  registration_endpoint: https://debounce.com/wp-json/novamira/v1/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://debounce.com/wp-json/novamira/v1/oauth/revoke
  source: well-known/debounce-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope the authorization server advertises. Grants a client access to the protected MCP resource at https://debounce.com/wp-json/mcp/novamira-oauth. The provider publishes no finer-grained breakdown of what the scope permits.
  flows:
  - authorizationCode
  scope: mcp
slug: debounce-scopes
source_filename: debounce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://debounce.com/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  DeBounce's REST validation API declares NO oauth2 security scheme — it is an\n  api-key-in-query surface end to end (see authentication/). The one OAuth\n  authorization server DeBounce operates is bound to the WordPress-hosted MCP\n  endpoint on the marketing site, and it publishes exactly one scope. This file\n  records that scope surface as probed from the provider's own RFC 8414 metadata;\n  no scope reference page is published, and none is invented here.\n\napplies_to:\n  resource: https://debounce.com/wp-json/mcp/novamira-oauth\n  kind: mcp-server\n  not_applicable_to:\n  - https://api.debounce.io\n  - https://bulk.debounce.io\n  - https://disposable.debounce.io\n  - https://logo.debounce.com\n\nschemes:\n- name: novamira-oauth\n  type: oauth2\n  source: well-known/debounce-oauth-authorization-server.json\n  issuer: https://debounce.com\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://debounce.com/wp-admin/admin.php?page=novamira-oauth-authorize\n    tokenUrl: https://debounce.com/wp-json/novamira/v1/oauth/token\n    refreshUrl: https://debounce.com/wp-json/novamira/v1/oauth/token\n  pkce:\n  - S256\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - none\n  registration_endpoint: https://debounce.com/wp-json/novamira/v1/oauth/register\n  revocation_endpoint: https://debounce.com/wp-json/novamira/v1/oauth/revoke\n  introspection_endpoint: https://debounce.com/wp-json/novamira/v1/oauth/introspect\n\nscopes:\n- scope: mcp\n  description: >-\n    The single scope the authorization server advertises. Grants a client access\n    to the protected MCP resource at\n    https://debounce.com/wp-json/mcp/novamira-oauth. The provider publishes no\n    finer-grained breakdown of what the scope permits.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - well-known/debounce-oauth-authorization-server.json\n  - well-known/debounce-oauth-protected-resource.json\n\nsummary:\n  scope_count: 1\n  oauth2_on_the_rest_api: false\n\nx-evidence:\n- url: https://debounce.com/.well-known/oauth-authorization-server\n  fetched: '2026-08-14'\n  http_status: 200\n- url: https://debounce.com/.well-known/oauth-protected-resource\n  fetched: '2026-08-14'\n  http_status: 200\n- url: https://debounce.com/wp-json/mcp/novamira-oauth\n  fetched: '2026-08-14'\n  http_status: 401\n  note: tools/list rejected with rest_oauth_required, confirming the resource is live and gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debounce/refs/heads/main/scopes/debounce-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Email Validation
- Email Verification
- Deliverability
- Disposable Email Detection
- MX Records
- Bulk Email Validation
- Data Enrichment
- Syntax Validation
- Reverse Email Lookup
- Logo API
token_urls:
- https://debounce.com/wp-json/novamira/v1/oauth/token
---
