---
api_specs:
- filename: profound-agents-api-openapi.yml
  format: yaml
  label: Profound Agents API
  slug: profound-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-agents-api-openapi.yml
- filename: profound-beta-api-openapi.yml
  format: yaml
  label: Profound Beta API
  slug: profound-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-beta-api-openapi.yml
- filename: profound-bot-traffic-reports-api-openapi.yml
  format: yaml
  label: Profound Bot Traffic Reports API
  slug: profound-bot-traffic-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-bot-traffic-reports-api-openapi.yml
- filename: profound-categories-api-openapi.yml
  format: yaml
  label: Profound Categories API
  slug: profound-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-categories-api-openapi.yml
- filename: profound-content-api-openapi.yml
  format: yaml
  label: Profound Content API
  slug: profound-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-content-api-openapi.yml
- filename: profound-content-optimization-api-openapi.yml
  format: yaml
  label: Profound Content optimization API
  slug: profound-content-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-content-optimization-api-openapi.yml
- filename: profound-documents-api-openapi.yml
  format: yaml
  label: Profound Documents API
  slug: profound-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-documents-api-openapi.yml
- filename: profound-human-referrals-api-openapi.yml
  format: yaml
  label: Profound Human Referrals API
  slug: profound-human-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-human-referrals-api-openapi.yml
- filename: profound-integrations-api-openapi.yml
  format: yaml
  label: Profound Integrations API
  slug: profound-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-integrations-api-openapi.yml
- filename: profound-knowledge-bases-api-openapi.yml
  format: yaml
  label: Profound Knowledge bases API
  slug: profound-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-knowledge-bases-api-openapi.yml
- filename: profound-openai-ads-api-openapi.yml
  format: yaml
  label: Profound OpenAI Ads API
  slug: profound-openai-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-openai-ads-api-openapi.yml
- filename: profound-organization-api-openapi.yml
  format: yaml
  label: Profound Organization API
  slug: profound-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-organization-api-openapi.yml
- filename: profound-projects-api-openapi.yml
  format: yaml
  label: Profound Projects API
  slug: profound-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-projects-api-openapi.yml
- filename: profound-prompts-api-openapi.yml
  format: yaml
  label: Profound Prompts API
  slug: profound-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-prompts-api-openapi.yml
- filename: profound-reports-api-openapi.yml
  format: yaml
  label: Profound Reports API
  slug: profound-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-reports-api-openapi.yml
authorization_urls:
- https://auth.tryprofound.com/oauth2/authorize
description: ''
docs: https://docs.tryprofound.com/mcp/authentication
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Profound Scopes
name_suffix: OAuth Scopes
note: The REST API declares NO oauth2 security scheme — it is API-key only (X-API-Key or Bearer), so derive-oauth-scopes.py correctly found zero scopes in the OpenAPI. The OAuth surface belongs to the hosted MCP server, whose authorization server metadata is anonymously readable. The scopes below are the identity scopes that server advertises; Profound publishes no resource-permission scope vocabulary — MCP authorization is coarse-grained, with every tool call executing as the signed-in user and returning only the data that user can already access.
overview: 'Profound publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Profound API on a user''s behalf.


  Tokens are issued from https://auth.tryprofound.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Profound
provider_slug: profound
schemes:
- client_id_metadata_document_supported: true
  dynamic_client_registration: true
  endpoints:
    introspection: https://auth.tryprofound.com/oauth2/introspection
    jwks: https://auth.tryprofound.com/oauth2/jwks
    registration: https://auth.tryprofound.com/oauth2/register
  flows:
  - authorizationUrl: https://auth.tryprofound.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://auth.tryprofound.com/oauth2/token
  - deviceAuthorizationUrl: https://auth.tryprofound.com/oauth2/device_authorization
    flow: deviceCode
    grantType: urn:ietf:params:oauth:grant-type:device_code
  - flow: refreshToken
    tokenUrl: https://auth.tryprofound.com/oauth2/token
  name: MCP OAuth 2.1
  response_modes_supported:
  - query
  response_types_supported:
  - code
  source: https://mcp.tryprofound.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC identity — issue an ID token for the signed-in Profound user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the signed-in Profound user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim for the signed-in Profound user.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the MCP client can maintain a long-lived session.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: profound-scopes
source_filename: profound-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.tryprofound.com/.well-known/oauth-authorization-server\ndocs: https://docs.tryprofound.com/mcp/authentication\nnote: >-\n  The REST API declares NO oauth2 security scheme — it is API-key only\n  (X-API-Key or Bearer), so derive-oauth-scopes.py correctly found zero scopes\n  in the OpenAPI. The OAuth surface belongs to the hosted MCP server, whose\n  authorization server metadata is anonymously readable. The scopes below are\n  the identity scopes that server advertises; Profound publishes no\n  resource-permission scope vocabulary — MCP authorization is coarse-grained,\n  with every tool call executing as the signed-in user and returning only the\n  data that user can already access.\napplies_to: mcp\nissuer: https://auth.tryprofound.com\nschemes:\n- name: MCP OAuth 2.1\n  source: https://mcp.tryprofound.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tryprofound.com/oauth2/authorize\n\
  \    tokenUrl: https://auth.tryprofound.com/oauth2/token\n    pkce: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.tryprofound.com/oauth2/device_authorization\n    grantType: urn:ietf:params:oauth:grant-type:device_code\n  - flow: refreshToken\n    tokenUrl: https://auth.tryprofound.com/oauth2/token\n  endpoints:\n    registration: https://auth.tryprofound.com/oauth2/register\n    introspection: https://auth.tryprofound.com/oauth2/introspection\n    jwks: https://auth.tryprofound.com/oauth2/jwks\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  response_types_supported: [code]\n  response_modes_supported: [query]\nscopes:\n- scope: openid\n  description: OIDC identity — issue an ID token for the signed-in Profound user.\n  flows: [authorizationCode]\n  sources: [https://mcp.tryprofound.com/.well-known/oauth-authorization-server]\n- scope: profile\n  description: Basic profile claims for the signed-in Profound user.\n  flows:\
  \ [authorizationCode]\n  sources: [https://mcp.tryprofound.com/.well-known/oauth-authorization-server]\n- scope: email\n  description: Email address claim for the signed-in Profound user.\n  flows: [authorizationCode]\n  sources: [https://mcp.tryprofound.com/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Issue a refresh token so the MCP client can maintain a long-lived session.\n  flows: [authorizationCode, refreshToken]\n  sources: [https://mcp.tryprofound.com/.well-known/oauth-authorization-server]\nprotected_resource:\n  resource: https://mcp.tryprofound.com/mcp\n  resource_name: profound_mcp\n  authorization_servers: [https://auth.tryprofound.com]\n  bearer_methods_supported: [header]\ngaps:\n- No resource/permission scopes (e.g. reports:read, agents:write) are published.\n- The REST API has no OAuth surface at all; API keys carry all of an organization's read access with no scoping.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://mcp.tryprofound.com/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n  - url: https://mcp.tryprofound.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/scopes/profound-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Company
- Artificial Intelligence
- Answer Engine Optimization
- AEO
- AI Search
- Generative Engine Optimization
- Marketing
- Analytics
- Agent Analytics
- Brand Visibility
- Citations
- MCP
token_urls:
- https://auth.tryprofound.com/oauth2/token
---
