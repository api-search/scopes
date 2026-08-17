---
authorization_urls:
- https://www.mobileaction.co/awfah-oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Mobile Action Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mobile Action publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mobile Action API on a user''s behalf.


  Tokens are issued from https://www.mobileaction.co/wp-json/awfah_oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mobile Action
provider_slug: mobile-action
schemes:
- flows:
  - authorizationUrl: https://www.mobileaction.co/awfah-oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://www.mobileaction.co/wp-json/awfah_oauth/v1/token
  grant_types:
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  issuer: https://www.mobileaction.co
  jwks_uri: https://www.mobileaction.co/wp-json/awfah_oauth/v1/jwks
  name: wordpress-site-oauth
  registration_endpoint: https://www.mobileaction.co/wp-json/awfah_oauth/v1/register
  revocation_endpoint: https://www.mobileaction.co/wp-json/awfah_oauth/v1/revoke
  source: well-known/mobile-action-openid-configuration.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- mcp:woocommerce
scopes:
- description: Read access for the WordPress site MCP plugin.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access for the WordPress site MCP plugin.
  flows:
  - authorizationCode
  scope: mcp:write
- description: WooCommerce access for the WordPress site MCP plugin.
  flows:
  - authorizationCode
  scope: mcp:woocommerce
slug: mobile-action-scopes
source_filename: mobile-action-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://www.mobileaction.co/.well-known/openid-configuration\napplies_to: https://www.mobileaction.co (WordPress marketing site)\ndoes_not_apply_to:\n- https://api.mobileaction.co\n- https://mcp.mobileaction.co\nscope_note: IMPORTANT SCOPE BOUNDARY. The MobileAction intelligence API has NO OAuth surface at all -\n  it authenticates with a single ?token= API key (see authentication/mobile-action-authentication.yml),\n  and the remote MCP server carries the same key in its URL. The OAuth 2.0 / OIDC authorization server\n  described here is served by an OAuth plugin on the WordPress marketing site at www.mobileaction.co and\n  governs that site only. It is recorded because MobileAction genuinely serves the discovery document\n  from its own domain, not because it fronts the data API.\nschemes:\n- name: wordpress-site-oauth\n  type: oauth2\n  issuer: https://www.mobileaction.co\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://www.mobileaction.co/awfah-oauth/authorize\n    tokenUrl: https://www.mobileaction.co/wp-json/awfah_oauth/v1/token\n    pkce:\n    - S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  registration_endpoint: https://www.mobileaction.co/wp-json/awfah_oauth/v1/register\n  revocation_endpoint: https://www.mobileaction.co/wp-json/awfah_oauth/v1/revoke\n  jwks_uri: https://www.mobileaction.co/wp-json/awfah_oauth/v1/jwks\n  id_token_signing_alg:\n  - RS256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  source: well-known/mobile-action-openid-configuration.json\nscopes:\n- scope: mcp:read\n  description: Read access for the WordPress site MCP plugin.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/mobile-action-openid-configuration.json\n- scope: mcp:write\n  description: Write access for the WordPress site MCP plugin.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/mobile-action-openid-configuration.json\n\
  - scope: mcp:woocommerce\n  description: WooCommerce access for the WordPress site MCP plugin.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/mobile-action-openid-configuration.json\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://www.mobileaction.co/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobile-action/refs/heads/main/scopes/mobile-action-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- App Store Optimization
- ASO
- Mobile Marketing
- Apple Search Ads
- App Intelligence
- Ad Intelligence
- Market Intelligence
- Analytics
- MCP
- Agent Tools
- App Store Intelligence
- Mobile Measurement
token_urls:
- https://www.mobileaction.co/wp-json/awfah_oauth/v1/token
---
