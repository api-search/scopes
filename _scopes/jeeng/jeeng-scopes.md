---
api_specs:
- filename: jeeng-advertisers-openapi.yml
  format: yaml
  label: Jeeng Email Monetization — Advertisers API
  slug: jeeng-email-monetization-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-advertisers-openapi.yml
- filename: jeeng-publishers-openapi.yml
  format: yaml
  label: Jeeng Email Monetization — Publishers API
  slug: jeeng-email-monetization-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-publishers-openapi.yml
- filename: jeeng-authentication-openapi.yml
  format: yaml
  label: Jeeng Email Monetization — Authentication
  slug: jeeng-email-monetization-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/openapi/jeeng-authentication-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.jeeng.com/reference/getting-an-access-token
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Jeeng Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jeeng publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jeeng API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jeeng
provider_slug: jeeng
schemes: []
scope_count: 1
scope_names:
- api://revenuestripe.onmicrosoft.com/partners/.default
scopes:
- description: The single partner scope for the Jeeng / OpenWeb Email Monetization APIs. Grants the permissions for all partner API endpoints — advertiser and publisher reporting, campaigns, creatives, and the performance reports.
  flows: []
  scope: api://revenuestripe.onmicrosoft.com/partners/.default
slug: jeeng-scopes
source_filename: jeeng-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developers.jeeng.com/reference/getting-an-access-token\ndocs: https://developers.jeeng.com/reference/getting-an-access-token\nidentity_provider: Microsoft Entra ID (Azure AD)\ntenant: revenuestripe.onmicrosoft.com\ntoken_url: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/oauth2/v2.0/token\nflow: client_credentials\nscheme: sec0\nscopes:\n- scope: api://revenuestripe.onmicrosoft.com/partners/.default\n  description: The single partner scope for the Jeeng / OpenWeb Email Monetization APIs. Grants the\n    permissions for all partner API endpoints — advertiser and publisher reporting, campaigns,\n    creatives, and the performance reports.\n  applies_to:\n  - openapi/jeeng-advertisers-openapi.yml\n  - openapi/jeeng-publishers-openapi.yml\n  required: true\n  source: https://developers.jeeng.com/reference/getting-an-access-token\nscope_count: 1\ngranularity: coarse\nnotes:\n- Jeeng publishes exactly one\
  \ scope. It is an Entra ID `.default` application scope, so consent is\n  granted at the application-registration level rather than per-endpoint; there is no read-only vs\n  write split, and no separate advertiser vs publisher scope.\n- 'Requesting any other scope is documented as the most common cause of an HTTP 401 with the message\n  \"Not authorized to this endpoint.\" Because a token issued for the wrong scope can still succeed on\n  some endpoints, the failure typically appears only on the performance report endpoints.'\n- >-\n  The OpenAPI `securitySchemes.sec0` object published for both APIs declares `type: oauth2` with an\n  empty `flows` object and therefore carries no machine-readable scope list; the scope above comes\n  from the provider's own authentication reference page.\nx-evidence:\n- url: https://developers.jeeng.com/reference/getting-an-access-token.md\n  http_status: 200\n  fetched: '2026-08-12'\n- url: https://login.microsoftonline.com/revenuestripe.onmicrosoft.com/v2.0/.well-known/openid-configuration\n\
  \  http_status: 200\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeeng/refs/heads/main/scopes/jeeng-scopes.yml
summary_line: 1 scope
tags:
- Company
- Advertising
- Publishing
- Email
- Push Notifications
- Monetization
- AdTech
- Newsletters
- Audience Engagement
- Reporting
- Analytics
- OData
- Authentication
token_urls: []
---
