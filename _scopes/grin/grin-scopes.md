---
authorization_urls:
- https://auth.grin.co/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Grin Scopes
name_suffix: OAuth Scopes
note: 'Scopes are read from the two anonymous discovery documents GRIN''s own hosts serve, not from an OpenAPI (none is publicly reachable) and not from a docs scopes reference (GRIN publishes none). Two distinct scope sets exist and are kept separate here: the identity scopes the auth.grin.co tenant advertises, and the much smaller set the Gia MCP server actually requires as a protected resource. GRIN publishes NO product/permission scopes — nothing of the form read:creators or write:programs is advertised anywhere public — so the MCP server''s authorization is account-wide identity rather than scoped capability. That is a real finding about the agent surface, not a gap in this probe.'
overview: 'Grin publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Grin API on a user''s behalf.


  Tokens are issued from https://auth.grin.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Grin
provider_slug: grin
schemes:
- flows:
  - authorizationUrl: https://auth.grin.co/authorize
    flow: authorizationCode
    tokenUrl: https://auth.grin.co/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.grin.co/oauth/token
  - deviceAuthorizationUrl: https://auth.grin.co/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.grin.co/oauth/token
  issuer: https://auth.grin.co/
  name: GrinOIDC
  source: well-known/grin-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
- phone
- address
scopes:
- description: OIDC authentication; issues an ID token identifying the GRIN user.
  flows:
  - authorizationCode
  - clientCredentials
  - deviceCode
  scope: openid
- description: Basic profile claims for the authenticated GRIN user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Email address of the authenticated GRIN user.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Whether the user's email address has been verified.
  flows:
  - authorizationCode
  scope: email_verified
- description: Issues a refresh token for long-lived access.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: Full name claim.
  flows:
  - authorizationCode
  scope: name
- description: Given-name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: Family-name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: Nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: Profile picture claim.
  flows:
  - authorizationCode
  scope: picture
- description: Account creation timestamp claim.
  flows:
  - authorizationCode
  scope: created_at
- description: Linked identity-provider records for the user.
  flows:
  - authorizationCode
  scope: identities
- description: Phone-number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Address claim.
  flows:
  - authorizationCode
  scope: address
slug: grin-scopes
source_filename: grin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.grin.co/.well-known/openid-configuration\nnote: >-\n  Scopes are read from the two anonymous discovery documents GRIN's own hosts\n  serve, not from an OpenAPI (none is publicly reachable) and not from a docs\n  scopes reference (GRIN publishes none). Two distinct scope sets exist and are\n  kept separate here: the identity scopes the auth.grin.co tenant advertises,\n  and the much smaller set the Gia MCP server actually requires as a protected\n  resource. GRIN publishes NO product/permission scopes — nothing of the form\n  read:creators or write:programs is advertised anywhere public — so the MCP\n  server's authorization is account-wide identity rather than scoped capability.\n  That is a real finding about the agent surface, not a gap in this probe.\n\nschemes:\n- name: GrinOIDC\n  source: well-known/grin-openid-configuration.json\n  issuer: https://auth.grin.co/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://auth.grin.co/authorize\n    tokenUrl: https://auth.grin.co/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.grin.co/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.grin.co/oauth/device/code\n    tokenUrl: https://auth.grin.co/oauth/token\n\nscopes:\n- scope: openid\n  description: OIDC authentication; issues an ID token identifying the GRIN user.\n  flows: [authorizationCode, clientCredentials, deviceCode]\n  required_by: [https://mcp.grin.co/mcp]\n  sources: [well-known/grin-openid-configuration.json, well-known/grin-oauth-protected-resource.json]\n- scope: profile\n  description: Basic profile claims for the authenticated GRIN user.\n  flows: [authorizationCode, deviceCode]\n  required_by: [https://mcp.grin.co/mcp]\n  sources: [well-known/grin-openid-configuration.json, well-known/grin-oauth-protected-resource.json]\n- scope: email\n  description: Email address of the authenticated GRIN user.\n  flows: [authorizationCode, deviceCode]\n\
  \  required_by: [https://mcp.grin.co/mcp]\n  sources: [well-known/grin-openid-configuration.json, well-known/grin-oauth-protected-resource.json]\n- scope: email_verified\n  description: Whether the user's email address has been verified.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: offline_access\n  description: Issues a refresh token for long-lived access.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: name\n  description: Full name claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: given_name\n  description: Given-name claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: family_name\n  description: Family-name claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: nickname\n  description: Nickname claim.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/grin-openid-configuration.json]\n- scope: picture\n  description: Profile picture claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: created_at\n  description: Account creation timestamp claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: identities\n  description: Linked identity-provider records for the user.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: phone\n  description: Phone-number claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n- scope: address\n  description: Address claim.\n  flows: [authorizationCode]\n  sources: [well-known/grin-openid-configuration.json]\n\nmcp_resource:\n  resource: https://mcp.grin.co/mcp\n  authorization_servers: [https://auth.grin.co/]\n  scopes_supported: [openid, email, profile]\n  source: well-known/grin-oauth-protected-resource.json\n\
  \ngaps:\n- id: no-product-scopes\n  detail: >-\n    No capability-level scopes are published. An agent authorizing against the\n    Gia MCP server presents only identity scopes, so a consumer cannot request\n    or reason about least privilege from the public surface.\n\nx-evidence:\n- url: https://auth.grin.co/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://mcp.grin.co/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grin/refs/heads/main/scopes/grin-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Influencer Marketing
- Creator Economy
- Creator Management
- Affiliate Marketing
- Marketing
- Social Media
- eCommerce
token_urls:
- https://auth.grin.co/oauth/token
---
