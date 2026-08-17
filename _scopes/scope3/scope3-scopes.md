---
api_specs:
- filename: scope3-buyer-openapi-original.yml
  format: yaml
  label: Scope3 Interchange Buyer API
  slug: scope3-interchange-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/_original/scope3-buyer-openapi-original.yml
- filename: scope3-storefront-openapi-original.yml
  format: yaml
  label: Scope3 Interchange Storefront API
  slug: scope3-interchange-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/_original/scope3-storefront-openapi-original.yml
- filename: scope3-ai-impact-measurement-api-openapi.yml
  format: yaml
  label: Scope3 AI Impact Measurement API
  slug: scope3-ai-impact-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-ai-impact-measurement-api-openapi.yml
- filename: scope3-benchmarks-api-openapi.yml
  format: yaml
  label: Scope3 Benchmarks API
  slug: scope3-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-benchmarks-api-openapi.yml
- filename: scope3-creative-api-openapi.yml
  format: yaml
  label: Scope3 Creative API
  slug: scope3-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-creative-api-openapi.yml
- filename: scope3-data-api-openapi.yml
  format: yaml
  label: Scope3 Data API
  slug: scope3-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-data-api-openapi.yml
- filename: scope3-gpu-api-openapi.yml
  format: yaml
  label: Scope3 Gpu API
  slug: scope3-gpu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-gpu-api-openapi.yml
- filename: scope3-impact-api-openapi.yml
  format: yaml
  label: Scope3 Impact API
  slug: scope3-impact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-impact-api-openapi.yml
- filename: scope3-measure-api-openapi.yml
  format: yaml
  label: Scope3 Measure API
  slug: scope3-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-measure-api-openapi.yml
- filename: scope3-model-api-openapi.yml
  format: yaml
  label: Scope3 Model API
  slug: scope3-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-model-api-openapi.yml
- filename: scope3-node-api-openapi.yml
  format: yaml
  label: Scope3 Node API
  slug: scope3-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-node-api-openapi.yml
- filename: scope3-reload-api-openapi.yml
  format: yaml
  label: Scope3 Reload API
  slug: scope3-reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-reload-api-openapi.yml
- filename: scope3-saved-lists-api-openapi.yml
  format: yaml
  label: Scope3 Saved Lists API
  slug: scope3-saved-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-saved-lists-api-openapi.yml
- filename: scope3-segment-api-openapi.yml
  format: yaml
  label: Scope3 Segment API
  slug: scope3-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-segment-api-openapi.yml
- filename: scope3-signals-api-openapi.yml
  format: yaml
  label: Scope3 Signals API
  slug: scope3-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-signals-api-openapi.yml
- filename: scope3-status-api-openapi.yml
  format: yaml
  label: Scope3 Status API
  slug: scope3-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-status-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.interchange.io/v2/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Scope3 Scopes
name_suffix: OAuth Scopes
note: Neither published OpenAPI declares an oauth2 securityScheme — both use HTTP bearer (`bearerAuth`), so 0-working/derive-oauth-scopes.py finds nothing to derive. The OAuth scope surface is published outside the specs, in the discovery documents the Interchange MCP endpoints advertise. Everything below was read from those documents on 2026-08-13, not inferred from the specs.
overview: 'Scope3 publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Scope3 API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scope3
provider_slug: scope3
schemes:
- authorization_endpoint: https://api.interchange.io/authorize
  dynamic_client_registration: true
  flows:
  - flow: authorizationCode
    note: Public-client authorization code with PKCE — the shape a Claude/ChatGPT MCP connector uses.
    pkce: S256
    token_endpoint_auth_methods:
    - none
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.interchange.io
  name: interchange-mcp-oauth
  registration_endpoint: https://api.interchange.io/auth/register
  role: authorization server fronting the MCP endpoints
  scopes_note: This document publishes no scopes_supported. The protected resource it guards is https://api.interchange.io/mcp (RFC 9728 metadata at https://api.interchange.io/.well-known/oauth-protected-resource), and it names https://identity.scope3.com as a co-equal authorization server.
  scopes_published: false
  source: https://api.interchange.io/.well-known/oauth-authorization-server
  token_endpoint: https://api.interchange.io/auth/token
  type: oauth2
- authorization_endpoint: https://identity.scope3.com/oauth2/authorize
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://identity.scope3.com
  name: scope3-identity
  role: Scope3 identity provider
  scopes_published: true
  source: https://identity.scope3.com/.well-known/openid-configuration
  token_endpoint: https://identity.scope3.com/oauth2/token
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OIDC scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope granting access to basic profile claims.
  flows: []
  scope: profile
- description: Standard OIDC scope granting access to the email and email_verified claims.
  flows: []
  scope: email
- description: Requests a refresh token so the client can act without the user present.
  flows: []
  scope: offline_access
slug: scope3-scopes
source_filename: scope3-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://identity.scope3.com/.well-known/openid-configuration\ndocs: https://docs.interchange.io/v2/authentication\nnote: >-\n  Neither published OpenAPI declares an oauth2 securityScheme — both use HTTP bearer\n  (`bearerAuth`), so 0-working/derive-oauth-scopes.py finds nothing to derive. The OAuth scope\n  surface is published outside the specs, in the discovery documents the Interchange MCP\n  endpoints advertise. Everything below was read from those documents on 2026-08-13, not\n  inferred from the specs.\nidentity_provider:\n  vendor: WorkOS\n  vendor_source: https://docs.interchange.io/v2/authentication\n  note: Interchange documents WorkOS as its credential control plane.\nschemes:\n- name: interchange-mcp-oauth\n  type: oauth2\n  role: authorization server fronting the MCP endpoints\n  source: https://api.interchange.io/.well-known/oauth-authorization-server\n  issuer: https://api.interchange.io\n  authorization_endpoint:\
  \ https://api.interchange.io/authorize\n  token_endpoint: https://api.interchange.io/auth/token\n  registration_endpoint: https://api.interchange.io/auth/register\n  dynamic_client_registration: true\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    token_endpoint_auth_methods: [none]\n    note: Public-client authorization code with PKCE — the shape a Claude/ChatGPT MCP connector uses.\n  grant_types: [authorization_code, refresh_token]\n  scopes_published: false\n  scopes_note: >-\n    This document publishes no scopes_supported. The protected resource it guards is\n    https://api.interchange.io/mcp (RFC 9728 metadata at\n    https://api.interchange.io/.well-known/oauth-protected-resource), and it names\n    https://identity.scope3.com as a co-equal authorization server.\n- name: scope3-identity\n  type: openIdConnect\n  role: Scope3 identity provider\n  source: https://identity.scope3.com/.well-known/openid-configuration\n  issuer: https://identity.scope3.com\n  authorization_endpoint:\
  \ https://identity.scope3.com/oauth2/authorize\n  token_endpoint: https://identity.scope3.com/oauth2/token\n  grant_types: [authorization_code, client_credentials, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  scopes_published: true\nscopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token.\n  schemes: [scope3-identity]\n  sources: ['https://identity.scope3.com/.well-known/openid-configuration']\n- scope: profile\n  description: Standard OIDC scope granting access to basic profile claims.\n  schemes: [scope3-identity]\n  sources: ['https://identity.scope3.com/.well-known/openid-configuration']\n- scope: email\n  description: Standard OIDC scope granting access to the email and email_verified claims.\n  schemes: [scope3-identity]\n  sources: ['https://identity.scope3.com/.well-known/openid-configuration']\n- scope: offline_access\n  description: Requests a refresh token so the client can act without the user present.\n  schemes: [scope3-identity]\n\
  \  sources: ['https://identity.scope3.com/.well-known/openid-configuration']\nauthorization_model:\n  api_scopes: none\n  note: >-\n    Scope3 publishes only the four standard OIDC identity scopes; there is no product-level\n    scope vocabulary (no read:campaigns / write:storefront style permissions) in any discovery\n    document or in the docs. Interchange authorization is enforced by account role,\n    organization entitlement (e.g. the `modular-sources` entitlement) and persona (buyer vs\n    storefront) rather than by OAuth scope — a 403 carries FORBIDDEN, ACCESS_DENIED,\n    ALPHA_OPT_IN_REQUIRED or TOS_ACCEPTANCE_REQUIRED. Recorded as an honest absence.\ncross_links:\n  authentication: authentication/scope3-authentication.yml\n  well_known: well-known/scope3-well-known.yml\n  mcp: mcp/scope3-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/scopes/scope3-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Enterprise
- Advertising
- Carbon Emissions
- Sustainability
- AdTech
- Measurement
- Artificial Intelligence
- Agentic
- AdCP
- MCP
- Programmatic
- Media Buying
- Publishing
token_urls: []
---
