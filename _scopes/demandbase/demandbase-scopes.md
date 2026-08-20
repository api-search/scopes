---
api_specs:
- filename: demandbase-b2b-openapi.yml
  format: yaml
  label: Demandbase B2B API
  slug: demandbase-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-b2b-openapi.yml
- filename: demandbase-data-export-openapi.yml
  format: yaml
  label: Demandbase Data Export API
  slug: demandbase-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-data-export-openapi.yml
- filename: demandbase-data-import-openapi.yml
  format: yaml
  label: Demandbase Data Import API
  slug: demandbase-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-data-import-openapi.yml
- filename: demandbase-intent-openapi.yml
  format: yaml
  label: Demandbase Intent API
  slug: demandbase-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-intent-openapi.yml
- filename: demandbase-admin-openapi.yml
  format: yaml
  label: Demandbase Admin API
  slug: demandbase-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-admin-openapi.yml
- filename: demandbase-usage-openapi.yml
  format: yaml
  label: Demandbase Usage API
  slug: demandbase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-usage-openapi.yml
- filename: demandbase-custom-sources-openapi.yml
  format: yaml
  label: Demandbase Custom Sources API
  slug: demandbase-custom-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-custom-sources-openapi.yml
- filename: demandbase-auth-openapi.yml
  format: yaml
  label: Demandbase Auth API
  slug: demandbase-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-auth-openapi.yml
authorization_urls:
- https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/authorize
description: ''
docs: https://developer.demandbase.com/docs/custom-mcp-clients
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Demandbase Scopes
name_suffix: OAuth Scopes
note: The REST platform APIs declare NO oauth2 security scheme and NO scopes — they use an opaque bearer token minted by a client-credentials exchange, with authorization decided server-side by the API Key Set's assigned permissions and the tenant's Export Collection. `python3 0-working/derive-oauth-scopes.py demandbase` therefore finds zero scopes in the OpenAPI, which is correct. The only real scope surface Demandbase publishes belongs to the MCP gateway, and it is recorded here from that server's own RFC 8414 / RFC 9728 metadata.
overview: 'Demandbase publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Demandbase API on a user''s behalf.


  Tokens are issued from https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Demandbase
provider_slug: demandbase
schemes:
- flows:
  - authorizationUrl: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://gateway.demandbase.com/mcp/v1/register
    tokenUrl: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/token
  issuer: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7
  name: MCP gateway OAuth
  source: well-known/demandbase-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication of the Demandbase user driving the MCP session.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated Demandbase user.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim for the authenticated Demandbase user.
  flows:
  - authorizationCode
  scope: email
- description: Refresh-token issuance so an agent session can outlive the initial access token.
  flows:
  - authorizationCode
  scope: offline_access
slug: demandbase-scopes
source_filename: demandbase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://gateway.demandbase.com/.well-known/oauth-protected-resource and\n  https://gateway.demandbase.com/.well-known/oauth-authorization-server (both HTTP 200,\n  saved verbatim under well-known/)\ndocs: https://developer.demandbase.com/docs/custom-mcp-clients\nnote: >-\n  The REST platform APIs declare NO oauth2 security scheme and NO scopes — they use an\n  opaque bearer token minted by a client-credentials exchange, with authorization decided\n  server-side by the API Key Set's assigned permissions and the tenant's Export Collection.\n  `python3 0-working/derive-oauth-scopes.py demandbase` therefore finds zero scopes in the\n  OpenAPI, which is correct. The only real scope surface Demandbase publishes belongs to the\n  MCP gateway, and it is recorded here from that server's own RFC 8414 / RFC 9728 metadata.\nsurfaces:\n  rest:\n    oauth2: false\n    scopes: []\n    authorization_model: >-\n      Permission Sets in\
  \ Demandbase One plus per-integration API Key Set permissions plus\n      the tenant's Export Collection entitlement. None of these are expressed as OAuth\n      scopes on the wire.\n  mcp:\n    oauth2: true\n    resource: https://gateway.demandbase.com/mcp/\n    authorization_servers:\n      - https://gateway.demandbase.com\nschemes:\n  - name: MCP gateway OAuth\n    source: well-known/demandbase-oauth-authorization-server.json\n    issuer: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/authorize\n        tokenUrl: https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/token\n        registrationUrl: https://gateway.demandbase.com/mcp/v1/register\n        pkce: S256\nscope_count: 4\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication of the Demandbase user driving the MCP session.\n    flows:\
  \ [authorizationCode]\n    sources: [well-known/demandbase-oauth-protected-resource.json, well-known/demandbase-oauth-authorization-server.json]\n  - scope: profile\n    description: Basic profile claims for the authenticated Demandbase user.\n    flows: [authorizationCode]\n    sources: [well-known/demandbase-oauth-protected-resource.json, well-known/demandbase-oauth-authorization-server.json]\n  - scope: email\n    description: Email claim for the authenticated Demandbase user.\n    flows: [authorizationCode]\n    sources: [well-known/demandbase-oauth-protected-resource.json, well-known/demandbase-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Refresh-token issuance so an agent session can outlive the initial access token.\n    flows: [authorizationCode]\n    sources: [well-known/demandbase-oauth-protected-resource.json, well-known/demandbase-oauth-authorization-server.json]\nobservation: >-\n  The MCP scope set is identity-only. There is no per-capability\
  \ scope — nothing that\n  separates \"read my accounts\" from \"read global company data\" from \"generate an account\n  brief\". Data-level authorization is enforced entirely by Demandbase One Permission Sets\n  after the token is presented, so the token itself carries no least-privilege signal an\n  agent operator can reason about or downscope.\nrelated:\n  - authentication/demandbase-authentication.yml\n  - well-known/demandbase-well-known.yml\n  - mcp/demandbase-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/scopes/demandbase-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Account Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Company Data
- Contact Data
- Data Enrichment
- Intent Data
- MCP
- Personalization
- Sales Intelligence
- Technographics
token_urls:
- https://authentication.demandbase.com/oauth2/aus7fu7m8kDj90Z532p7/v1/token
---
