---
api_specs:
- filename: scanverity-resolution-api-openapi.json
  format: json
  label: Scanverity Resolution API
  slug: scanverity-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scanverity-resolution-api/refs/heads/main/openapi/scanverity-resolution-api-openapi.json
authorization_urls: []
description: 'Four named, deny-by-default scopes bound to the opaque bearer token at issue time. IMPORTANT -- this is NOT OAuth 2.0: the API declares a single http/bearer security scheme, there is no authorization server, no /token endpoint, no consent screen and no scope negotiation. The scopes are recorded here because they are real, documented and gate individual operations; the canonical OAuthScopes pointer is used because it is the catalog''s scope-reference type, not because an OAuth flow exists.'
docs: https://scanverity.com/resolution-api/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Scanverity Resolution Api Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Scanverity Resolution API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Scanverity Resolution API
provider_slug: scanverity-resolution-api
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: scanverity-resolution-api-scopes
source_filename: scanverity-resolution-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://scanverity.com/resolution-api/docs\nderived_from: openapi/scanverity-resolution-api-openapi.json\nname: Scanverity Resolution API scopes\ndescription: >-\n  Four named, deny-by-default scopes bound to the opaque bearer token at issue time. IMPORTANT --\n  this is NOT OAuth 2.0: the API declares a single http/bearer security scheme, there is no\n  authorization server, no /token endpoint, no consent screen and no scope negotiation. The scopes\n  are recorded here because they are real, documented and gate individual operations; the canonical\n  OAuthScopes pointer is used because it is the catalog's scope-reference type, not because an OAuth\n  flow exists.\ndocs: https://scanverity.com/resolution-api/docs\nmodel: token-bound\ndefault: deny\nauthorization_server: null\nscope_count: 4\nscopes:\n  - name: resolution:request\n    description: Authorizes creation of new resolution assessments. This is the only billable scope.\n\
  \    operations:\n      - createResolutionAssessment\n  - name: resolution:read\n    description: Authorizes reading and polling an existing account-scoped assessment. Never billable.\n    operations:\n      - getResolutionAssessment\n  - name: usage:read\n    description: >-\n      Authorizes only the live reconciled-usage routes. A sandbox token carrying this scope is still\n      refused; the docs state a live token is required.\n    operations:\n      - getResolutionUsageSummary\n      - listResolutionUsageEvents\n  - name: webhooks:manage\n    description: >-\n      Authorizes only the webhook endpoint registry and the append-only delivery-evidence\n      operations, including manual redelivery.\n    operations:\n      - createResolutionWebhookEndpoint\n      - listResolutionWebhookEndpoints\n      - deleteResolutionWebhookEndpoint\n      - listResolutionWebhookDeliveries\n      - redeliverResolutionWebhook\nenforcement:\n  insufficient_scope_status: 403\n  insufficient_scope_code:\
  \ INSUFFICIENT_SCOPE\n  note: >-\n    The 403 body carries a detail string naming the missing scope, e.g. \"This token lacks the\n    'resolution:request' scope.\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scanverity-resolution-api/refs/heads/main/scopes/scanverity-resolution-api-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Prediction Markets
- Resolution Risk
- Market Intelligence
- Due Diligence
- Webhooks
- OpenAPI
- Fintech
- Risk Analytics
- Polymarket
- Event Contracts
- Agent Ready
token_urls: []
---
