---
api_specs:
- filename: sendspark-dvm-bundles-api-openapi.yml
  format: yaml
  label: Sendspark DVM Bundles API
  slug: sendspark-dvm-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-dvm-bundles-api-openapi.yml
- filename: sendspark-dynamics-campaign-api-openapi.yml
  format: yaml
  label: Sendspark Dynamics Campaign API
  slug: sendspark-dynamics-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-dynamics-campaign-api-openapi.yml
- filename: sendspark-webhook-api-openapi.yml
  format: yaml
  label: Sendspark Webhook API
  slug: sendspark-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-webhook-api-openapi.yml
- filename: sendspark-workspace-api-openapi.yml
  format: yaml
  label: Sendspark Workspace API
  slug: sendspark-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-workspace-api-openapi.yml
authorization_urls:
- https://auth.sendspark.com/oauth2/authorize
description: ''
docs: https://help.sendspark.com/mcp/overview
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Sendspark Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sendspark publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sendspark API on a user''s behalf.


  Tokens are issued from https://auth.sendspark.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sendspark
provider_slug: sendspark
schemes:
- client_id_metadata_document_supported: true
  dynamic_client_registration: true
  endpoints:
    introspection_endpoint: https://auth.sendspark.com/oauth2/introspection
    jwks_uri: https://auth.sendspark.com/oauth2/jwks
    registration_endpoint: https://auth.sendspark.com/oauth2/register
  flows:
  - authorizationUrl: https://auth.sendspark.com/oauth2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://auth.sendspark.com/oauth2/token
  - deviceAuthorizationUrl: https://auth.sendspark.com/oauth2/device_authorization
    flow: deviceCode
    grant: urn:ietf:params:oauth:grant-type:device_code
    tokenUrl: https://auth.sendspark.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://auth.sendspark.com/oauth2/token
  name: mcpOAuth
  resource_indicators_supported: true
  source: https://auth.sendspark.com/.well-known/openid-configuration
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OIDC scope requesting an ID token for the signed-in Sendspark user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Standard OIDC scope releasing the signed-in user's basic profile claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Standard OIDC scope releasing the signed-in user's email address.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Requests a refresh token so the MCP connector can stay authorized without a repeat browser sign-in.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: sendspark-scopes
source_filename: sendspark-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource:\n- https://auth.sendspark.com/.well-known/openid-configuration\n- https://apiv2.sendspark.com/.well-known/oauth-authorization-server\n- https://apiv2.sendspark.com/.well-known/oauth-protected-resource/api/mcp\ndocs: https://help.sendspark.com/mcp/overview\napplies_to: >-\n  The OAuth 2.0 / OIDC surface that authenticates the hosted MCP server at\n  https://apiv2.sendspark.com/api/mcp. The REST API (api-gw.sendspark.com) does\n  NOT use OAuth — it authenticates with an x-api-key + x-api-secret header pair\n  and therefore has no scope surface. `derive-oauth-scopes.py` correctly found\n  zero oauth2 schemes in the OpenAPI; every scope below comes from the live\n  authorization-server metadata documents, not from the spec.\nissuer: https://auth.sendspark.com\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  source: https://auth.sendspark.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://auth.sendspark.com/oauth2/authorize\n    tokenUrl: https://auth.sendspark.com/oauth2/token\n    pkce: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.sendspark.com/oauth2/device_authorization\n    grant: 'urn:ietf:params:oauth:grant-type:device_code'\n    tokenUrl: https://auth.sendspark.com/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://auth.sendspark.com/oauth2/token\n  endpoints:\n    jwks_uri: https://auth.sendspark.com/oauth2/jwks\n    introspection_endpoint: https://auth.sendspark.com/oauth2/introspection\n    registration_endpoint: https://auth.sendspark.com/oauth2/register\n  token_endpoint_auth_methods_supported: [none, client_secret_post, client_secret_basic]\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  resource_indicators_supported: true\nscopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token for the signed-in Sendspark user.\n  flows: [authorizationCode, deviceCode]\n\
  \  sources: [https://auth.sendspark.com/.well-known/openid-configuration]\n- scope: profile\n  description: Standard OIDC scope releasing the signed-in user's basic profile claims.\n  flows: [authorizationCode, deviceCode]\n  sources: [https://auth.sendspark.com/.well-known/openid-configuration]\n- scope: email\n  description: Standard OIDC scope releasing the signed-in user's email address.\n  flows: [authorizationCode, deviceCode]\n  sources: [https://auth.sendspark.com/.well-known/openid-configuration]\n- scope: offline_access\n  description: Requests a refresh token so the MCP connector can stay authorized without a repeat browser sign-in.\n  flows: [authorizationCode, deviceCode]\n  sources: [https://auth.sendspark.com/.well-known/openid-configuration]\nprotected_resource:\n  resource: https://apiv2.sendspark.com/api/mcp\n  authorization_servers: [https://auth.sendspark.com]\n  bearer_methods_supported: [header]\n  scopes_required: null\nfindings:\n- >-\n  Sendspark publishes only\
  \ the four standard OIDC scopes. There are NO\n  Sendspark-specific authorization scopes — no per-resource or per-action scope\n  such as campaigns:read or prospects:read. Authorization is coarse: a token\n  grants the signed-in user's identity, and the MCP server then enforces\n  read-only access to whatever workspaces that user belongs to. The\n  protected-resource metadata declares no required scopes.\n- >-\n  The authorization server supports dynamic client registration\n  (/oauth2/register) and RFC 8707 resource indicators, which is what lets an\n  arbitrary MCP client connect with no pre-provisioned client id.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/scopes/sendspark-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Company
- Video
- Sales
- Marketing
- Personalization
- Artificial Intelligence
- Video Messaging
- Webhook
- MCP
token_urls:
- https://auth.sendspark.com/oauth2/token
---
