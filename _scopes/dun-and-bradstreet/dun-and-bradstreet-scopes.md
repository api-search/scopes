---
api_specs:
- filename: dun-and-bradstreet-authentication-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Authentication API
  slug: dun-and-bradstreet-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-authentication-api-openapi.yml
- filename: dun-and-bradstreet-data-file-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Data File API
  slug: dun-and-bradstreet-data-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-data-file-api-openapi.yml
- filename: dun-and-bradstreet-enrich-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Enrich API
  slug: dun-and-bradstreet-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-enrich-api-openapi.yml
- filename: dun-and-bradstreet-identity-resolution-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Identity Resolution API
  slug: dun-and-bradstreet-identity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-identity-resolution-api-openapi.yml
- filename: dun-and-bradstreet-monitoring-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Monitoring API
  slug: dun-and-bradstreet-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-monitoring-api-openapi.yml
- filename: dun-and-bradstreet-multi-process-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Multi-Process API
  slug: dun-and-bradstreet-multi-process-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-multi-process-api-openapi.yml
- filename: dun-and-bradstreet-research-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Research API
  slug: dun-and-bradstreet-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-research-api-openapi.yml
- filename: dun-and-bradstreet-search-api-openapi.yml
  format: yaml
  label: Dun & Bradstreet Search API
  slug: dun-and-bradstreet-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/openapi/dun-and-bradstreet-search-api-openapi.yml
authorization_urls:
- https://agents.riskanalytics.dnb.com/authorize
description: OAuth scope surface for Dun & Bradstreet. The Direct+ REST OpenAPI declares no oauth2 securityScheme (it models the token exchange as an explicit operation plus http basic/bearer), so derive-oauth-scopes.py finds nothing there. The real scope surface is published by the D&B Risk Analytics remote MCP server, which serves RFC 8414 authorization-server metadata anonymously. Every scope below was read verbatim from that document.
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Dun And Bradstreet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dun & Bradstreet publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dun & Bradstreet API on a user''s behalf.


  Tokens are issued from https://agents.riskanalytics.dnb.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dun & Bradstreet
provider_slug: dun-and-bradstreet
schemes:
- flows:
  - authorizationUrl: https://agents.riskanalytics.dnb.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://agents.riskanalytics.dnb.com/token
  - flow: clientCredentials
    tokenUrl: https://agents.riskanalytics.dnb.com/token
  issuer: https://agents.riskanalytics.dnb.com
  name: D&B Risk Analytics MCP authorization server
  protected_resource: https://agents.riskanalytics.dnb.com/mcp
  refresh_token: true
  source: https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
scope_count: 6
scope_names:
- mcp.read
- mcp.write
- offline_access
- openid
- email
- profile
scopes:
- description: Read access to the D&B Risk Analytics MCP surface. Description is inferred from the scope name; D&B publishes no scope reference page.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp.read
- description: Write access to the D&B Risk Analytics MCP surface. Description is inferred from the scope name; D&B publishes no scope reference page.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp.write
- description: Issue a refresh token so the client can reconnect without re-authorizing.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect authentication (standard OIDC scope).
  flows:
  - authorizationCode
  scope: openid
- description: Release the authenticated user's email address (standard OIDC scope).
  flows:
  - authorizationCode
  scope: email
- description: Release the authenticated user's profile claims (standard OIDC scope).
  flows:
  - authorizationCode
  scope: profile
slug: dun-and-bradstreet-scopes
source_filename: dun-and-bradstreet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server\ndescription: >-\n  OAuth scope surface for Dun & Bradstreet. The Direct+ REST OpenAPI declares\n  no oauth2 securityScheme (it models the token exchange as an explicit\n  operation plus http basic/bearer), so derive-oauth-scopes.py finds nothing\n  there. The real scope surface is published by the D&B Risk Analytics remote\n  MCP server, which serves RFC 8414 authorization-server metadata anonymously.\n  Every scope below was read verbatim from that document.\n\nschemes:\n  - name: D&B Risk Analytics MCP authorization server\n    source: https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server\n    issuer: https://agents.riskanalytics.dnb.com\n    protected_resource: https://agents.riskanalytics.dnb.com/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://agents.riskanalytics.dnb.com/authorize\n     \
  \   tokenUrl: https://agents.riskanalytics.dnb.com/token\n        pkce: [S256, plain]\n      - flow: clientCredentials\n        tokenUrl: https://agents.riskanalytics.dnb.com/token\n    refresh_token: true\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n\nscopes:\n  - scope: mcp.read\n    description: >-\n      Read access to the D&B Risk Analytics MCP surface. Description is\n      inferred from the scope name; D&B publishes no scope reference page.\n    flows: [authorizationCode, clientCredentials]\n    sources: [https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server]\n  - scope: mcp.write\n    description: >-\n      Write access to the D&B Risk Analytics MCP surface. Description is\n      inferred from the scope name; D&B publishes no scope reference page.\n    flows: [authorizationCode, clientCredentials]\n    sources: [https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server]\n  - scope: offline_access\n    description:\
  \ Issue a refresh token so the client can reconnect without re-authorizing.\n    flows: [authorizationCode]\n    sources: [https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server]\n  - scope: openid\n    description: OpenID Connect authentication (standard OIDC scope).\n    flows: [authorizationCode]\n    sources: [https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server]\n  - scope: email\n    description: Release the authenticated user's email address (standard OIDC scope).\n    flows: [authorizationCode]\n    sources: [https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server]\n  - scope: profile\n    description: Release the authenticated user's profile claims (standard OIDC scope).\n    flows: [authorizationCode]\n    sources: [https://agents.riskanalytics.dnb.com/.well-known/oauth-authorization-server]\n\nother_credentials:\n  - name: Direct+ client_credentials token exchange\n    scopes: none\n    note: >-\n      POST https://plus.dnb.com/v3/token\
  \ with grant_type=client_credentials\n      and HTTP Basic (consumer key : consumer secret) returns a bearer JWT.\n      The exchange carries NO scope parameter — Direct+ entitlement is\n      contract-driven (which Data Blocks a customer licensed), not\n      scope-driven. See authentication/dun-and-bradstreet-authentication.yml.\n  - name: Dplus-API-Key\n    scopes: none\n    note: >-\n      The Commercial Graph / Direct+ MCP server authenticates with a single\n      API key header and exposes no scope surface.\n\nabsences:\n  - No scope reference / permissions page published by D&B.\n  - >-\n    The scopes_supported list advertises openid/email/profile but the host\n    serves no /.well-known/openid-configuration (404).\n  - The Direct+ REST API has no OAuth scope model at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dun-and-bradstreet/refs/heads/main/scopes/dun-and-bradstreet-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Business Data
- Company Data
- D-U-N-S Number
- Credit
- Risk
- Master Data
- Data Enrichment
- Identity Resolution
- Compliance
- Supply Chain
- Sales Intelligence
- Monitoring
token_urls:
- https://agents.riskanalytics.dnb.com/token
---
