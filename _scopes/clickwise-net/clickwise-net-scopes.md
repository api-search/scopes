---
api_specs:
- filename: clickwise-net-account-api-openapi.yml
  format: yaml
  label: Clickwise Account API
  slug: clickwise-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-account-api-openapi.yml
- filename: clickwise-net-deals-api-openapi.yml
  format: yaml
  label: Clickwise Deals API
  slug: clickwise-net-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-deals-api-openapi.yml
- filename: clickwise-net-feeds-api-openapi.yml
  format: yaml
  label: Clickwise Feeds API
  slug: clickwise-net-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-feeds-api-openapi.yml
- filename: clickwise-net-links-api-openapi.yml
  format: yaml
  label: Clickwise Links API
  slug: clickwise-net-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-links-api-openapi.yml
- filename: clickwise-net-monetize-api-openapi.yml
  format: yaml
  label: Clickwise Monetize API
  slug: clickwise-net-monetize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-monetize-api-openapi.yml
- filename: clickwise-net-news-api-openapi.yml
  format: yaml
  label: Clickwise News API
  slug: clickwise-net-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-news-api-openapi.yml
- filename: clickwise-net-offers-api-openapi.yml
  format: yaml
  label: Clickwise Offers API
  slug: clickwise-net-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-offers-api-openapi.yml
- filename: clickwise-net-onboarding-api-openapi.yml
  format: yaml
  label: Clickwise Onboarding API
  slug: clickwise-net-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-onboarding-api-openapi.yml
- filename: clickwise-net-postbacks-api-openapi.yml
  format: yaml
  label: Clickwise Postbacks API
  slug: clickwise-net-postbacks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-postbacks-api-openapi.yml
- filename: clickwise-net-products-api-openapi.yml
  format: yaml
  label: Clickwise Products API
  slug: clickwise-net-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-products-api-openapi.yml
- filename: clickwise-net-programs-api-openapi.yml
  format: yaml
  label: Clickwise Programs API
  slug: clickwise-net-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-programs-api-openapi.yml
- filename: clickwise-net-public-api-openapi.yml
  format: yaml
  label: Clickwise Public API
  slug: clickwise-net-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-public-api-openapi.yml
- filename: clickwise-net-reporting-api-openapi.yml
  format: yaml
  label: Clickwise Reporting API
  slug: clickwise-net-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-reporting-api-openapi.yml
- filename: clickwise-net-subscribers-api-openapi.yml
  format: yaml
  label: Clickwise Subscribers API
  slug: clickwise-net-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-subscribers-api-openapi.yml
- filename: clickwise-net-widgets-api-openapi.yml
  format: yaml
  label: Clickwise Widgets API
  slug: clickwise-net-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clickwise-net/openapi/clickwise-net-widgets-api-openapi.yml
authorization_urls: []
description: ''
docs: https://partners.clickwise.net/llms-full.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clickwise Scopes
name_suffix: OAuth Scopes
note: Access tokens 1 h, rotating refresh tokens 30 days; revoke at https://partners.clickwise.net/oauth/connections/. get_product_feed needs an API key.
overview: 'Clickwise publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clickwise API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clickwise
provider_slug: clickwise-net
schemes: []
scope_count: 2
scope_names:
- affiliate:read
- affiliate:links
scopes:
- description: programs, reports, conversions
  flows: []
  scope: affiliate:read
- description: tracked links and product search
  flows: []
  scope: affiliate:links
slug: clickwise-net-scopes
source_filename: clickwise-net-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://partners.clickwise.net/llms-full.txt\ndocs: https://partners.clickwise.net/llms-full.txt\napplies_to: MCP account endpoint https://partners.clickwise.net/api/v1/mcp/account (OAuth 2.1); the REST OpenAPI declares no oauth2 scheme\nscopes:\n- name: affiliate:read\n  description: programs, reports, conversions\n- name: affiliate:links\n  description: tracked links and product search\nnote: Access tokens 1 h, rotating refresh tokens 30 days; revoke at https://partners.clickwise.net/oauth/connections/. get_product_feed needs an API key.\n"
source_yaml_url: https://artifacts.apis.io/clickwise-net/scopes/clickwise-net-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Affiliate Marketing
- Affiliate Network
- Performance Marketing
- tracked-links
- Publishers
- E-Commerce
- MCP
token_bound: false
token_urls: []
---
