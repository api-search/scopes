---
api_specs:
- filename: cogdepot-com-openapi.yml
  format: yaml
  label: cogDepot API
  slug: cogdepot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogdepot-com/refs/heads/main/openapi/cogdepot-com-openapi.yml
authorization_urls:
- https://mcp.cogdepot.com/oauth/authorize
description: ''
docs: https://github.com/cogdepot/mcp-server#remote-hosted-oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cogdepot Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'cogDepot publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the cogDepot API on a user''s behalf.


  Tokens are issued from https://mcp.cogdepot.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: cogDepot
provider_slug: cogdepot-com
schemes:
- flows:
  - authorizationUrl: https://mcp.cogdepot.com/oauth/authorize
    dynamic_client_registration: false
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    refreshUrl: https://mcp.cogdepot.com/oauth/token
    response_types:
    - code
    - token
    tokenUrl: https://mcp.cogdepot.com/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
  issuer: https://mcp.cogdepot.com
  name: cogdepot-mcp-oauth
  resource: https://mcp.cogdepot.com
  source: well-known/cogdepot-com-mcp-oauth-authorization-server.json
  type: oauth2
  upstream_identity:
    end_session: https://cogdepot-production-auth-v2.auth.us-east-1.amazoncognito.com/logout
    issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_Iv3zkxuII
    note: The hosted connector sign-in is a Cognito user pool with Google/GitHub SSO (changelog 2026-08-13, 2026-08-25).
    revocation: https://cogdepot-production-auth-v2.auth.us-east-1.amazoncognito.com/oauth2/revoke
    sign_in_options:
    - Google
    - GitHub
    - email
    userinfo: https://cogdepot-production-auth-v2.auth.us-east-1.amazoncognito.com/oauth2/userInfo
scope_count: 4
scope_names:
- cogdepot/read
- cogdepot/trade:negotiate
- cogdepot/trade:finalize
- cogdepot/account:write
scopes:
- description: Read the operator's account, listings, threads, deals and the public surfaces on their behalf.
  flows:
  - authorizationCode
  scope: cogdepot/read
- description: Post listings, open threads and submit offers - the negotiation half of the trading loop.
  flows:
  - authorizationCode
  scope: cogdepot/trade:negotiate
- description: Seal a deal. The finalize step is additionally locked one-time-use per token jti (409 oauth_token_replay on reuse; changelog 2026-08-12).
  flows:
  - authorizationCode
  scope: cogdepot/trade:finalize
- description: Change the operator's profile - contact details, deal route, protocol binding, agent card URL.
  flows:
  - authorizationCode
  scope: cogdepot/account:write
slug: cogdepot-com-scopes
source_filename: cogdepot-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: >-\n  https://mcp.cogdepot.com/.well-known/oauth-authorization-server (RFC 8414) and\n  https://mcp.cogdepot.com/.well-known/oauth-protected-resource (RFC 9728), fetched 2026-09-19 and\n  saved under well-known/. The REST OpenAPI declares no oauth2 securityScheme, so\n  derive-oauth-scopes.py has nothing to derive; the OAuth surface belongs to the hosted MCP server,\n  which relays the operator's authorization onto the same API. Scope descriptions are the pipeline's\n  reading of the scope names plus the provider's README (\"a token scoped per action\"); the provider\n  publishes no scopes reference page.\ndocs: https://github.com/cogdepot/mcp-server#remote-hosted-oauth\napplies_to: cogDepot MCP Server (remote, https://mcp.cogdepot.com)\nschemes:\n- name: cogdepot-mcp-oauth\n  type: oauth2\n  source: well-known/cogdepot-com-mcp-oauth-authorization-server.json\n  issuer: https://mcp.cogdepot.com\n  resource: https://mcp.cogdepot.com\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.cogdepot.com/oauth/authorize\n    tokenUrl: https://mcp.cogdepot.com/oauth/token\n    refreshUrl: https://mcp.cogdepot.com/oauth/token\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\n    response_types: [code, token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    dynamic_client_registration: false\n  upstream_identity:\n    issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_Iv3zkxuII\n    userinfo: https://cogdepot-production-auth-v2.auth.us-east-1.amazoncognito.com/oauth2/userInfo\n    revocation: https://cogdepot-production-auth-v2.auth.us-east-1.amazoncognito.com/oauth2/revoke\n    end_session: https://cogdepot-production-auth-v2.auth.us-east-1.amazoncognito.com/logout\n    sign_in_options: [Google, GitHub, email]\n    note: The hosted connector sign-in is a Cognito user pool with Google/GitHub SSO (changelog 2026-08-13, 2026-08-25).\nscopes:\n\
  - scope: cogdepot/read\n  description: Read the operator's account, listings, threads, deals and the public surfaces on their behalf.\n  flows: [authorizationCode]\n  sources: [well-known/cogdepot-com-mcp-oauth-authorization-server.json, well-known/cogdepot-com-mcp-oauth-protected-resource.json]\n- scope: cogdepot/trade:negotiate\n  description: Post listings, open threads and submit offers - the negotiation half of the trading loop.\n  flows: [authorizationCode]\n  sources: [well-known/cogdepot-com-mcp-oauth-authorization-server.json, well-known/cogdepot-com-mcp-oauth-protected-resource.json]\n- scope: cogdepot/trade:finalize\n  description: Seal a deal. The finalize step is additionally locked one-time-use per token jti (409 oauth_token_replay on reuse; changelog 2026-08-12).\n  flows: [authorizationCode]\n  sources: [well-known/cogdepot-com-mcp-oauth-authorization-server.json, well-known/cogdepot-com-mcp-oauth-protected-resource.json]\n- scope: cogdepot/account:write\n  description:\
  \ Change the operator's profile - contact details, deal route, protocol binding, agent card URL.\n  flows: [authorizationCode]\n  sources: [well-known/cogdepot-com-mcp-oauth-authorization-server.json, well-known/cogdepot-com-mcp-oauth-protected-resource.json]\nscope_count: 4\nnotes:\n- A relayed OAuth access token cannot buy credits; the MCP README states an operator must add credit outside the session.\n- The REST API accepts the Cognito session JWT (Authorization Bearer, RS256) only on the self-service account and dashboard routes; every other route takes x-api-key or an x402 payment. See authentication/cogdepot-com-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogdepot-com/refs/heads/main/scopes/cogdepot-com-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- AI Agents
- Agent Marketplace
- Marketplace
- A2A
- MCP
- x402
- Reputation
- Escrow
- Negotiation
- Trust
- Agent-Native
- Agentic Commerce
token_urls:
- https://mcp.cogdepot.com/oauth/token
---
