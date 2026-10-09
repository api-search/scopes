---
api_specs:
- filename: contactout-openapi-generated.yml
  format: yaml
  label: ContactOut API
  slug: contactout-api-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/_ae-authored/contactout-openapi-generated.yml
authorization_urls: []
description: ''
docs: https://api.contactout.com#contactout-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Contactout Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 (authorization code + PKCE S256, refresh_token, dynamic client registration) is used only for the hosted MCP server at https://contactout.com/mcp; the REST API authenticates with an API key in the token header and has no scopes. The authorization-server metadata advertises a single scope.
overview: 'ContactOut publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the ContactOut API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ContactOut
provider_slug: contactout
schemes: []
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: The only scope in scopes_supported of the authorization-server metadata; grants an MCP client use of the ContactOut MCP server on behalf of the user's API token.
  flows: []
  scope: mcp:use
slug: contactout-scopes
source_filename: contactout-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://contactout.com/.well-known/oauth-authorization-server\ndocs: https://api.contactout.com#contactout-mcp\nissuer: https://contactout.com\nnote: OAuth 2.0 (authorization code + PKCE S256, refresh_token, dynamic client registration) is used only for the hosted MCP server at https://contactout.com/mcp; the REST API authenticates with an API key in the token header and has no scopes. The authorization-server metadata advertises a single scope.\nscopes:\n- name: mcp:use\n  description: The only scope in scopes_supported of the authorization-server metadata; grants an MCP client use of the ContactOut MCP server on behalf of the user's API token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/scopes/contactout-scopes.yml
summary_line: 1 scope
tags:
- Company
- Contact Data
- Email Finder
- Data Enrichment
- People Search
- Company Search
- Email Verification
- Sales Intelligence
- Recruiting
- B2B Data
token_bound: false
token_urls: []
---
