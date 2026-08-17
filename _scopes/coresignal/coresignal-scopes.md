---
api_specs:
- filename: coresignal-collect-api-openapi.yml
  format: yaml
  label: Coresignal Collect API
  slug: coresignal-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-collect-api-openapi.yml
- filename: coresignal-search-api-openapi.yml
  format: yaml
  label: Coresignal Search API
  slug: coresignal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-search-api-openapi.yml
authorization_urls:
- https://dashboard.coresignal.com/api/auth/oauth2/authorize
description: ''
docs: https://docs.coresignal.com/integrations/coresignal-mcp
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Coresignal Scopes
name_suffix: OAuth Scopes
note: 'Coresignal''s REST data APIs use an api-key header and have NO scope surface at all. The only OAuth on the estate authenticates the MCP v2 server, and it is a sign-in flow, not a permissioning model: the four scopes below are the standard OIDC identity set, and the protected resource itself advertises scopes_supported: [] — meaning once a user signs in, the server resolves their team''s API key and the token carries the team''s full data entitlement. There is no read/write split, no per-dataset scope, and no way for an agent to request less than everything the team can see.'
overview: 'Coresignal publishes 4 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coresignal API on a user''s behalf.


  Tokens are issued from https://dashboard.coresignal.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coresignal
provider_slug: coresignal
schemes:
- end_session_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/end-session
  flows:
  - authorizationUrl: https://dashboard.coresignal.com/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/introspect
  issuer: https://dashboard.coresignal.com/api/auth
  jwks_uri: https://dashboard.coresignal.com/api/auth/jwks
  name: Coresignal Dashboard OAuth 2.1
  protects: https://mcp.coresignal.com/mcp/v2
  registration_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/register
  revocation_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/revoke
  source: https://dashboard.coresignal.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  userinfo_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/userinfo
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OIDC scope — request an ID token identifying the signed-in dashboard user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope — name, given_name, family_name, picture claims for the dashboard user.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope — email and email_verified claims for the dashboard user.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC scope — issue a refresh token so the MCP client can keep the session alive without re-prompting the user in the browser.
  flows:
  - authorizationCode
  scope: offline_access
slug: coresignal-scopes
source_filename: coresignal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  well-known/coresignal-oauth-authorization-server.json,\n  well-known/coresignal-openid-configuration.json,\n  well-known/coresignal-oauth-protected-resource.json\ndocs: https://docs.coresignal.com/integrations/coresignal-mcp\nnote: >-\n  Coresignal's REST data APIs use an api-key header and have NO scope surface at all. The only OAuth\n  on the estate authenticates the MCP v2 server, and it is a sign-in flow, not a permissioning model:\n  the four scopes below are the standard OIDC identity set, and the protected resource itself\n  advertises scopes_supported: [] — meaning once a user signs in, the server resolves their team's\n  API key and the token carries the team's full data entitlement. There is no read/write split, no\n  per-dataset scope, and no way for an agent to request less than everything the team can see.\nschemes:\n  - name: Coresignal Dashboard OAuth 2.1\n    source: https://dashboard.coresignal.com/.well-known/oauth-authorization-server\n\
  \    issuer: https://dashboard.coresignal.com/api/auth\n    protects: https://mcp.coresignal.com/mcp/v2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://dashboard.coresignal.com/api/auth/oauth2/authorize\n        tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://dashboard.coresignal.com/api/auth/oauth2/token\n    jwks_uri: https://dashboard.coresignal.com/api/auth/jwks\n    introspection_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/introspect\n    revocation_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/revoke\n    registration_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/register\n    userinfo_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/userinfo\n    end_session_endpoint: https://dashboard.coresignal.com/api/auth/oauth2/end-session\n\
  \    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    id_token_signing_alg: [RS256]\nscopes:\n  - scope: openid\n    description: Standard OIDC scope — request an ID token identifying the signed-in dashboard user.\n    flows: [authorizationCode]\n    sources: [well-known/coresignal-oauth-authorization-server.json]\n  - scope: profile\n    description: >-\n      Standard OIDC scope — name, given_name, family_name, picture claims for the dashboard user.\n    flows: [authorizationCode]\n    sources: [well-known/coresignal-oauth-authorization-server.json]\n  - scope: email\n    description: Standard OIDC scope — email and email_verified claims for the dashboard user.\n    flows: [authorizationCode]\n    sources: [well-known/coresignal-oauth-authorization-server.json]\n  - scope: offline_access\n    description: >-\n      Standard OIDC scope — issue a refresh token so the MCP client can keep the session alive without\n      re-prompting the user in the browser.\n\
  \    flows: [authorizationCode]\n    sources: [well-known/coresignal-oauth-authorization-server.json]\nresource_scopes:\n  resource: https://mcp.coresignal.com/mcp/v2\n  scopes_supported: []\n  bearer_methods_supported: [header]\n  interpretation: >-\n    The MCP resource declares an EMPTY scope list. Authorization is binary — a valid token for a team\n    grants every tool, including the credit-spending ones (entity_search at 20 credits, entity_fetch\n    at up to 20 credits per record, email_enrich at 10 credits per email). Spend control is handled by\n    the server's confirmation prompt before expensive calls, not by the token.\nclaims_supported: [sub, iss, aud, exp, iat, sid, scope, azp, email, email_verified, name, picture, family_name, given_name]\nrest_api_scopes:\n  present: false\n  note: >-\n    api.coresignal.com authenticates with a 32-character `apikey` header. Keys have no scopes and no\n    least-privilege model; entitlement is the plan attached to the account. Multiple\
  \ keys per account\n    can be generated and revoked, which is the only isolation mechanism available.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/scopes/coresignal-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Agentic Search
- B2B Data
- Companies
- Company Data
- Data as a Service
- Elasticsearch
- Employee Data
- Employees
- Enrichment
- Firmographics
- Job Postings
- Jobs
- Lead Generation
- People Data
- Sales Intelligence
- Talent Intelligence
- Web Data
token_urls:
- https://dashboard.coresignal.com/api/auth/oauth2/token
---
