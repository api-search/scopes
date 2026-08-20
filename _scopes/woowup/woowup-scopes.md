---
authorization_urls:
- https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/authorize
description: The OAuth 2.1 surface WoowUp exposes belongs to its hosted MCP server at mcp.woowup.com, not to the REST API v3. The REST API v3 authenticates with a static account API key and has no scope model at all (see authentication/woowup-authentication.yml). The authorization server is an external Zitadel tenant; the resource server advertises one WoowUp-specific scope, campaigns:read, alongside the standard OIDC scopes.
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Woowup Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WoowUp publishes 4 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the WoowUp API on a user''s behalf.


  Tokens are issued from https://mcp.woowup.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WoowUp
provider_slug: woowup
schemes:
- flows:
  - authorizationUrl: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://mcp.woowup.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://mcp.woowup.com/oauth/token
  - deviceAuthorizationUrl: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/device_authorization
    flow: deviceCode
  - authorizationUrl: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/authorize
    flow: implicit
    notes: advertised in response_types_supported (id_token, "id_token token")
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/introspect
  issuer: https://my-dev-instance-ap11e0.us1.zitadel.cloud
  jwks_uri: https://mcp.woowup.com/oauth/jwks
  name: MCPOAuth2
  registration_endpoint: https://mcp.woowup.com/oauth/register
  revocation_endpoint: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/revoke
  source: https://mcp.woowup.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  type: oauth2
scope_count: 4
scope_names:
- campaigns:read
- openid
- profile
- email
scopes:
- description: Read access to campaigns through the MCP server. The only WoowUp-specific scope published; the tool set it unlocks is not enumerable anonymously (tools/list returns 401).
  flows: []
  scope: campaigns:read
- description: Standard OIDC scope — request an ID token for the authenticating user.
  flows: []
  scope: openid
- description: Standard OIDC scope — basic profile claims (name, preferred_username, locale).
  flows: []
  scope: profile
- description: Standard OIDC scope — email and email_verified claims.
  flows: []
  scope: email
slug: woowup-scopes
source_filename: woowup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.woowup.com/.well-known/oauth-protected-resource (RFC 9728) and\n  https://mcp.woowup.com/.well-known/oauth-authorization-server (RFC 8414),\n  both HTTP 200 and saved verbatim under well-known/. WoowUp publishes no\n  OpenAPI and no scopes/permissions reference page, so this is the complete\n  published scope surface — nothing is inferred.\ndescription: >-\n  The OAuth 2.1 surface WoowUp exposes belongs to its hosted MCP server at\n  mcp.woowup.com, not to the REST API v3. The REST API v3 authenticates with a\n  static account API key and has no scope model at all (see\n  authentication/woowup-authentication.yml). The authorization server is an\n  external Zitadel tenant; the resource server advertises one WoowUp-specific\n  scope, campaigns:read, alongside the standard OIDC scopes.\nresource:\n  identifier: https://mcp.woowup.com/\n  authorization_servers:\n    - https://mcp.woowup.com/\n  bearer_methods_supported:\
  \ [header]\nschemes:\n  - name: MCPOAuth2\n    type: oauth2\n    source: https://mcp.woowup.com/.well-known/oauth-authorization-server\n    issuer: https://my-dev-instance-ap11e0.us1.zitadel.cloud\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/authorize\n        tokenUrl: https://mcp.woowup.com/oauth/token\n        pkce: [S256]\n      - flow: clientCredentials\n        tokenUrl: https://mcp.woowup.com/oauth/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/device_authorization\n      - flow: implicit\n        authorizationUrl: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/authorize\n        notes: advertised in response_types_supported (id_token, \"id_token token\")\n    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - client_credentials\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n\
  \      - 'urn:ietf:params:oauth:grant-type:device_code'\n    token_endpoint_auth_methods_supported: [none, client_secret_basic, client_secret_post, private_key_jwt]\n    registration_endpoint: https://mcp.woowup.com/oauth/register\n    jwks_uri: https://mcp.woowup.com/oauth/jwks\n    introspection_endpoint: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/introspect\n    revocation_endpoint: https://my-dev-instance-ap11e0.us1.zitadel.cloud/oauth/v2/revoke\nscopes:\n  - scope: 'campaigns:read'\n    description: >-\n      Read access to campaigns through the MCP server. The only\n      WoowUp-specific scope published; the tool set it unlocks is not\n      enumerable anonymously (tools/list returns 401).\n    surface: mcp\n    sources: ['https://mcp.woowup.com/.well-known/oauth-protected-resource']\n  - scope: openid\n    description: Standard OIDC scope — request an ID token for the authenticating user.\n    surface: mcp\n    sources: ['https://mcp.woowup.com/.well-known/oauth-protected-resource']\n\
  \  - scope: profile\n    description: Standard OIDC scope — basic profile claims (name, preferred_username, locale).\n    surface: mcp\n    sources: ['https://mcp.woowup.com/.well-known/oauth-protected-resource']\n  - scope: email\n    description: Standard OIDC scope — email and email_verified claims.\n    surface: mcp\n    sources: ['https://mcp.woowup.com/.well-known/oauth-protected-resource']\nauthorization_server_scopes_supported:\n  - openid\n  - profile\n  - email\n  - phone\n  - address\n  - offline_access\nnotes: >-\n  scopes_supported differs between the two metadata documents: the\n  authorization server (Zitadel) advertises the standard OIDC set plus\n  offline_access, while the protected resource advertises openid/profile/email\n  plus campaigns:read. The resource document is authoritative for what the MCP\n  server itself accepts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woowup/refs/heads/main/scopes/woowup-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials/deviceCode/implicit
tags:
- Company
- CRM
- Loyalty
- Customer Data
- Marketing Automation
- Retail
- E-Commerce
- Push Notifications
token_urls:
- https://mcp.woowup.com/oauth/token
---
