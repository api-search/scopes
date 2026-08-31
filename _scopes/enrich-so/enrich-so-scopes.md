---
api_specs:
- filename: enrich-so-email-finder-api-openapi.yml
  format: yaml
  label: Enrich Email Finder API
  slug: enrich-so-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-email-finder-api-openapi.yml
- filename: enrich-so-lead-finder-api-openapi.yml
  format: yaml
  label: Enrich Lead Finder API
  slug: enrich-so-lead-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-lead-finder-api-openapi.yml
- filename: enrich-so-phone-finder-api-openapi.yml
  format: yaml
  label: Enrich Phone Finder API
  slug: enrich-so-phone-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-phone-finder-api-openapi.yml
- filename: enrich-so-teams-api-openapi.yml
  format: yaml
  label: Enrich Teams API
  slug: enrich-so-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-teams-api-openapi.yml
- filename: enrich-so-people-search-api-openapi.yml
  format: yaml
  label: Enrich People Search API
  slug: enrich-so-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-people-search-api-openapi.yml
- filename: enrich-so-authentication-api-openapi.yml
  format: yaml
  label: Enrich Authentication API
  slug: enrich-so-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-authentication-api-openapi.yml
- filename: enrich-so-company-followers-api-openapi.yml
  format: yaml
  label: Enrich Company Followers API
  slug: enrich-so-company-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-company-followers-api-openapi.yml
- filename: enrich-so-company-followers-count-estimation-api-openapi.yml
  format: yaml
  label: Enrich Company Followers/Count Estimation API
  slug: enrich-so-company-followers-count-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-company-followers-count-estimation-api-openapi.yml
- filename: enrich-so-email-validation-api-openapi.yml
  format: yaml
  label: Enrich Email Validation API
  slug: enrich-so-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-email-validation-api-openapi.yml
- filename: enrich-so-enrich-api-openapi.yml
  format: yaml
  label: Enrich Enrich API
  slug: enrich-so-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-enrich-api-openapi.yml
- filename: enrich-so-ip-to-company-api-openapi.yml
  format: yaml
  label: Enrich IP to Company API
  slug: enrich-so-ip-to-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-ip-to-company-api-openapi.yml
- filename: enrich-so-reverse-email-lookup-api-openapi.yml
  format: yaml
  label: Enrich Reverse Email Lookup API
  slug: enrich-so-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-reverse-email-lookup-api-openapi.yml
- filename: enrich-so-wallets-api-openapi.yml
  format: yaml
  label: Enrich Wallets API
  slug: enrich-so-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-wallets-api-openapi.yml
- filename: enrich-so-account-api-openapi.yml
  format: yaml
  label: Enrich Account API
  slug: enrich-so-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-account-api-openapi.yml
- filename: enrich-so-company-intelligence-api-openapi.yml
  format: yaml
  label: Enrich Company Intelligence API
  slug: enrich-so-company-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-company-intelligence-api-openapi.yml
- filename: enrich-so-email-verification-api-openapi.yml
  format: yaml
  label: Enrich Email Verification API
  slug: enrich-so-email-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-email-verification-api-openapi.yml
- filename: enrich-so-person-enrichment-api-openapi.yml
  format: yaml
  label: Enrich Person Enrichment API
  slug: enrich-so-person-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-person-enrichment-api-openapi.yml
- filename: enrich-so-webhooks-api-openapi.yml
  format: yaml
  label: Enrich Webhooks API
  slug: enrich-so-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/openapi/enrich-so-webhooks-api-openapi.yml
authorization_urls: []
description: 'Enrich exposes OAuth 2.0 on exactly one surface — its remote MCP server at mcp.enrich.so — and that server advertises a single scope. The REST API v3 has no OAuth at all: it authenticates with a static organization-scoped API key (sk_ prefix) passed in x-api-key or as a Bearer token, with no scope, permission or capability model of any kind. derive-oauth-scopes.py found 0 oauth2 securitySchemes in the OpenAPI, which is correct rather than a miss; the scope below was read off the live authorization-server metadata instead.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Enrich So Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Enrich uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Enrich
provider_slug: enrich-so
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: enrich-so-scopes
source_filename: enrich-so-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.enrich.so/.well-known/oauth-authorization-server\nprovider: Enrich\nproviderId: enrich-so\ndescription: >-\n  Enrich exposes OAuth 2.0 on exactly one surface — its remote MCP server at\n  mcp.enrich.so — and that server advertises a single scope. The REST API v3 has no OAuth\n  at all: it authenticates with a static organization-scoped API key (sk_ prefix) passed\n  in x-api-key or as a Bearer token, with no scope, permission or capability model of any\n  kind. derive-oauth-scopes.py found 0 oauth2 securitySchemes in the OpenAPI, which is\n  correct rather than a miss; the scope below was read off the live authorization-server\n  metadata instead.\nauthorization_servers:\n- issuer: https://mcp.enrich.so/\n  metadata_url: https://mcp.enrich.so/.well-known/oauth-authorization-server\n  metadata_file: well-known/enrich-so-mcp-oauth-authorization-server.json\n  probed: '2026-08-14'\n  http_status: 200\n  authorization_endpoint:\
  \ https://mcp.enrich.so/authorize\n  token_endpoint: https://mcp.enrich.so/token\n  revocation_endpoint: https://mcp.enrich.so/revoke\n  registration_endpoint: https://mcp.enrich.so/register\n  grant_types:\n  - authorization_code\n  - refresh_token\n  pkce: S256\n  applies_to: MCP (https://mcp.enrich.so/mcp)\nscopes:\n- name: mcp:tools\n  server: https://mcp.enrich.so/\n  description: >-\n    The only scope Enrich advertises. Grants an MCP client access to the server's tools.\n    Enrich publishes no description for it and no finer-grained scopes.\n  documented: false\n  granularity: coarse\nanalysis:\n  scope_count: 1\n  read_write_split: false\n  per_product_scopes: false\n  note: >-\n    One scope for everything is all-or-nothing consent. A user authorizing an agent\n    against Enrich's MCP server cannot grant email validation (1 credit per call) without\n    also granting phone lookup (500 credits per call) and lead reveal (up to 575 credits\n    per lead). Given the API is metered\
  \ against a prepaid balance, coarse scope\n    granularity is a direct financial exposure, not just a privacy one.\nrest_api:\n  oauth: false\n  scopes: false\n  permission_model: >-\n    API keys are scoped to an organization and carry \"member-level permissions\"\n    (https://doc.enrich.so/authentication-1951026m0). Enrich does not publish what those\n    permissions are, does not offer per-key scoping, and the Teams endpoints note that\n    invitation management requires an admin or owner role — so a role model exists inside\n    the product but is not expressible on an API key.\n  recommendation: >-\n    Issue a separate key per workload so credit consumption maps to a cost centre; that\n    is the only isolation mechanism available.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enrich-so/refs/heads/main/scopes/enrich-so-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Data Enrichment
- Contact Discovery
- Web Intelligence
- B2B Data
- Lead Enrichment
- Email Finder
- Email Verification
- Phone Numbers
- People Search
- IP Intelligence
- LinkedIn
- Reference Data
- MCP
token_urls: []
---
