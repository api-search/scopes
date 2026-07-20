---
api_specs:
- filename: lightrun-openapi-original.json
  format: json
  label: Lightrun Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightrun/refs/heads/main/openapi/lightrun-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.lightrun.com/public-api/introduction/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lightrun Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightrun uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightrun
provider_slug: lightrun
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: lightrun-scopes
source_filename: lightrun-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# Lightrun scopes and permission levels\ngenerated: '2026-07-19'\nmethod: searched\nsource: openapi/lightrun-openapi-original.json\ndocs: https://docs.lightrun.com/public-api/introduction/\nnotes: >-\n  Two distinct scope surfaces. (1) The Public REST API does not use OAuth — it authenticates\n  with a bearer API token — but it does have a real permission model: every operation\n  description states a \"Required API permission level\", and system API keys are minted with\n  an explicit scopes array. (2) The Lightrun identity realm (Keycloak, app.lightrun.com) is a\n  full OIDC provider whose scopes govern SSO and the MCP server. Both are recorded here; the\n  OIDC scopes are verbatim from the live discovery document.\napi_permission_levels:\n  applies_to: Public REST API bearer tokens\n  parameter: 'scopes (query, on createSystemApiKey)'\n  enum_source: openapi/lightrun-openapi-original.json#/paths/~1api~1v1~1access~1company~1{company}~1system-api-key/post\n  levels:\n    -\
  \ scope: DEV\n      description: >-\n        The debugging surface — actions (logs, snapshots, counters, metrics), agents, agent\n        pools, tags, custom sources, debug cases and runbooks. The level required by the\n        majority of operations.\n    - scope: COMPANY\n      description: >-\n        Tenant administration — IdM authentication and provisioning configuration, SMTP\n        connectivity, feature-flag toggles, license, and system API key management.\n    - scope: SECURITY\n      description: >-\n        Security surface, aligned with the Dynamic SBOM, loaded packages and watched packages\n        APIs. Declared in the system API key scopes enum.\n    - scope: CROSS_COMPANY\n      description: >-\n        Cross-tenant access. Declared in the system API key scopes enum; used for\n        multi-tenant deployments.\n  note: >-\n    The createSystemApiKey `scopes` parameter documents its values as (COMPANY, ENVIRONMENT,\n    APP_SEC) in prose while the schema enum is [COMPANY,\
  \ DEV, SECURITY, CROSS_COMPANY]. The\n    enum is recorded as authoritative; the prose appears to be a stale label set.\noidc:\n  applies_to: SSO and the Lightrun MCP server\n  issuer: https://app.lightrun.com/auth/realms/lightrun\n  discovery: well-known/lightrun-openid-configuration.json\n  authorization_endpoint: https://app.lightrun.com/auth/realms/lightrun/protocol/openid-connect/auth\n  token_endpoint: https://app.lightrun.com/auth/realms/lightrun/protocol/openid-connect/token\n  flows: [authorization_code, client_credentials, implicit, password, refresh_token, device_code, jwt-bearer, token-exchange, uma-ticket, ciba]\n  pkce: [plain, S256]\n  scopes:\n    - {scope: openid, description: Standard OIDC scope requesting an ID token.}\n    - {scope: profile, description: Standard OIDC profile claims.}\n    - {scope: email, description: Standard OIDC email claims.}\n    - {scope: address, description: Standard OIDC address claims.}\n    - {scope: phone, description: Standard OIDC phone\
  \ claims.}\n    - {scope: offline_access, description: Standard OIDC scope requesting a refresh token.}\n    - {scope: roles, description: Keycloak scope adding realm and client role claims.}\n    - {scope: mcp, description: Scope governing access to the Lightrun MCP server at https://app.lightrun.com/mcp.}\n    - {scope: service_account, description: Keycloak service-account scope for machine clients.}\n    - {scope: microprofile-jwt, description: Keycloak MicroProfile JWT claim set.}\n    - {scope: basic, description: Keycloak basic claim set.}\n    - {scope: web-origins, description: Keycloak scope adding allowed CORS origins to the token.}\n    - {scope: acr, description: Authentication context class reference claim.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightrun/refs/heads/main/scopes/lightrun-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Developer Tools
- Observability
- Debugging
- Monitoring
- Logging
- Application Performance
- Agent Skills
- Model Context Protocol
- DevOps
token_urls: []
---
