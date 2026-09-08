---
authorization_urls: []
description: ''
docs: https://docs.databricks.com/aws/en/dev-tools/auth/oauth-m2m
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Databricks Asset Bundles Scopes
name_suffix: OAuth Scopes
note: The baseline scope list is read verbatim from the RFC 8414 authorization server metadata document Databricks serves anonymously on the account console host — not from prose. The managed-MCP scopes below are read from the managed MCP documentation and are not present in scopes_supported.
overview: 'Databricks Asset Bundles uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Databricks Asset Bundles
provider_slug: databricks-asset-bundles
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: databricks-asset-bundles-scopes
source_filename: databricks-asset-bundles-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://accounts.cloud.databricks.com/oidc/.well-known/oauth-authorization-server\ndocs: https://docs.databricks.com/aws/en/dev-tools/auth/oauth-m2m\nnote: >-\n  The baseline scope list is read verbatim from the RFC 8414 authorization\n  server metadata document Databricks serves anonymously on the account console\n  host — not from prose. The managed-MCP scopes below are read from the\n  managed MCP documentation and are not present in scopes_supported.\nauthorization_server:\n  issuer: https://accounts.cloud.databricks.com/oidc\n  authorization_endpoint: https://accounts.cloud.databricks.com/oidc/v1/authorize\n  token_endpoint: https://accounts.cloud.databricks.com/oidc/v1/token\n  jwks_uri: https://accounts.cloud.databricks.com/oidc/jwks.json\n  grant_types_supported:\n    - client_credentials\n    - authorization_code\n    - refresh_token\n  code_challenge_methods_supported:\n    - S256\nscopes:\n  - name: all-apis\n    description:\
  \ >-\n      Full access to every Databricks REST API the principal is entitled to.\n      This is the scope the Databricks CLI (and therefore every `databricks\n      bundle` command) requests for OAuth U2M and M2M authentication.\n    source: scopes_supported\n  - name: sql\n    description: Access to Databricks SQL warehouses and query APIs.\n    source: scopes_supported\n  - name: openid\n    description: OIDC — request an ID token.\n    source: scopes_supported\n  - name: profile\n    description: OIDC — basic profile claims (name, family_name, given_name, preferred_username).\n    source: scopes_supported\n  - name: email\n    description: OIDC — email claim.\n    source: scopes_supported\n  - name: offline_access\n    description: Issue a refresh token so the CLI can renew without re-prompting.\n    source: scopes_supported\n  - name: genie\n    description: Access the Genie One / Genie Agent managed MCP servers.\n    source: managed-mcp-docs\n    docs: https://docs.databricks.com/aws/en/generative-ai/mcp/managed-mcp\n\
  \  - name: ai-search\n    description: Access the AI Search (vector search index) managed MCP server.\n    source: managed-mcp-docs\n    docs: https://docs.databricks.com/aws/en/generative-ai/mcp/managed-mcp\n  - name: unity-catalog\n    description: Access the Unity Catalog functions managed MCP server.\n    source: managed-mcp-docs\n    docs: https://docs.databricks.com/aws/en/generative-ai/mcp/managed-mcp\nscope_count: 9\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databricks-asset-bundles/refs/heads/main/scopes/databricks-asset-bundles-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CI/CD
- Data Engineering
- Databricks
- Deployment
- Infrastructure as Code
- Job
- Machine-Learning
- MLOps
- Pipelines
- Workflows
token_urls: []
---
