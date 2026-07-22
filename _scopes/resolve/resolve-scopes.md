---
api_specs:
- filename: resolve-merchant-api-openapi.yaml
  format: yaml
  label: Resolve Merchant API
  slug: resolve-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-merchant-api-openapi.yaml
- filename: resolve-partners-api-openapi.yaml
  format: yaml
  label: Resolve Partners API
  slug: resolve-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/openapi/resolve-partners-api-openapi.yaml
authorization_urls: []
description: ''
docs: https://docs.resolvepay.com/guides/direct-api-access-and-authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Resolve Scopes
name_suffix: OAuth Scopes
note: The OpenAPI models auth as HTTP basic + bearer (JWT), but Resolve's OAuth access keys (M2M) carry coarse-grained scopes documented in the auth guide and the MCP tool reference. Read tools require merchant:read; write tools require merchant:write.
overview: 'Resolve publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Resolve API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Resolve
provider_slug: resolve
schemes:
- description: OAuth access keys created in Merchant Dashboard, exchanged for a JWT bearer token.
  name: bearerAuth
  source: openapi/resolve-merchant-api-openapi.yaml
  token_url: https://app.resolvepay.com/api/access-keys/token
  type: oauth-access-key
scope_count: 2
scope_names:
- merchant:read
- merchant:write
scopes:
- description: Read-only access to merchant resources (list/fetch customers, invoices, orders, charges, shipments, payments, payouts).
  flows:
  - clientCredentials
  scope: merchant:read
- description: Write access to merchant resources (create/update/send/capture/void/cancel invoices, customers, orders, charges, shipments, credit checks, enrollment).
  flows:
  - clientCredentials
  scope: merchant:write
slug: resolve-scopes
source_filename: resolve-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/resolve-merchant-api-openapi.yaml\ndocs: https://docs.resolvepay.com/guides/direct-api-access-and-authentication\nnote: >-\n  The OpenAPI models auth as HTTP basic + bearer (JWT), but Resolve's OAuth\n  access keys (M2M) carry coarse-grained scopes documented in the auth guide and\n  the MCP tool reference. Read tools require merchant:read; write tools require\n  merchant:write.\nschemes:\n  - name: bearerAuth\n    source: openapi/resolve-merchant-api-openapi.yaml\n    type: oauth-access-key\n    token_url: https://app.resolvepay.com/api/access-keys/token\n    description: OAuth access keys created in Merchant Dashboard, exchanged for a JWT bearer token.\nscopes:\n  - scope: merchant:read\n    description: Read-only access to merchant resources (list/fetch customers, invoices, orders, charges, shipments, payments, payouts).\n    flows: [clientCredentials]\n    sources: [https://docs.resolvepay.com/guides/mcp-tools]\n\
  \  - scope: merchant:write\n    description: Write access to merchant resources (create/update/send/capture/void/cancel invoices, customers, orders, charges, shipments, credit checks, enrollment).\n    flows: [clientCredentials]\n    sources: [https://docs.resolvepay.com/guides/mcp-tools]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resolve/refs/heads/main/scopes/resolve-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Payments
- B2B
- Net Terms
- Credit
- Invoicing
- Financing
- Embedded Finance
token_urls: []
---
