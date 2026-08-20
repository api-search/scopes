---
api_specs:
- filename: moloco-ads-campaign-management-openapi.yml
  format: yaml
  label: Moloco Ads Campaign Management API
  slug: moloco-ads-campaign-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-ads-campaign-management-openapi.yml
- filename: moloco-cloud-auth-openapi.yml
  format: yaml
  label: Moloco Cloud Auth API
  slug: moloco-cloud-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-cloud-auth-openapi.yml
- filename: moloco-commerce-media-management-openapi.yml
  format: yaml
  label: Moloco Commerce Media Management API
  slug: moloco-commerce-media-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-management-openapi.yml
- filename: moloco-commerce-media-decision-openapi.yml
  format: yaml
  label: Moloco Commerce Media Decision API
  slug: moloco-commerce-media-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-decision-openapi.yml
- filename: moloco-commerce-media-event-openapi.yml
  format: yaml
  label: Moloco Commerce Media Event API
  slug: moloco-commerce-media-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-event-openapi.yml
- filename: moloco-commerce-media-webhooks-openapi.yml
  format: yaml
  label: Moloco Commerce Media Webhooks
  slug: moloco-commerce-media-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-webhooks-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Moloco Scopes
name_suffix: OAuth Scopes
note: 'Moloco''s published OpenAPI documents declare only apiKey security schemes (Authorization bearer token / x-api-key), so no scopes are derivable from the specs. The OAuth surface was found by probing the API host directly: api.moloco.cloud serves RFC 8414 authorization-server metadata, and mcp.moloco.cloud/mcp answers with an RFC 9728 WWW-Authenticate challenge naming the required scope. Scope descriptions below are the observed identifiers only — Moloco publishes no scope reference page, so no descriptions are asserted.'
overview: 'MOLOCO publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the MOLOCO API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MOLOCO
provider_slug: moloco
schemes: []
scope_count: 2
scope_names:
- cloudapi.read
- offline_access
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: cloudapi.read
- description: ''
  flows:
  - authorizationCode
  - refresh_token
  scope: offline_access
slug: moloco-scopes
source_filename: moloco-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://api.moloco.cloud/.well-known/oauth-authorization-server\nnote: >-\n  Moloco's published OpenAPI documents declare only apiKey security schemes (Authorization bearer token /\n  x-api-key), so no scopes are derivable from the specs. The OAuth surface was found by probing the API host\n  directly: api.moloco.cloud serves RFC 8414 authorization-server metadata, and mcp.moloco.cloud/mcp answers\n  with an RFC 9728 WWW-Authenticate challenge naming the required scope. Scope descriptions below are the\n  observed identifiers only — Moloco publishes no scope reference page, so no descriptions are asserted.\nauthorization_server:\n  issuer: https://api.moloco.cloud\n  authorization_endpoint: https://api.moloco.cloud/oauth/authorize\n  token_endpoint: https://api.moloco.cloud/oauth/token\n  revocation_endpoint: https://api.moloco.cloud/oauth/revoke\n  jwks_uri: https://api.moloco.cloud/oauth/jwks.json\n  grant_types_supported:\n\
  \  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\n  metadata_file: well-known/moloco-oauth-authorization-server.json\nprotected_resources:\n- resource: https://mcp.moloco.cloud/mcp\n  authorization_servers:\n  - https://api.moloco.cloud\n  scopes_supported:\n  - cloudapi.read\n  - offline_access\n  metadata_file: well-known/moloco-mcp-oauth-protected-resource.json\n  challenge: 'Bearer scope=\"cloudapi.read\", resource_metadata=\"https://mcp.moloco.cloud/.well-known/oauth-protected-resource/mcp\"'\nscopes:\n- scope: cloudapi.read\n  description: null\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.moloco.cloud/.well-known/oauth-authorization-server\n  - https://mcp.moloco.cloud/.well-known/oauth-protected-resource/mcp\n  required_by:\n  - https://mcp.moloco.cloud/mcp\n\
  - scope: offline_access\n  description: null\n  flows:\n  - authorizationCode\n  - refresh_token\n  sources:\n  - https://api.moloco.cloud/.well-known/oauth-authorization-server\n  - https://mcp.moloco.cloud/.well-known/oauth-protected-resource/mcp\nx-evidence:\n  fetched: '2026-07-31'\n  authorization_server_metadata:\n    url: https://api.moloco.cloud/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  protected_resource_metadata:\n    url: https://mcp.moloco.cloud/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/scopes/moloco-scopes.yml
summary_line: 2 scopes
tags:
- Advertising
- AdTech
- Demand-Side Platform
- Retail Media
- Commerce Media
- Programmatic Advertising
- Campaign Management
- Ad Serving
- Machine-Learning
- Mobile Marketing
- Reporting
- user-events
token_urls: []
---
