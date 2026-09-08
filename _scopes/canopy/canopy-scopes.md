---
api_specs:
- filename: canopy-openapi.json
  format: json
  label: Canopy Connect API
  slug: canopy-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/openapi/canopy-openapi.json
authorization_urls: []
description: ''
docs: https://docs.usecanopy.com/reference/apps-api-requests
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Canopy Scopes
name_suffix: OAuth Scopes
note: These scopes govern Canopy Connect Apps - third-party integrations acting on another Team's behalf with a Bearer access token. They do NOT apply to HTTP Basic calls against your own Team, which are unscoped. The scopes are documented only on the Apps "Making API Requests" page; the published OpenAPI declares no oauth2 securityScheme at all, so no operation in the spec carries a scope requirement. The operation mapping below is transcribed from the provider's own scope table and joined to operationIds in openapi/canopy-openapi.json.
overview: 'Canopy Connect uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canopy Connect
provider_slug: canopy
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: canopy-scopes
source_filename: canopy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://docs.usecanopy.com/reference/apps-api-requests#scopes\ndocs: https://docs.usecanopy.com/reference/apps-api-requests\nprovider: Canopy Connect\nproviderId: canopy\nflow: authorizationCode\npkce: required\nauthorization_url: https://app.usecanopy.com/oauth2/authorize\nnote: >-\n  These scopes govern Canopy Connect Apps - third-party integrations acting on\n  another Team's behalf with a Bearer access token. They do NOT apply to HTTP\n  Basic calls against your own Team, which are unscoped. The scopes are\n  documented only on the Apps \"Making API Requests\" page; the published OpenAPI\n  declares no oauth2 securityScheme at all, so no operation in the spec carries\n  a scope requirement. The operation mapping below is transcribed from the\n  provider's own scope table and joined to operationIds in\n  openapi/canopy-openapi.json.\nscope_count: 12\nscopes:\n  - name: read:pulls\n    description: Read Pulls, list Pulls,\
  \ and download the documents attached to a Pull.\n    operations:\n      - get-pull-by-id\n      - get-pulls\n      - get-document-by-id\n      - download-document-by-id\n      - post-pull-policy-check\n      - get-pull-policy-check-pdf\n  - name: read:policy_checks\n    description: Read Policy Check settings and evaluate/read Policy Check results.\n    operations:\n      - post-pull-policy-check\n      - get-pull-policy-check-pdf\n      - get-policy-check-team-settings\n  - name: write:policy_checks\n    description: Configure the Team's Policy Check settings and run a Policy Check on a Pull.\n    operations:\n      - post-pull-policy-check\n      - post-policy-check-team-settings\n  - name: read:webhooks\n    description: List webhooks. An App can only see webhooks it created itself.\n    operations:\n      - get-webhooks\n  - name: write:webhooks\n    description: Create, update and delete webhooks. An App can only modify webhooks it created itself.\n    operations:\n      - post-webhooks\n\
  \      - patch-webhook\n      - delete-webhook\n  - name: read:widgets\n    description: List widgets (links) and read a single widget.\n    operations:\n      - get-widgets\n      - get-widgetId\n  - name: write:widgets\n    description: Create, update and delete widgets, and upload a widget logo or icon.\n    operations:\n      - post-widgets\n      - patch-widgetId\n      - delete-widgetId\n      - put-widgetId-logo\n      - put-widgetId-icon\n  - name: read:driver_license_lookup\n    description: Call the driver licence enrichment lookup.\n    operations:\n      - get-enrichment-driverlicense\n  - name: read:driving_record_iq_lookup\n    description: Call the driving-record IQ enrichment lookup.\n    operations:\n      - get-enrichment-drivingrecordiq\n  - name: read:household_lookup\n    description: Call the household enrichment lookup.\n    operations:\n      - get-enrichment-household\n  - name: read:property_lookup\n    description: Call the ad-hoc property data lookup.\n    operations:\n\
  \      - get-property-data\n  - name: write:whitelabel\n    description: >-\n      Drive the white-label flows - collect consent, create and authenticate a\n      Pull, submit MFA/identity verification, mint reconnect tokens, and confirm\n      servicing actions.\n    operations:\n      - post-consent\n      - post-consent-and-connect\n      - post-connect\n      - post-idv\n      - post-idvoptions\n      - post-reconnect-token\n      - post-servicing-action\nuncovered_operations_note: >-\n  The provider's scope table covers 31 of the 54 published operations. The\n  Teams API, Monitorings API, Servicings API (list/create/read), Policy Search\n  API, Policy Forms API, Carriers, /tos, /health and\n  post-consent-and-documents appear in the OpenAPI but not in the Apps scope\n  table, which means they are reachable only with Basic (own-Team) credentials\n  as documented today.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canopy/refs/heads/main/scopes/canopy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Auto Insurance
- Casualty
- Financial-Services
- Homeowners Insurance
- Insurance
- Insurance Verification
- Property
token_urls: []
---
