---
api_specs:
- filename: openapi.json
  format: json
  label: DomScan API
  slug: domscan-api
  spec_type: OpenAPI
  url: https://domscan.net/v1/openapi.json
authorization_urls: []
description: ''
docs: https://domscan.net/mcp-domain-checker
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Domscan Scopes
name_suffix: OAuth Scopes
note: 'The REST API authenticates with API keys (no OAuth scopes in the OpenAPI). OAuth 2.0 is used for the MCP endpoint: authorization-code flow with PKCE S256, dynamic client registration, public clients (token_endpoint_auth_methods_supported: none). One scope is published.'
overview: 'DomScan publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the DomScan API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DomScan
provider_slug: domscan
schemes: []
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Invoke DomScan MCP tools at https://domscan.net/mcp on behalf of the authorizing account.
  flows: []
  scope: mcp:tools
slug: domscan-scopes
source_filename: domscan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://domscan.net/.well-known/oauth-authorization-server\ndocs: https://domscan.net/mcp-domain-checker\nnote: 'The REST API authenticates with API keys (no OAuth scopes in the OpenAPI). OAuth 2.0 is used for the MCP endpoint: authorization-code flow\n  with PKCE S256, dynamic client registration, public clients (token_endpoint_auth_methods_supported: none). One scope is published.'\nauthorization:\n  issuer: https://domscan.net\n  authorization_endpoint: https://domscan.net/oauth/authorize\n  token_endpoint: https://domscan.net/oauth/token\n  registration_endpoint: https://domscan.net/oauth/register\n  grant_types:\n  - authorization_code\n  pkce:\n  - S256\nscopes:\n- scope: mcp:tools\n  description: Invoke DomScan MCP tools at https://domscan.net/mcp on behalf of the authorizing account.\n  source: scopes_supported in RFC 8414 metadata and RFC 9728 protected-resource metadata\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domscan/refs/heads/main/scopes/domscan-scopes.yml
summary_line: 1 scope
tags:
- Domains
- DNS
- WHOIS
- rdap
- SSL/TLS
- Email Security
- domain-valuation
- Brand Protection
- OSINT
- Threat Intelligence
- MCP
- agent-native
token_urls: []
---
