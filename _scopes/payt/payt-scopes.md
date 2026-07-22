---
api_specs:
- filename: payt-openapi-original.json
  format: json
  label: Payt Customer API v1
  slug: payt-customer-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payt/refs/heads/main/openapi/payt-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.paytsoftware.com/authentication/permissions
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Payt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Payt uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Payt
provider_slug: payt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: payt-scopes
source_filename: payt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.paytsoftware.com/authentication/permissions\ndocs: https://docs.paytsoftware.com/authentication/permissions\nmodel:\n  standard: oauth2\n  naming: '<resource>:<action>'\n  actions:\n  - read\n  - write\n  delimiter: space\n  notes: >-\n    Payt permissions are implemented as OAuth 2.0 scopes (RFC 6749 section 3.3);\n    the words \"permission\" and \"scope\" are used interchangeably. Scopes are\n    requested via the scope parameter on the authorize URL (space-separated) and\n    the granted set is returned on every token create and on token introspection.\n    Acting on a resource without its scope returns 403 with a body naming the\n    missing permission, e.g. {\"code\":\"forbidden\",\"message\":\"Missing permission:\n    invoices:write\"}. The full, current list of scopes is published only on the\n    application create/edit form inside the Payt UI (Connections page), not in the\n    public docs, so the list\
  \ below captures the scopes explicitly evidenced in the\n    documentation plus the resource families exposed by the API.\nconfirmed_scopes:\n- scope: debtors:read\n  evidence: authorize-URL example and webhook payload scoping note\n- scope: invoices:read\n  evidence: authorize-URL / token-response example (scope \"invoices:read debtors:read\")\n- scope: invoices:write\n  evidence: '403 error example (Missing permission: invoices:write)'\nresource_families:\n  note: >-\n    Each API resource family below is a candidate scope prefix under the\n    <resource>:read / <resource>:write model. Only the three scopes in\n    confirmed_scopes are documented verbatim; the rest are inferred from the API\n    surface and MUST be confirmed against the in-app application form before use.\n  prefixes:\n  - administrations\n  - companies\n  - contacts\n  - credit_cases\n  - debtors\n  - files\n  - invoices\n  - messages\n  - notes\n  - notifications\n  - order_lines\n  - orders\n  - payment_conditions\n\
  \  - payment_plans\n  - payments\n  - psp_mandates\n  - psp_transactions\n  - tasks\n  - vat_rates\nlifecycle:\n  add: >-\n    Adding a scope to an application does not retroactively grant it; users must\n    re-authorize to grant newly requested scopes.\n  remove: >-\n    Removing a scope immediately invalidates it across all existing tokens; those\n    endpoints then return 403 even for previously valid tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payt/refs/heads/main/scopes/payt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Applicative SaaS
- Accounts Receivable
- Order to Cash
- Invoicing
- Debt Collection
- Payments
- Fintech
- Credit Management
- Netherlands
token_urls: []
---
