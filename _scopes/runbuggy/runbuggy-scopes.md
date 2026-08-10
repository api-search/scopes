---
api_specs:
- filename: runbuggy-companies-api-openapi.yml
  format: yaml
  label: RunBuggy Companies API
  slug: runbuggy-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-companies-api-openapi.yml
- filename: runbuggy-orders-api-openapi.yml
  format: yaml
  label: RunBuggy Orders API
  slug: runbuggy-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-orders-api-openapi.yml
- filename: runbuggy-token-api-openapi.yml
  format: yaml
  label: RunBuggy Token API
  slug: runbuggy-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-token-api-openapi.yml
- filename: runbuggy-vehicle-transfer-orders-api-openapi.yml
  format: yaml
  label: RunBuggy Vehicle Transfer Orders API
  slug: runbuggy-vehicle-transfer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-vehicle-transfer-orders-api-openapi.yml
- filename: runbuggy-webhooks-api-openapi.yml
  format: yaml
  label: RunBuggy Webhooks API
  slug: runbuggy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Runbuggy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RunBuggy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RunBuggy
provider_slug: runbuggy
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: runbuggy-scopes
source_filename: runbuggy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: well-known/runbuggy-oauth-authorization-server.json, https://docs.runbuggy.com/docs/shipping/d483faef38c3b-embedding-i-frame-order-status\nsummary: 'RunBuggy has almost no scope surface. The REST Shippers API is bearer-token\n  authenticated with no scopes at all — permission is a property of the token holder''s\n  company, not of the request. Exactly one scope value is published anywhere in the\n  estate, and the OAuth authorization server that fronts the MCP layer publishes none.'\nmodel: opaque-bearer-token-no-scopes\nrest_api:\n  scopes_supported: []\n  detail: 'securityDefinitions on all three Swagger 2.0 documents is a single\n    `apiKey in header` named Authorization. No oauth2 flow, no scopes object, and no\n    per-operation security requirement differentiation — every operation carries the\n    same blanket requirement.'\n  authorization_model: 'Authority is company-scoped and relationship-granted. A company\n  \
  \  can act for another company only after RunBuggy establishes that authorization\n    out-of-band (\"Your Runbuggy support contact can work with you to establish this\n    authorization\"), and the caller then discovers it via the Companies API.'\n  docs: https://docs.runbuggy.com/docs/shipping/94fced2e96c5f-placing-an-order-for-another-company\nscopes:\n- name: openid\n  used_by: embeddable order-status iframe token exchange\n  description: The only scope value published by RunBuggy. Requested in the body of the\n    platform oauth2/token call to mint the short-lived JWT that authorizes an\n    unauthenticated buyer or seller to view a single order's status in an iframe.\n  grants: read access to one order's status for the token lifetime (documented as 60\n    seconds)\n  source: https://docs.runbuggy.com/docs/shipping/d483faef38c3b-embedding-i-frame-order-status\nmcp_authorization_server:\n  issuer: https://apps.runbuggy.com/runbuggy/mcp-datascience\n  metadata: well-known/runbuggy-oauth-authorization-server.json\n\
  \  scopes_supported: null\n  detail: The RFC 8414 metadata document omits `scopes_supported` entirely. An MCP\n    client performing dynamic client registration has no published vocabulary to request\n    against, and the protected-resource metadata that would normally carry it is not\n    served.\ngaps:\n- No scope or permission reference page exists on docs.runbuggy.com.\n- The REST API has no scopes, so a bearer token is all-or-nothing across all 28\n  operations — including order creation and cancellation.\n- The MCP authorization server advertises no scopes_supported.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - url: https://apps.runbuggy.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://docs.runbuggy.com/docs/shipping/d483faef38c3b-embedding-i-frame-order-status\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/scopes/runbuggy-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Automotive
- Logistics
- Transportation
- Vehicle Shipping
- Marketplace
- Supply Chain
- Fleet
- TMS
- Freight
token_urls: []
---
