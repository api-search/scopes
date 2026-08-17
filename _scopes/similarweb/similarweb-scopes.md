---
api_specs:
- filename: similarweb-account-api-openapi.yml
  format: yaml
  label: SimilarWeb Account API
  slug: similarweb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-account-api-openapi.yml
- filename: similarweb-app-intelligence-api-openapi.yml
  format: yaml
  label: SimilarWeb App Intelligence API
  slug: similarweb-app-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-app-intelligence-api-openapi.yml
- filename: similarweb-credits-api-openapi.yml
  format: yaml
  label: SimilarWeb Credits API
  slug: similarweb-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-credits-api-openapi.yml
- filename: similarweb-geography-api-openapi.yml
  format: yaml
  label: SimilarWeb Geography API
  slug: similarweb-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-geography-api-openapi.yml
- filename: similarweb-integrations-api-openapi.yml
  format: yaml
  label: SimilarWeb Integrations API
  slug: similarweb-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-integrations-api-openapi.yml
- filename: similarweb-keywords-api-openapi.yml
  format: yaml
  label: SimilarWeb Keywords API
  slug: similarweb-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-keywords-api-openapi.yml
- filename: similarweb-lead-enrichment-api-openapi.yml
  format: yaml
  label: SimilarWeb Lead Enrichment API
  slug: similarweb-lead-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-lead-enrichment-api-openapi.yml
- filename: similarweb-rankings-api-openapi.yml
  format: yaml
  label: SimilarWeb Rankings API
  slug: similarweb-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-rankings-api-openapi.yml
- filename: similarweb-reports-api-openapi.yml
  format: yaml
  label: SimilarWeb Reports API
  slug: similarweb-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-reports-api-openapi.yml
- filename: similarweb-similar-sites-api-openapi.yml
  format: yaml
  label: SimilarWeb Similar Sites API
  slug: similarweb-similar-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-similar-sites-api-openapi.yml
- filename: similarweb-traffic-and-engagement-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic and Engagement API
  slug: similarweb-traffic-and-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-and-engagement-api-openapi.yml
- filename: similarweb-traffic-sources-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic Sources API
  slug: similarweb-traffic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-sources-api-openapi.yml
- filename: similarweb-webhooks-api-openapi.yml
  format: yaml
  label: SimilarWeb Webhooks API
  slug: similarweb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-webhooks-api-openapi.yml
authorization_urls:
- https://mcp-auth.similarweb.com/authorize
description: 'Similarweb''s REST and Batch APIs have NO OAuth surface — they authenticate with an `api-key` header and declare no oauth2 securityScheme in any OpenAPI in this repo (derive-oauth-scopes.py found 0 oauth2 schemes across 13 specs). The only OAuth surface Similarweb operates is in front of its hosted MCP server, and it is deliberately minimal: a single `read` scope covering the whole resource. There is no per-dataset or per-endpoint scope model, so an OAuth-issued MCP token is all-or-nothing over whatever the underlying subscription entitles. Entitlement, not scope, is what actually bounds access at Similarweb — countries, datasets and history windows come from the plan and are introspected with the Check Capabilities operation, not from a token claim.'
docs: https://docs.similarweb.com/api-v5/similarweb-mcp/mcp-setup
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Similarweb Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SimilarWeb publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SimilarWeb API on a user''s behalf.


  Tokens are issued from https://mcp-auth.similarweb.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SimilarWeb
provider_slug: similarweb
schemes:
- applies_to: https://mcp.similarweb.com
  flows:
  - authorizationUrl: https://mcp-auth.similarweb.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    refresh: true
    tokenUrl: https://mcp-auth.similarweb.com/token
  issuer: https://mcp-auth.similarweb.com
  name: MCP OAuth 2.1
  registration_endpoint: https://mcp-auth.similarweb.com/register
  revocation_endpoint: https://mcp-auth.similarweb.com/revoke
  source: https://mcp-auth.similarweb.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - none
scope_count: 1
scope_names:
- read
scopes:
- description: Read access to the Similarweb datasets exposed through the MCP server. The only scope advertised by either the protected-resource or the authorization-server metadata.
  flows:
  - authorizationCode
  scope: read
slug: similarweb-scopes
source_filename: similarweb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.similarweb.com/.well-known/oauth-protected-resource\ndescription: >-\n  Similarweb's REST and Batch APIs have NO OAuth surface — they authenticate with an\n  `api-key` header and declare no oauth2 securityScheme in any OpenAPI in this repo\n  (derive-oauth-scopes.py found 0 oauth2 schemes across 13 specs). The only OAuth surface\n  Similarweb operates is in front of its hosted MCP server, and it is deliberately\n  minimal: a single `read` scope covering the whole resource. There is no per-dataset or\n  per-endpoint scope model, so an OAuth-issued MCP token is all-or-nothing over whatever\n  the underlying subscription entitles. Entitlement, not scope, is what actually bounds\n  access at Similarweb — countries, datasets and history windows come from the plan and\n  are introspected with the Check Capabilities operation, not from a token claim.\n\ndocs: https://docs.similarweb.com/api-v5/similarweb-mcp/mcp-setup\n\n\
  schemes:\n- name: MCP OAuth 2.1\n  applies_to: https://mcp.similarweb.com\n  source: https://mcp-auth.similarweb.com/.well-known/oauth-authorization-server\n  issuer: https://mcp-auth.similarweb.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp-auth.similarweb.com/authorize\n    tokenUrl: https://mcp-auth.similarweb.com/token\n    refresh: true\n    pkce: [S256, plain]\n  registration_endpoint: https://mcp-auth.similarweb.com/register\n  revocation_endpoint: https://mcp-auth.similarweb.com/revoke\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\n\nscopes:\n- scope: read\n  description: >-\n    Read access to the Similarweb datasets exposed through the MCP server. The only scope\n    advertised by either the protected-resource or the authorization-server metadata.\n  flows: [authorizationCode]\n  sources:\n  - https://mcp.similarweb.com/.well-known/oauth-protected-resource\n  - https://mcp-auth.similarweb.com/.well-known/oauth-authorization-server\n\
  \nscope_count: 1\n\nentitlement_model:\n  note: >-\n    Effective access is bounded by subscription entitlement rather than token scope.\n    Callers should introspect it at runtime.\n  introspection_operation: checkCapabilities\n  introspection_path: /v1/website/{domain_name}/capabilities\n  bounded_by: [countries, datasets, historical date range, data-credit balance]\n  error_on_out_of_scope: 103 Country not available\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: https://mcp.similarweb.com/.well-known/oauth-protected-resource, http_status: 200}\n  - {url: https://mcp-auth.similarweb.com/.well-known/oauth-authorization-server, http_status: 200}\n  - {url: 'https://mcp-auth.similarweb.com/.well-known/openid-configuration', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/scopes/similarweb-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-commerce
- SEO
token_urls:
- https://mcp-auth.similarweb.com/token
---
