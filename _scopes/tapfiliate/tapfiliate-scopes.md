---
api_specs:
- filename: tapfiliate-affiliate-groups-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliate Groups API
  slug: tapfiliate-affiliate-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliate-groups-api-openapi.yml
- filename: tapfiliate-affiliate-prospects-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliate Prospects API
  slug: tapfiliate-affiliate-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliate-prospects-api-openapi.yml
- filename: tapfiliate-affiliates-api-openapi.yml
  format: yaml
  label: Tapfiliate Affiliates API
  slug: tapfiliate-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-affiliates-api-openapi.yml
- filename: tapfiliate-balances-api-openapi.yml
  format: yaml
  label: Tapfiliate Balances API
  slug: tapfiliate-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-balances-api-openapi.yml
- filename: tapfiliate-clicks-api-openapi.yml
  format: yaml
  label: Tapfiliate Clicks API
  slug: tapfiliate-clicks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-clicks-api-openapi.yml
- filename: tapfiliate-commissions-api-openapi.yml
  format: yaml
  label: Tapfiliate Commissions API
  slug: tapfiliate-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-commissions-api-openapi.yml
- filename: tapfiliate-conversions-api-openapi.yml
  format: yaml
  label: Tapfiliate Conversions API
  slug: tapfiliate-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-conversions-api-openapi.yml
- filename: tapfiliate-customers-api-openapi.yml
  format: yaml
  label: Tapfiliate Customers API
  slug: tapfiliate-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-customers-api-openapi.yml
- filename: tapfiliate-payments-api-openapi.yml
  format: yaml
  label: Tapfiliate Payments API
  slug: tapfiliate-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-payments-api-openapi.yml
- filename: tapfiliate-programs-api-openapi.yml
  format: yaml
  label: Tapfiliate Programs API
  slug: tapfiliate-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-programs-api-openapi.yml
authorization_urls: []
description: Tapfiliate's REST API v1.6 does NOT use OAuth — it authenticates with a static X-Api-Key header and the OpenAPI securitySchemes carry no oauth2 entry, so the derive pass over openapi/ finds no scopes. The only OAuth surface Tapfiliate operates is the one fronting its MCP server, and it publishes its scopes in machine-readable form. These four scope names are read verbatim from the provider's own protected-resource metadata document, not inferred.
docs: https://support.tapfiliate.com/en/articles/16011230-how-to-use-your-new-affiliate-analyst-the-tapfiliate-mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tapfiliate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tapfiliate publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tapfiliate API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tapfiliate
provider_slug: tapfiliate
schemes:
- authorizationUrl: https://app.tapfiliate.com/ai/mcp/connect/
  authorization_server: well-known/tapfiliate-mcp-oauth-authorization-server.json
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.tapfiliate.com
  jwks_uri: https://api.tapfiliate.com/.well-known/jwks.json
  name: Tapfiliate MCP OAuth
  pkce:
  - S256
  protected_resource: well-known/tapfiliate-mcp-oauth-protected-resource.json
  registrationUrl: https://app.tapfiliate.com/oauth/v2/register/
  resource: https://mcp.tapfiliate.com/mcp
  response_types:
  - code
  tokenUrl: https://mcp.tapfiliate.com/oauth/v2/token/
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 4
scope_names:
- affiliates
- conversions_commissions
- programs
- payments
scopes:
- description: Affiliate records and their organisation — affiliates, affiliate groups and affiliate prospects. Covers the Affiliates, Affiliate Groups and Affiliate Prospects tags in openapi/.
  flows: []
  scope: affiliates
- description: Tracked activity and its earnings — clicks, customers, conversions and the commissions generated from them. Covers the Conversions, Commissions, Clicks and Customers tags in openapi/.
  flows: []
  scope: conversions_commissions
- description: Affiliate programs, their settings, commission types, MLM levels and bonuses. Covers the Programs tag in openapi/.
  flows: []
  scope: programs
- description: Affiliate balances and payouts. Covers the Payments and Balances tags in openapi/.
  flows: []
  scope: payments
slug: tapfiliate-scopes
source_filename: tapfiliate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.tapfiliate.com/.well-known/oauth-protected-resource (HTTP 200) and\n  https://mcp.tapfiliate.com/.well-known/oauth-authorization-server (HTTP 200),\n  fetched anonymously. Both saved verbatim under well-known/.\ndocs: https://support.tapfiliate.com/en/articles/16011230-how-to-use-your-new-affiliate-analyst-the-tapfiliate-mcp-server\ndescription: >-\n  Tapfiliate's REST API v1.6 does NOT use OAuth — it authenticates with a static\n  X-Api-Key header and the OpenAPI securitySchemes carry no oauth2 entry, so the\n  derive pass over openapi/ finds no scopes. The only OAuth surface Tapfiliate\n  operates is the one fronting its MCP server, and it publishes its scopes in\n  machine-readable form. These four scope names are read verbatim from the\n  provider's own protected-resource metadata document, not inferred.\nschemes:\n  - name: Tapfiliate MCP OAuth\n    type: oauth2\n    resource: https://mcp.tapfiliate.com/mcp\n\
  \    issuer: https://api.tapfiliate.com\n    authorizationUrl: https://app.tapfiliate.com/ai/mcp/connect/\n    tokenUrl: https://mcp.tapfiliate.com/oauth/v2/token/\n    registrationUrl: https://app.tapfiliate.com/oauth/v2/register/\n    jwks_uri: https://api.tapfiliate.com/.well-known/jwks.json\n    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    pkce: [S256]\n    token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n    dynamic_client_registration: true\n    client_id_metadata_document_supported: true\n    bearer_methods: [header]\n    protected_resource: well-known/tapfiliate-mcp-oauth-protected-resource.json\n    authorization_server: well-known/tapfiliate-mcp-oauth-authorization-server.json\nscopes:\n  - scope: affiliates\n    description: >-\n      Affiliate records and their organisation — affiliates, affiliate groups and\n      affiliate prospects. Covers the Affiliates, Affiliate Groups and Affiliate\n      Prospects tags\
  \ in openapi/.\n    schemes: [Tapfiliate MCP OAuth]\n  - scope: conversions_commissions\n    description: >-\n      Tracked activity and its earnings — clicks, customers, conversions and the\n      commissions generated from them. Covers the Conversions, Commissions,\n      Clicks and Customers tags in openapi/.\n    schemes: [Tapfiliate MCP OAuth]\n  - scope: programs\n    description: >-\n      Affiliate programs, their settings, commission types, MLM levels and\n      bonuses. Covers the Programs tag in openapi/.\n    schemes: [Tapfiliate MCP OAuth]\n  - scope: payments\n    description: >-\n      Affiliate balances and payouts. Covers the Payments and Balances tags in\n      openapi/.\n    schemes: [Tapfiliate MCP OAuth]\nnotes:\n  - >-\n    Scope GRANULARITY is coarse: four scopes across a 77-operation surface, with\n    no read/write split. The write half is currently unreachable regardless —\n    the provider documents the MCP server as read-only in this beta — so the\n    scopes\
  \ describe data domains rather than permissions.\n  - >-\n    The authorization-server metadata declares issuer https://api.tapfiliate.com\n    but is served from https://mcp.tapfiliate.com; the issuer host itself 404s on\n    /.well-known/oauth-authorization-server. Recorded as observed.\n  - >-\n    The REST API has no OAuth path. An integration that is not an MCP client\n    authenticates with a long-lived account API key and therefore has no scoping\n    at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/scopes/tapfiliate-scopes.yml
summary_line: 4 scopes
tags:
- Affiliate Marketing
- Affiliate Tracking
- Commission Management
- Conversion Tracking
- Partner Programs
- Referral Programs
- Influencer Marketing
token_urls: []
---
