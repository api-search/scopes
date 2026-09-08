---
api_specs:
- filename: dealogic-analytics-spac-v2-openapi.json
  format: json
  label: Dealogic Analytics SPAC API
  slug: dealogic-analytics-spac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-spac-v2-openapi.json
- filename: dealogic-analytics-bank-openapi.json
  format: json
  label: Dealogic Analytics Bank API
  slug: dealogic-analytics-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-bank-openapi.json
- filename: dealogic-analytics-company-openapi.json
  format: json
  label: Dealogic Analytics Company API
  slug: dealogic-analytics-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-company-openapi.json
- filename: dealogic-analytics-sponsor-openapi.json
  format: json
  label: Dealogic Analytics Sponsor API
  slug: dealogic-analytics-sponsor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-analytics-sponsor-openapi.json
- filename: dealogic-reporting-openapi.json
  format: json
  label: Dealogic Reporting API
  slug: dealogic-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-reporting-openapi.json
- filename: dealogic-cortex-reporting-openapi.json
  format: json
  label: Cortex Reporting API
  slug: cortex-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-cortex-reporting-openapi.json
- filename: dealogic-iona-profiles-openapi.json
  format: json
  label: IONA Profiles API
  slug: iona-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/openapi/dealogic-iona-profiles-openapi.json
authorization_urls: []
description: ''
docs: https://iongroup.com/analytics/data-portal/apis-data-feeds/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Dealogic Scopes
name_suffix: OAuth Scopes
note: Every harvested spec declares oauth2 with an EMPTY scopes map, so nothing is derivable from the contracts. The scopes below are the authorization server's own scopes_supported list, read from the OIDC discovery document. Dealogic publishes no per-product scope reference page; entitlement to a given dataset is granted on the licence, not by a scope string.
overview: 'Dealogic publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dealogic API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dealogic
provider_slug: dealogic
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- dealogic
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope; requests the end user's basic profile claims.
  flows: []
  scope: profile
- description: Standard OpenID Connect scope; requests the end user's email claim.
  flows: []
  scope: email
- description: Dealogic's single product scope. It is the only non-standard scope the authorization server advertises; the Dealogic APIs do not decompose access into per-resource or read/write scopes.
  flows: []
  scope: dealogic
slug: dealogic-scopes
source_filename: dealogic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://login.dealogic.com/.well-known/openid-configuration (HTTP 200, fetched 2026-09-05); baseline\n  derived by derive-oauth-scopes.py from the eight harvested OpenAPI documents\ndocs: https://iongroup.com/analytics/data-portal/apis-data-feeds/\nauthorization_server:\n  issuer: https://login.dealogic.com\n  authorization_endpoint: https://login.dealogic.com/as/authorization.oauth2\n  token_endpoint: https://login.dealogic.com/as/token.oauth2\nnote: Every harvested spec declares oauth2 with an EMPTY scopes map, so nothing is derivable from the\n  contracts. The scopes below are the authorization server's own scopes_supported list, read from the\n  OIDC discovery document. Dealogic publishes no per-product scope reference page; entitlement to a given\n  dataset is granted on the licence, not by a scope string.\nscope_count: 4\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; requests an ID token.\n \
  \ source: oidc-discovery\n- scope: profile\n  description: Standard OpenID Connect scope; requests the end user's basic profile claims.\n  source: oidc-discovery\n- scope: email\n  description: Standard OpenID Connect scope; requests the end user's email claim.\n  source: oidc-discovery\n- scope: dealogic\n  description: Dealogic's single product scope. It is the only non-standard scope the authorization server\n    advertises; the Dealogic APIs do not decompose access into per-resource or read/write scopes.\n  source: oidc-discovery\nclaims_supported:\n- idp\n- sub\ngranularity:\n  verdict: coarse\n  detail: One product scope for the whole Dealogic API estate. An agent cannot request read-only access,\n    nor access to one dataset (SPAC, Bank, Company, Sponsor, Reporting) without the rest; separation is\n    enforced by licence entitlement server-side, not by the token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/scopes/dealogic-scopes.yml
summary_line: 4 scopes
tags:
- Analytics
- Capital Markets
- Compliance
- Deal Management
- Debt Capital Markets
- Equity Capital Markets
- Finance
- Financial Data
- Investment Banking
- League Tables
- M&A
- OData
- Private Equity
- Reporting
- SPAC
- Syndicated Loans
token_urls: []
---
