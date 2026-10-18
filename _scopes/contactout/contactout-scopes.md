---
api_specs:
- filename: contactout-api-usage-stats-api-openapi.yml
  format: yaml
  label: ContactOut API Usage Stats API
  slug: contactout-api-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-api-usage-stats-api-openapi.yml
- filename: contactout-campaigns-api-api-openapi.yml
  format: yaml
  label: ContactOut Campaigns API
  slug: contactout-campaigns-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-campaigns-api-api-openapi.yml
- filename: contactout-company-information-from-domains-api-openapi.yml
  format: yaml
  label: ContactOut Company information from domains API
  slug: contactout-company-information-from-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-company-information-from-domains-api-openapi.yml
- filename: contactout-company-search-api-api-openapi.yml
  format: yaml
  label: ContactOut Company Search API
  slug: contactout-company-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-company-search-api-api-openapi.yml
- filename: contactout-contact-checker-api-api-openapi.yml
  format: yaml
  label: ContactOut Contact Checker API
  slug: contactout-contact-checker-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-checker-api-api-openapi.yml
- filename: contactout-contact-info-api-bulk-api-openapi.yml
  format: yaml
  label: ContactOut Contact Info API - Bulk API
  slug: contactout-contact-info-api-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-info-api-bulk-api-openapi.yml
- filename: contactout-contact-info-api-single-api-openapi.yml
  format: yaml
  label: ContactOut Contact Info API - Single API
  slug: contactout-contact-info-api-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-info-api-single-api-openapi.yml
- filename: contactout-decision-makers-api-api-openapi.yml
  format: yaml
  label: ContactOut Decision Makers API
  slug: contactout-decision-makers-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-decision-makers-api-api-openapi.yml
- filename: contactout-email-to-linkedin-api-api-openapi.yml
  format: yaml
  label: ContactOut Email to LinkedIn API
  slug: contactout-email-to-linkedin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-email-to-linkedin-api-api-openapi.yml
- filename: contactout-email-verifier-api-api-openapi.yml
  format: yaml
  label: ContactOut Email Verifier API
  slug: contactout-email-verifier-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-email-verifier-api-api-openapi.yml
- filename: contactout-hashed-email-api-api-openapi.yml
  format: yaml
  label: ContactOut Hashed Email API
  slug: contactout-hashed-email-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-hashed-email-api-api-openapi.yml
- filename: contactout-linkedin-profile-api-api-openapi.yml
  format: yaml
  label: ContactOut LinkedIn Profile API
  slug: contactout-linkedin-profile-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-linkedin-profile-api-api-openapi.yml
- filename: contactout-people-count-api-api-openapi.yml
  format: yaml
  label: ContactOut People Count API
  slug: contactout-people-count-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-count-api-api-openapi.yml
- filename: contactout-people-enrich-api-api-openapi.yml
  format: yaml
  label: ContactOut People Enrich API
  slug: contactout-people-enrich-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-enrich-api-api-openapi.yml
- filename: contactout-people-search-api-api-openapi.yml
  format: yaml
  label: ContactOut People Search API
  slug: contactout-people-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-search-api-api-openapi.yml
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
