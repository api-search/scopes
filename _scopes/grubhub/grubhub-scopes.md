---
api_specs:
- filename: grubhub-menu-openapi.yml
  format: yaml
  label: Grubhub Menu API
  slug: grubhub-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-menu-openapi.yml
- filename: grubhub-orders-openapi.yml
  format: yaml
  label: Grubhub Orders API
  slug: grubhub-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-orders-openapi.yml
- filename: grubhub-merchant-data-openapi.yml
  format: yaml
  label: Grubhub Merchant Data API
  slug: grubhub-merchant-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-data-openapi.yml
- filename: grubhub-merchant-schedules-openapi.yml
  format: yaml
  label: Grubhub Merchant Schedules API
  slug: grubhub-merchant-schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-merchant-schedules-openapi.yml
- filename: grubhub-busy-intervals-openapi.yml
  format: yaml
  label: Grubhub Busy Intervals API
  slug: grubhub-busy-intervals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-busy-intervals-openapi.yml
- filename: grubhub-deliveries-openapi.yml
  format: yaml
  label: Grubhub Deliveries API
  slug: grubhub-deliveries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-deliveries-openapi.yml
- filename: grubhub-connect-endpoints-openapi.yml
  format: yaml
  label: Grubhub Connect (Delivery as a Service) API
  slug: grubhub-connect-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-endpoints-openapi.yml
- filename: grubhub-connect-webhooks-openapi.yml
  format: yaml
  label: Grubhub Connect Webhooks
  slug: grubhub-connect-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-connect-webhooks-openapi.yml
- filename: grubhub-onboarding-openapi.yml
  format: yaml
  label: Grubhub Onboarding API
  slug: grubhub-onboarding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-onboarding-openapi.yml
- filename: grubhub-reporting-endpoints-openapi.yml
  format: yaml
  label: Grubhub Merchant Reporting API
  slug: grubhub-reporting-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-endpoints-openapi.yml
- filename: grubhub-reporting-webhooks-openapi.yml
  format: yaml
  label: Grubhub Reporting Webhooks
  slug: grubhub-reporting-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-reporting-webhooks-openapi.yml
- filename: grubhub-testing-openapi.yml
  format: yaml
  label: Grubhub Testing API
  slug: grubhub-testing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-testing-openapi.yml
authorization_urls: []
description: ''
docs: https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Grubhub Scopes
name_suffix: OAuth Scopes
note: Upgraded 2026-09-17 from searched to probed. The scope list is no longer inferred from a docs article - it is read directly from Grubhub's own RFC 8414 authorization-server metadata, which both partner API hosts serve anonymously. scopes_supported is exactly ["openid", "diner"]. None of the twelve published partner OpenAPI documents declares an oauth2 securityScheme, so no scope is bound to an operation anywhere in the machine-readable contract.
overview: 'Grubhub publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Grubhub API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Grubhub
provider_slug: grubhub
schemes: []
scope_count: 2
scope_names:
- openid
- diner
scopes:
- description: OpenID Connect base scope. Advertised in scopes_supported by the production and preproduction authorization servers.
  flows: []
  scope: openid
- description: Grants a partner application an access token bound to a Grubhub diner record, for diner-facing ordering integrations. Advertised in scopes_supported by the production and preproduction authorization servers.
  flows: []
  scope: diner
slug: grubhub-scopes
source_filename: grubhub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server\ndocs: https://grubhub-developers.zendesk.com/hc/en-us/articles/115004598023-Open-ID-Authentication\nnote: >-\n  Upgraded 2026-09-17 from searched to probed. The scope list is no longer inferred from a docs\n  article - it is read directly from Grubhub's own RFC 8414 authorization-server metadata, which\n  both partner API hosts serve anonymously. scopes_supported is exactly [\"openid\", \"diner\"].\n  None of the twelve published partner OpenAPI documents declares an oauth2 securityScheme, so\n  no scope is bound to an operation anywhere in the machine-readable contract.\ndiscovery:\n  url: https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server\n  status: 200\n  fetched: '2026-09-17'\n  file: well-known/grubhub-oauth-authorization-server.json\nissuer: https://api-gtm.grubhub.com\nauthorization_endpoint: https://api-gtm.grubhub.com/oauth2/authorize\n\
  token_endpoint: https://api-gtm.grubhub.com/oauth2/token\nregistration_endpoint: https://api-gtm.grubhub.com/oauth/register\nscope_count: 2\nscopes:\n- scope: openid\n  description: >-\n    OpenID Connect base scope. Advertised in scopes_supported by the production and preproduction\n    authorization servers.\n  sources:\n  - https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server\n- scope: diner\n  description: >-\n    Grants a partner application an access token bound to a Grubhub diner record, for diner-facing\n    ordering integrations. Advertised in scopes_supported by the production and preproduction\n    authorization servers.\n  sources:\n  - https://api-third-party-gtm.grubhub.com/.well-known/oauth-authorization-server\ngaps:\n- No scope is referenced by any operation in any published OpenAPI document (no securitySchemes at all).\n- Partner-side integration (Menu, Orders, Merchant Data, Schedules, Connect, Reporting) authenticates\n  with the X-GH-PARTNER-KEY\
  \ header rather than a scoped OAuth token; those surfaces have no scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/scopes/grubhub-scopes.yml
summary_line: 2 scopes
tags:
- Food Delivery
- Restaurant
- Marketplace
- Online Ordering
- Point-of-Sale
- Logistics
- Last Mile Delivery
- Menu Management
- Hospitality
- Local Commerce
token_urls: []
---
