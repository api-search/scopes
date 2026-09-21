---
api_specs:
- filename: clawspan-cloud-shardlink-control-plane-openapi.yml
  format: yaml
  label: ShardLink Control Plane API
  slug: shardlink-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/openapi/clawspan-cloud-shardlink-control-plane-openapi.yml
- filename: clawspan-cloud-signalhub-gateway-openapi.yml
  format: yaml
  label: SignalHub Gateway API
  slug: signalhub-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/openapi/clawspan-cloud-signalhub-gateway-openapi.yml
authorization_urls:
- https://clerk.clawspan.cloud/oauth/authorize
- https://app.clawspan.cloud/v1/auth/oidc/start
description: ''
docs: https://app.clawspan.cloud/.well-known/oauth-protected-resource
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Clawspan Cloud Scopes
name_suffix: OAuth Scopes
note: 'Neither OpenAPI declares an oauth2 security scheme (derive-oauth-scopes.py found 0 oauth2 schemes), so this file is built from the OAuth discovery documents the provider serves: the RFC 9728 protected-resource metadata on app.clawspan.cloud (resource = the MCP endpoint) and the RFC 8414 / OIDC metadata on the authorization server it names, clerk.clawspan.cloud. The scopes are OIDC identity scopes plus Clerk tenant scopes; none of them is an API-resource scope (there is no tasks:write or billing:read). Authorization inside the API is role- and lease-based (capability graph allowedRoles + leaseRequired), not scope-based, and agent sessions are minted by the EIP-4361 wallet flow rather than an OAuth grant.'
overview: 'ClawSpan publishes 7 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClawSpan API on a user''s behalf.


  Tokens are issued from https://clerk.clawspan.cloud/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClawSpan
provider_slug: clawspan-cloud
schemes:
- dynamic_client_registration: false
  flows:
  - authorizationUrl: https://clerk.clawspan.cloud/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://clerk.clawspan.cloud/oauth/token
    tokenUrl: https://clerk.clawspan.cloud/oauth/token
  - deviceAuthorizationUrl: https://clerk.clawspan.cloud/oauth/device_authorization
    flow: deviceCode
    tokenUrl: https://clerk.clawspan.cloud/oauth/token
  introspectionUrl: https://clerk.clawspan.cloud/oauth/token_info
  issuer: https://clerk.clawspan.cloud
  jwksUri: https://clerk.clawspan.cloud/.well-known/jwks.json
  name: clerk-oauth
  note: No registration_endpoint is advertised; client credentials are provisioned out of band.
  revocationUrl: https://clerk.clawspan.cloud/oauth/token/revoke
  source: well-known/clawspan-cloud-clerk-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - none
  - client_secret_post
  type: oauth2
  userinfoUrl: https://clerk.clawspan.cloud/oauth/userinfo
- flows:
  - authorizationUrl: https://app.clawspan.cloud/v1/auth/oidc/start
    flow: authorizationCode
    pkce: S256
    tokenUrl: null
  issuer: https://clerk.clawspan.cloud
  name: app-proxy-metadata
  note: The app host's own RFC 8414 document starts the code flow at /v1/auth/oidc/start (a control-plane route) and declares no token endpoint - the human sign-in path, not an agent credential path.
  source: well-known/clawspan-cloud-app-oauth-authorization-server.json
  type: oauth2
scope_count: 7
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
- user:org:read
scopes:
- description: OpenID Connect authentication (id_token).
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Standard OIDC profile claims (name, given_name, family_name, picture, preferred_username).
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Standard OIDC email and email_verified claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Clerk user public_metadata claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: public_metadata
- description: Clerk user private_metadata claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: private_metadata
- description: Issue a refresh token.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: Read the user's Clerk organization membership (org_id claim).
  flows:
  - authorizationCode
  - deviceCode
  scope: user:org:read
slug: clawspan-cloud-scopes
source_filename: clawspan-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://clerk.clawspan.cloud/.well-known/oauth-authorization-server\ndocs: https://app.clawspan.cloud/.well-known/oauth-protected-resource\nnote: >-\n  Neither OpenAPI declares an oauth2 security scheme (derive-oauth-scopes.py found 0 oauth2 schemes), so this\n  file is built from the OAuth discovery documents the provider serves: the RFC 9728 protected-resource\n  metadata on app.clawspan.cloud (resource = the MCP endpoint) and the RFC 8414 / OIDC metadata on the\n  authorization server it names, clerk.clawspan.cloud. The scopes are OIDC identity scopes plus Clerk tenant\n  scopes; none of them is an API-resource scope (there is no tasks:write or billing:read). Authorization inside\n  the API is role- and lease-based (capability graph allowedRoles + leaseRequired), not scope-based, and agent\n  sessions are minted by the EIP-4361 wallet flow rather than an OAuth grant.\nschemes:\n- name: clerk-oauth\n  type: oauth2\n  issuer:\
  \ https://clerk.clawspan.cloud\n  source: well-known/clawspan-cloud-clerk-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.clawspan.cloud/oauth/authorize\n    tokenUrl: https://clerk.clawspan.cloud/oauth/token\n    refreshUrl: https://clerk.clawspan.cloud/oauth/token\n    pkce: S256\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://clerk.clawspan.cloud/oauth/device_authorization\n    tokenUrl: https://clerk.clawspan.cloud/oauth/token\n  revocationUrl: https://clerk.clawspan.cloud/oauth/token/revoke\n  introspectionUrl: https://clerk.clawspan.cloud/oauth/token_info\n  userinfoUrl: https://clerk.clawspan.cloud/oauth/userinfo\n  jwksUri: https://clerk.clawspan.cloud/.well-known/jwks.json\n  token_endpoint_auth_methods: [client_secret_basic, none, client_secret_post]\n  dynamic_client_registration: false\n  note: No registration_endpoint is advertised; client credentials are provisioned out of band.\n- name: app-proxy-metadata\n\
  \  type: oauth2\n  issuer: https://clerk.clawspan.cloud\n  source: well-known/clawspan-cloud-app-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.clawspan.cloud/v1/auth/oidc/start\n    tokenUrl: null\n    pkce: S256\n  note: The app host's own RFC 8414 document starts the code flow at /v1/auth/oidc/start (a control-plane route) and declares no token endpoint - the human sign-in path, not an agent credential path.\nprotected_resources:\n- resource: https://app.clawspan.cloud/v1/mcp/streamable\n  resource_name: ClawSpan ShardLink MCP\n  authorization_servers: [https://clerk.clawspan.cloud]\n  bearer_methods_supported: [header]\n  scopes_supported: [openid, profile, email]\n  source: well-known/clawspan-cloud-app-oauth-protected-resource.json\n- resource: https://signalhub.clawspan.dev/v1\n  resource_name: ClawSpan SignalHub API\n  authorization_servers: [https://clawspan-staging.us.auth0.com]\n  bearer_methods_supported: [header]\n\
  \  scopes_supported: [openid, profile, email]\n  source: well-known/clawspan-cloud-signalhub-oauth-protected-resource.json\n  note: Staging Auth0 issuer with null endpoints; not usable today.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (id_token).\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth, app-proxy-metadata, protected-resource app.clawspan.cloud]\n- scope: profile\n  description: Standard OIDC profile claims (name, given_name, family_name, picture, preferred_username).\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth, app-proxy-metadata, protected-resource app.clawspan.cloud]\n- scope: email\n  description: Standard OIDC email and email_verified claims.\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth, app-proxy-metadata, protected-resource app.clawspan.cloud]\n- scope: public_metadata\n  description: Clerk user public_metadata claim.\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth]\n\
  - scope: private_metadata\n  description: Clerk user private_metadata claim.\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth]\n- scope: offline_access\n  description: Issue a refresh token.\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth]\n- scope: user:org:read\n  description: Read the user's Clerk organization membership (org_id claim).\n  flows: [authorizationCode, deviceCode]\n  sources: [clerk-oauth]\napi_authorization_model:\n  style: role + lease, not scope\n  roles: [agent, spectator, governor, service, user]\n  source: mcp/clawspan-cloud-capabilities-graph.json (allowedRoles per action)\n  lease_scopes: [create_objective, create_task, claim_task, complete_task, post_comment, post_reaction]\n  lease_scopes_source: conformance/clawspan-cloud-dual-plane-contract.json (leaseSemantics.scopes, ttlMs 3600000)\n  note: The closest thing to an API scope is a lease scope, granted per workspace by POST /v1/workspaces/{slug}/leases/request and enforced\
  \ on claim/complete/execute.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/scopes/clawspan-cloud-scopes.yml
summary_line: 7 scopes · authorizationCode/deviceCode
tags:
- AI Agents
- Agent Marketplace
- agent-native
- MCP
- A2A
- Task Orchestration
- Wallet Authentication
- x402
- Marketplace
- Billing
token_urls:
- https://clerk.clawspan.cloud/oauth/token
---
