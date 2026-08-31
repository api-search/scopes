---
api_specs:
- filename: cb-insights-authorization-api-openapi.yml
  format: yaml
  label: CB Insights Authorization API
  slug: cb-insights-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-authorization-api-openapi.yml
- filename: cb-insights-businessrelationships-api-openapi.yml
  format: yaml
  label: CB Insights Business Relationships API
  slug: cb-insights-businessrelationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-businessrelationships-api-openapi.yml
- filename: cb-insights-chatcbi-api-openapi.yml
  format: yaml
  label: CB Insights Chat CBI API
  slug: cb-insights-chatcbi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-chatcbi-api-openapi.yml
- filename: cb-insights-financialtransactions-api-openapi.yml
  format: yaml
  label: CB Insights Financial Transactions API
  slug: cb-insights-financialtransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-financialtransactions-api-openapi.yml
- filename: cb-insights-firmographics-api-openapi.yml
  format: yaml
  label: CB Insights Firmographics API
  slug: cb-insights-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-firmographics-api-openapi.yml
- filename: cb-insights-managementandboard-api-openapi.yml
  format: yaml
  label: CB Insights Management And Board API
  slug: cb-insights-managementandboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-managementandboard-api-openapi.yml
- filename: cb-insights-organizations-api-openapi.yml
  format: yaml
  label: CB Insights Organizations API
  slug: cb-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-organizations-api-openapi.yml
- filename: cb-insights-outlook-api-openapi.yml
  format: yaml
  label: CB Insights Outlook API
  slug: cb-insights-outlook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-outlook-api-openapi.yml
- filename: cb-insights-revenue-api-openapi.yml
  format: yaml
  label: CB Insights Revenue API
  slug: cb-insights-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-revenue-api-openapi.yml
- filename: cb-insights-scoutingreports-api-openapi.yml
  format: yaml
  label: CB Insights Scouting Reports API
  slug: cb-insights-scoutingreports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-scoutingreports-api-openapi.yml
- filename: cb-insights-strategymap-api-openapi.yml
  format: yaml
  label: CB Insights Strategy Map API
  slug: cb-insights-strategymap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-strategymap-api-openapi.yml
authorization_urls:
- https://mcp.cbinsights.com/authorize
description: ''
docs:
- https://mcp.cbinsights.com/.well-known/oauth-authorization-server
- https://mcp.cbinsights.com/.well-known/oauth-protected-resource
- https://api-docs.cbinsights.com/portal/docs/Integrations/cbi-mcp-server
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Cb Insights Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CB Insights publishes 3 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CB Insights API on a user''s behalf.


  Tokens are issued from https://mcp.cbinsights.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CB Insights
provider_slug: cb-insights
schemes:
- applies_to: CB Insights MCP Server (https://mcp.cbinsights.com/)
  bearer_methods_supported:
  - header
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.cbinsights.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.cbinsights.com/token
  - flow: clientCredentials
    tokenUrl: https://mcp.cbinsights.com/token
  - flow: refreshToken
    tokenUrl: https://mcp.cbinsights.com/token
  issuer: https://mcp.cbinsights.com/
  metadata_document: well-known/cb-insights-mcp-oauth-authorization-server.json
  name: MCP OAuth 2.1
  registration_endpoint: https://mcp.cbinsights.com/register
  sources:
  - https://mcp.cbinsights.com/.well-known/oauth-authorization-server
  - https://mcp.cbinsights.com/.well-known/oauth-protected-resource
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect authentication — requests an ID token asserting who the end user is. Grants no data access of its own.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect claim scope — releases the end user's email address to the client.
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect claim scope — releases the end user's basic profile claims to the client.
  flows:
  - authorizationCode
  scope: profile
slug: cb-insights-scopes
source_filename: cb-insights-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.cbinsights.com/.well-known/oauth-authorization-server\ndocs:\n- https://mcp.cbinsights.com/.well-known/oauth-authorization-server\n- https://mcp.cbinsights.com/.well-known/oauth-protected-resource\n- https://api-docs.cbinsights.com/portal/docs/Integrations/cbi-mcp-server\nsummary: >-\n  Only one surface in the CB Insights estate has an OAuth scope model at all, and it is the hosted MCP\n  server — not the REST API. mcp.cbinsights.com runs a real RFC 8414 authorization server and\n  advertises exactly three scopes: openid, email and profile. All three are OpenID Connect identity\n  scopes. NOT ONE data scope is published, so an access token cannot be narrowed to a dataset, to\n  read-only, or to a spend ceiling — the token identifies the seat and the seat's full entitlement\n  follows. The REST APIs (v1 and v2) have no scope surface whatsoever: they use a bespoke\n  clientId/clientSecret exchange that returns a bare\
  \ {\"token\": ...} with no scope, no grant_type and\n  no token_type, and the published Swagger 2.0 contract declares an apiKey-in-header scheme rather\n  than oauth2. derive-oauth-scopes.py therefore finds zero oauth2 schemes in openapi/ — this file is\n  built from the live authorization-server metadata instead.\nderived_from_openapi: false\nopenapi_oauth2_schemes: 0\nopenapi_note: >-\n  Ran python3 all/0-working/derive-oauth-scopes.py cb-insights on 2026-08-14 — \"providers with\n  oauth2: 0, with scopes: 0\". The v2 contract's only securityDefinition is BearerAuth, an\n  apiKey-in-header scheme, so no scope can be derived from the spec.\nschemes:\n- name: MCP OAuth 2.1\n  type: oauth2\n  applies_to: CB Insights MCP Server (https://mcp.cbinsights.com/)\n  issuer: https://mcp.cbinsights.com/\n  metadata_document: well-known/cb-insights-mcp-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.cbinsights.com/authorize\n    tokenUrl:\
  \ https://mcp.cbinsights.com/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://mcp.cbinsights.com/token\n  - flow: refreshToken\n    tokenUrl: https://mcp.cbinsights.com/token\n  registration_endpoint: https://mcp.cbinsights.com/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  bearer_methods_supported:\n  - header\n  sources:\n  - https://mcp.cbinsights.com/.well-known/oauth-authorization-server\n  - https://mcp.cbinsights.com/.well-known/oauth-protected-resource\nscopes:\n- scope: openid\n  kind: identity\n  description: >-\n    OpenID Connect authentication — requests an ID token asserting who the end user is. Grants no data\n    access of its own.\n  flows: [authorizationCode]\n  sources: [https://mcp.cbinsights.com/.well-known/oauth-authorization-server]\n- scope: email\n  kind: identity\n  description: OpenID Connect claim scope — releases the end user's email address\
  \ to the client.\n  flows: [authorizationCode]\n  sources: [https://mcp.cbinsights.com/.well-known/oauth-authorization-server]\n- scope: profile\n  kind: identity\n  description: OpenID Connect claim scope — releases the end user's basic profile claims to the client.\n  flows: [authorizationCode]\n  sources: [https://mcp.cbinsights.com/.well-known/oauth-authorization-server]\nscope_count: 3\ndata_scope_count: 0\nprotected_resource:\n  resource: https://mcp.cbinsights.com/\n  authorization_servers:\n  - https://mcp.cbinsights.com/\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  file: well-known/cb-insights-mcp-oauth-protected-resource.json\n  rfc: RFC 9728\n  note: >-\n    The 401 challenge from the MCP endpoint itself carries resource_metadata pointing at this document,\n    so an MCP client can discover the authorization server correctly. What it discovers, however, is a\n    scope set that cannot express least privilege over the data.\nsurfaces_without_scopes:\n- surface:\
  \ CB Insights API v2\n  base_url: https://api.cbinsights.com\n  auth: bespoke clientId/clientSecret POST to /v2/authorize returning a 24-hour bearer JWT\n  scopes: none — the token carries no scope claim and none is documented\n  source: https://api-docs.cbinsights.com/portal/docs/CBI-API/cbi-authentication\n- surface: CB Insights API v1\n  base_url: https://api.cbinsights.com\n  auth: GET /v1/authorize with clientId and clientSecret as query parameters\n  scopes: none\n  source: https://api-docs.cbinsights.com/docs/tutorials/authentication_flow/\ngaps:\n- No data scopes anywhere. An agent connecting through Claude, ChatGPT, Perplexity or Copilot receives\n  a token that identifies the seat; entitlement and credit spend follow the seat, not the grant, so the\n  user cannot consent to a narrower slice than \"everything this seat can see\".\n- No read-only scope, so there is no token-level distinction between reading firmographics and\n  generating a billable scouting report or ChatCBI response.\n\
  - No scope reference page exists in the developer documentation — the three scopes are discoverable\n  only from the RFC 8414 metadata document, never from prose.\n- No token revocation or introspection endpoint is advertised, so a scope grant cannot be audited or\n  withdrawn programmatically.\nx-evidence:\n- url: https://mcp.cbinsights.com/.well-known/oauth-authorization-server\n  status: 200\n  fetched: '2026-08-14'\n  content_type: application/json\n- url: https://mcp.cbinsights.com/.well-known/oauth-protected-resource\n  status: 200\n  fetched: '2026-08-09'\n  content_type: application/json\ncross_links:\n  authentication: authentication/cb-insights-authentication.yml\n  mcp: mcp/cb-insights-mcp.yml\n  well_known: well-known/cb-insights-well-known.yml\n  conformance: conformance/cb-insights-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/scopes/cb-insights-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Market Intelligence
- private-company-data
- venture-capital
- funding-data
- investor-data
- company-data
- people-data
- business-relationships
- predictive-scoring
- MCP
- agent-native
- Data Enrichment
- snowflake
token_urls:
- https://mcp.cbinsights.com/token
---
