---
api_specs:
- filename: datarails-financeos-mcp-openapi.json
  format: json
  label: Datarails FinanceOS MCP Server
  slug: financeos-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/openapi/datarails-financeos-mcp-openapi.json
authorization_urls:
- https://mcp.datarails.com/authorize
description: Datarails publishes exactly one OAuth scope. The FinanceOS MCP authorization server advertises scopes_supported ["datarails"] in both its RFC 8414 and its OIDC discovery documents — a single coarse scope that grants an agent the caller's whole readable FinanceOS surface. There is no read/write split, no per-table scope and no per-tool scope; granularity is delegated entirely to the tenant's in-app permission model and to per-tenant feature flags.
docs: https://support.datarails.com/hc/en-us/articles/25849710214556-Datarails-FinanceOS-MCP-Server-Technical-Documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Datarails Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Datarails publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Datarails API on a user''s behalf.


  Tokens are issued from https://mcp.datarails.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Datarails
provider_slug: datarails
schemes:
- flows:
  - authorizationUrl: https://mcp.datarails.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.datarails.com/token
  issuer: https://mcp.datarails.com/
  name: FinanceOS MCP OAuth 2.1
  source: https://mcp.datarails.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- datarails
scopes:
- description: 'Access the authenticated user''s Datarails FinanceOS data through the MCP server. Read-only in effect: Datarails documents that the MCP connection cannot create, update or delete records. Effective reach is bounded by the user''s existing Datarails permissions, enforced server-side.'
  flows:
  - authorizationCode
  scope: datarails
slug: datarails-scopes
source_filename: datarails-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://mcp.datarails.com/.well-known/oauth-authorization-server\ndocs: https://support.datarails.com/hc/en-us/articles/25849710214556-Datarails-FinanceOS-MCP-Server-Technical-Documentation\ndescription: >-\n  Datarails publishes exactly one OAuth scope. The FinanceOS MCP authorization\n  server advertises scopes_supported [\"datarails\"] in both its RFC 8414 and its\n  OIDC discovery documents — a single coarse scope that grants an agent the\n  caller's whole readable FinanceOS surface. There is no read/write split, no\n  per-table scope and no per-tool scope; granularity is delegated entirely to\n  the tenant's in-app permission model and to per-tenant feature flags.\n\nschemes:\n  - name: FinanceOS MCP OAuth 2.1\n    source: https://mcp.datarails.com/.well-known/oauth-authorization-server\n    issuer: https://mcp.datarails.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.datarails.com/authorize\n\
  \        tokenUrl: https://mcp.datarails.com/token\n\nscopes:\n  - scope: datarails\n    description: >-\n      Access the authenticated user's Datarails FinanceOS data through the MCP\n      server. Read-only in effect: Datarails documents that the MCP connection\n      cannot create, update or delete records. Effective reach is bounded by\n      the user's existing Datarails permissions, enforced server-side.\n    flows: [authorizationCode]\n    sources:\n      - https://mcp.datarails.com/.well-known/oauth-authorization-server\n      - https://mcp.datarails.com/.well-known/openid-configuration\n\ngranularity:\n  scope_count: 1\n  read_write_split: false\n  resource_indicators: false\n  effective_controls:\n    - control: tenant entitlement\n      description: FinanceOS AI connector must be enabled for the tenant and the user (paid feature, gated by the CSM).\n    - control: in-app permissions\n      description: Server-side enforcement of the caller's existing Datarails data-access permissions.\n\
  \    - control: feature flag use_semantic_layer_v2\n      description: Default-deny gate on the get_business_metric_* data tools.\n    - control: feature flag mcp_use_llm_sql_tool\n      description: Gate on the free-form sql_query tool.\n  assessment: >-\n    A single scope means an agent-consent screen cannot express least\n    privilege — a user granting \"datarails\" grants every readable table. The\n    real least-privilege boundary lives outside OAuth, in Datarails' own\n    permission model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datarails/refs/heads/main/scopes/datarails-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- FP&A
- Financial Planning
- Finance
- Accounting
- Budgeting
- Forecasting
- Business Intelligence
- Reporting
- Data Integration
- Model Context Protocol
- Artificial Intelligence
- Excel
- SaaS
token_urls:
- https://mcp.datarails.com/token
---
