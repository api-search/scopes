---
api_specs:
- filename: overview
  format: yaml
  label: SE Ranking Data API
  slug: data-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: overview
  format: yaml
  label: SE Ranking Project API
  slug: project-api
  spec_type: Postman
  url: https://www.postman.com/serankingdev/se-ranking-developers/overview
- filename: se-ranking-account-system-api-openapi.yml
  format: yaml
  label: SE Ranking Account & system API
  slug: se-ranking-account-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-account-system-api-openapi.yml
- filename: se-ranking-ai-search-api-openapi.yml
  format: yaml
  label: SE Ranking AI search API
  slug: se-ranking-ai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-ai-search-api-openapi.yml
- filename: se-ranking-backlinks-api-openapi.yml
  format: yaml
  label: SE Ranking backlinks API
  slug: se-ranking-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-backlinks-api-openapi.yml
- filename: se-ranking-domain-analysis-api-openapi.yml
  format: yaml
  label: SE Ranking Domain Analysis API
  slug: se-ranking-domain-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-domain-analysis-api-openapi.yml
- filename: se-ranking-keyword-research-api-openapi.yml
  format: yaml
  label: SE Ranking Keyword Research API
  slug: se-ranking-keyword-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-keyword-research-api-openapi.yml
- filename: se-ranking-serp-results-classic-api-openapi.yml
  format: yaml
  label: SE Ranking SERP Results > classic API
  slug: se-ranking-serp-results-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-serp-results-classic-api-openapi.yml
- filename: se-ranking-website-audit-api-openapi.yml
  format: yaml
  label: SE Ranking Website Audit API
  slug: se-ranking-website-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/openapi/se-ranking-website-audit-api-openapi.yml
authorization_urls:
- https://seranking.com/wp-json/seranking-mcp-oauth/v1/authorize
description: ''
docs: https://seranking.com/api/mcp/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Se Ranking Scopes
name_suffix: OAuth Scopes
note: 'SE Ranking''s REST OpenAPI declares no oauth2 scheme (apiKey only), so there are no REST scopes. The OAuth surface belongs entirely to the hosted MCP server: an RFC 8414 authorization server at https://seranking.com issuing tokens for the MCP resource. It advertises exactly ONE scope, `mcp`, which is coarse — a granted token carries the whole 217-tool surface including destructive PROJECT_delete*/SEV_delete* tools. Recorded as published, not as an endorsement.'
overview: 'SE Ranking publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SE Ranking API on a user''s behalf.


  Tokens are issued from https://seranking.com/wp-json/seranking-mcp-oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SE Ranking
provider_slug: se-ranking
schemes:
- flows:
  - authorizationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/register
    revocationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/revoke
    tokenUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/token
    token_endpoint_auth_methods:
    - none
  name: MCP OAuth 2.1
  source: https://seranking.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Full access to the SE Ranking MCP server at https://api.seranking.com/mcp — all 217 tools across the DATA, PROJECT and SE Visible namespaces.
  flows:
  - authorizationCode
  scope: mcp
slug: se-ranking-scopes
source_filename: se-ranking-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://seranking.com/.well-known/oauth-authorization-server\ndocs: https://seranking.com/api/mcp/\nnote: 'SE Ranking''s REST OpenAPI declares no oauth2 scheme (apiKey only), so there are no REST scopes. The OAuth surface belongs entirely\n  to the hosted MCP server: an RFC 8414 authorization server at https://seranking.com issuing tokens for the MCP resource. It advertises\n  exactly ONE scope, `mcp`, which is coarse — a granted token carries the whole 217-tool surface including destructive PROJECT_delete*/SEV_delete*\n  tools. Recorded as published, not as an endorsement.'\nschemes:\n- name: MCP OAuth 2.1\n  source: https://seranking.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/authorize\n    tokenUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/token\n    revocationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/revoke\n\
  \    registrationUrl: https://seranking.com/wp-json/seranking-mcp-oauth/v1/register\n    pkce:\n    - S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    token_endpoint_auth_methods:\n    - none\nscopes:\n- scope: mcp\n  description: Full access to the SE Ranking MCP server at https://api.seranking.com/mcp — all 217 tools across the DATA, PROJECT and\n    SE Visible namespaces.\n  flows:\n  - authorizationCode\n  sources:\n  - https://seranking.com/.well-known/oauth-authorization-server\nprotected_resource:\n  resource: https://seranking.com/wp-json/seranking-mcp-oauth/v1/mcp\n  authorization_servers:\n  - https://seranking.com\n  bearer_methods_supported:\n  - header\n  source: https://seranking.com/.well-known/oauth-protected-resource\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/se-ranking/refs/heads/main/scopes/se-ranking-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- SEO
- Keyword Research
- Rank Tracking
- Backlinks
- Competitor Analysis
- Website Audit
- AI Search
- Geo
- Digital Marketing
- MCP
- AI Agents
- Agent Skills
token_urls:
- https://seranking.com/wp-json/seranking-mcp-oauth/v1/token
---
