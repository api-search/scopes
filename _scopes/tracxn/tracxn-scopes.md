---
api_specs:
- filename: overview
  format: yaml
  label: Tracxn API
  slug: tracxn-api
  spec_type: Postman
  url: https://www.postman.com/tracxnapi/tracxn-api/overview
authorization_urls: []
description: 'Tracxn''s only OAuth surface is the MCP server; the REST API is API-key authenticated and has no scope model at all. The MCP authorization server advertises exactly ONE scope — `read` — in both its authorization-server metadata and its protected-resource metadata. There is no write scope because there is no write surface: every MCP tool and every REST endpoint is a query. Authorization is therefore coarse-grained by design; what a token can actually reach is governed by the customer''s Tracxn subscription entitlements and credit balance, not by the scope string.'
docs: https://help.tracxn.com/en/articles/14686877-what-is-tracxn-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tracxn Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tracxn uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tracxn
provider_slug: tracxn
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tracxn-scopes
source_filename: tracxn-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://platform.tracxn.com/.well-known/oauth-authorization-server/mcp (HTTP 200,\n  fetched 2026-08-14, saved verbatim at\n  well-known/tracxn-oauth-authorization-server-mcp.json) ;\n  https://platform.tracxn.com/.well-known/oauth-protected-resource/mcp (HTTP 200, saved at\n  well-known/tracxn-oauth-protected-resource-mcp.json) ;\n  RFC 9728 challenge returned by https://platform.tracxn.com/mcp\ndocs: https://help.tracxn.com/en/articles/14686877-what-is-tracxn-mcp\ndescription: >-\n  Tracxn's only OAuth surface is the MCP server; the REST API is API-key authenticated and has\n  no scope model at all. The MCP authorization server advertises exactly ONE scope — `read` —\n  in both its authorization-server metadata and its protected-resource metadata. There is no\n  write scope because there is no write surface: every MCP tool and every REST endpoint is a\n  query. Authorization is therefore coarse-grained by design; what\
  \ a token can actually reach\n  is governed by the customer's Tracxn subscription entitlements and credit balance, not by\n  the scope string.\nauthorization_server:\n  issuer: https://platform.tracxn.com/mcp\n  authorization_endpoint: https://platform.tracxn.com/auth/2.0/mcp/authorize\n  token_endpoint: https://platform.tracxn.com/auth/2.0/mcp/token\n  registration_endpoint: https://platform.tracxn.com/auth/2.0/mcp/register\n  grant_types_supported: [authorization_code]\n  response_types_supported: [code]\n  response_modes_supported: [query]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  authorization_response_iss_parameter_supported: true\nprotected_resource:\n  resource: https://platform.tracxn.com/mcp\n  authorization_servers:\n    - https://platform.tracxn.com/mcp\nscopes:\n  - name: read\n    description: >-\n      Read access to the Tracxn private-market dataset through the MCP server — companies,\n      legal entities, funding rounds,\
  \ acquisitions, investors, IPOs, time series, locations\n      and sectors. Advertised in scopes_supported by both the authorization-server and\n      protected-resource metadata. The sole scope Tracxn defines.\n    surface: mcp\n    grants: All 11 published MCP tools (see mcp/tracxn-mcp.yml)\n    write: false\nscope_count: 1\nnotes:\n  - >-\n    token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients — correct for\n    desktop/CLI MCP clients that cannot hold a secret, and consistent with the mandatory PKCE\n    S256 requirement.\n  - >-\n    Dynamic client registration is open at /auth/2.0/mcp/register, which is why a generic MCP\n    client can connect with nothing but the server URL.\n  - >-\n    The issuer and the resource are the same URL (https://platform.tracxn.com/mcp) — the MCP\n    server is its own authorization server rather than delegating to a separate platform IdP.\n  - >-\n    Entitlement, not scope, is the real access boundary: Tracxn's troubleshooting\
  \ guide tells\n    users that tools may appear but return errors when \"your subscription covers the data\n    you're querying (e.g. financials may require a higher tier)\". A `read` token does not\n    imply access to every dataset.\n  - >-\n    The REST API (accessToken header) has NO scopes and is not represented here. See\n    authentication/tracxn-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracxn/refs/heads/main/scopes/tracxn-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cloud Saas
- Market Intelligence
- Private Markets
- Venture Capital
- Startups
- Company Data
- Investors
- Funding
token_urls: []
---
