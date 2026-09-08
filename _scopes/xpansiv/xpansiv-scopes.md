---
api_specs:
- filename: xpansiv-connect-openapi.yml
  format: yaml
  label: Xpansiv Connect API
  slug: xpansiv-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-connect-openapi.yml
- filename: xpansiv-managed-solutions-openapi.yml
  format: yaml
  label: Xpansiv Managed Solutions API
  slug: xpansiv-managed-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-managed-solutions-openapi.yml
- filename: xpansiv-nar-registry-client-openapi.yml
  format: yaml
  label: NAR Registry Client API
  slug: xpansiv-nar-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-nar-registry-client-openapi.yml
- filename: xpansiv-tigr-registry-client-openapi.yml
  format: yaml
  label: TIGRS Registry Client API
  slug: xpansiv-tigr-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-tigr-registry-client-openapi.yml
- filename: xpansiv-optimal-system-openapi.yml
  format: yaml
  label: Xpansiv Optimal Outcomes APIs
  slug: xpansiv-optimal-outcomes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-optimal-system-openapi.yml
- filename: xpansiv-apx-power-markets-file-registry-openapi.yml
  format: yaml
  label: APX Power Markets File Registry API
  slug: xpansiv-apx-power-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-apx-power-markets-file-registry-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Xpansiv Scopes
name_suffix: OAuth Scopes
note: 'derive-oauth-scopes.py returned "providers with oauth2: 0" — none of the eleven OpenAPI descriptions declares an oauth2 securityScheme, so there is nothing to derive from the contracts. Every scope below was read from a discovery document that was actually fetched, or from the provider''s own authentication pages. THERE IS NO PUBLISHED API-PERMISSION SCOPE REFERENCE: Xpansiv does not document a scope vocabulary that grants or restricts access to Connect, registry, Optimal or Managed Solutions operations. Authorisation is carried by the account and credentials Xpansiv issues, not by a scope string the client chooses. An integrator cannot request least privilege.'
overview: 'Xpansiv uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xpansiv
provider_slug: xpansiv
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: xpansiv-scopes
source_filename: xpansiv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://auth.xpansiv.com/.well-known/openid-configuration (200) ,\n  https://developer.xpansiv.com/.well-known/oauth-protected-resource/mcp (200) ,\n  https://developer.xpansiv.com/developer-portal/nar-registry/authentication ,\n  https://developer.xpansiv.com/developer-portal/xpansiv-connect/getting-started\nprovider: Xpansiv\nnote: >-\n  derive-oauth-scopes.py returned \"providers with oauth2: 0\" — none of the eleven OpenAPI\n  descriptions declares an oauth2 securityScheme, so there is nothing to derive from the\n  contracts. Every scope below was read from a discovery document that was actually\n  fetched, or from the provider's own authentication pages. THERE IS NO PUBLISHED\n  API-PERMISSION SCOPE REFERENCE: Xpansiv does not document a scope vocabulary that\n  grants or restricts access to Connect, registry, Optimal or Managed Solutions\n  operations. Authorisation is carried by the account and credentials Xpansiv\
  \ issues, not\n  by a scope string the client chooses. An integrator cannot request least privilege.\nscope_reference_published: false\ndocs: null\nauthorization_servers:\n- issuer: https://auth.xpansiv.com/\n  discovery: https://auth.xpansiv.com/.well-known/openid-configuration\n  serves: Xpansiv Connect API, Xpansiv Data API\n  platform: Auth0\n  token_endpoint: https://auth.xpansiv.com/oauth/token\n  jwks_uri: https://auth.xpansiv.com/.well-known/jwks.json\n  code_challenge_methods_supported: [S256, plain]\n  scopes_supported:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n  - phone\n  - address\n  scope_kind: identity\n  note: >-\n    These are the standard OIDC identity claims the Auth0 tenant advertises, not API\n    permissions. The Connect getting-started example passes a literal placeholder\n    `scope=SCOPE` in its token request and never says what\
  \ a real value would be, and the\n    successful response it shows returns `\"scope\": \"\"` — an empty scope. In practice the\n    audience (https://xpansiv/platform) selects the API and the account selects the\n    rights.\n- issuer: https://apxjwtauthprod.apx.com/oauth/token\n  discovery: none published (host returns 403 on every /.well-known/ path)\n  serves: NAR Registry Client API, TIGRS Registry Client API, APX Power Markets File\n    Registry API\n  uat: https://apxjwtauthuat.apx.com/oauth/token\n  grant_type: password (RFC 6749 §4.3.2)\n  client_authentication: 'HTTP Basic {clientId:clientSecret}'\n  scopes_supported:\n  - name: access\n    description: >-\n      The single scope value this authorization server returns. The published Results\n      table states verbatim: \"scope — The scope of the granted access. The value returned\n      will be 'access'.\" It is not requestable, not subdividable, and grants whatever the\n      Client API Service user account is entitled to.\n\
  \  scope_kind: fixed single value\n  source: https://developer.xpansiv.com/developer-portal/nar-registry/authentication and\n    https://developer.xpansiv.com/developer-portal/xpansiv-power/rest_api/authentication\n- issuer: https://auth.cloud.redocly.com\n  discovery: https://developer.xpansiv.com/.well-known/oauth-authorization-server\n  serves: the developer portal and its MCP server at https://developer.xpansiv.com/mcp\n  protected_resource_metadata: https://developer.xpansiv.com/.well-known/oauth-protected-resource/mcp\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - offline_access\n  scope_kind: identity\n  note: >-\n    Docs-platform authentication (Redocly) reached through Xpansiv's own host. Governs\n    the documentation MCP server, not any Xpansiv business API. tools/list answered\n    anonymously.\n- issuer: https://support.xpansiv.com\n  discovery: https://support.xpansiv.com/.well-known/openid-configuration\n  serves: the Salesforce Experience Cloud support community\n\
  \  scope_kind: identity\n  note: Support portal sign-in; unrelated to API authorisation.\nnon_oauth_credentials:\n- api: Xpansiv Managed Solutions API\n  model: bearer API key\n  issued_at: https://www.ms.xpansiv.com/app/api_access/manage\n  scope_model: >-\n    None. The provider states the key \"is linked to a user and an account, and has the\n    same rights as\" that user — a full-privilege credential with no scoping, no\n    per-endpoint restriction and no read-only variant. This is the widest-blast-radius\n    credential in the Xpansiv catalog and is worth flagging to any integrator.\n  source: https://developer.xpansiv.com/developer-portal/xpansiv-managed-solutions/authorization\n- api: Xpansiv Data API\n  model: Basic auth exchanged for a JWT + refresh token, or an NG_API_KEY, or Auth0 SSO\n  scope_model: none published\n  source: https://developer.xpansiv.com/developer-portal/xpansiv-data/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/scopes/xpansiv-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Environmental Commodities
- Carbon Markets
- Renewable Energy Certificates
- Registries
- Market Data
- Trading
- Energy
- Sustainability
- Climate
token_urls: []
---
