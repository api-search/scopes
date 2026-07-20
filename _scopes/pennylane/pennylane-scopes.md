---
api_specs:
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customer Invoicing API
  slug: pennylane-customer-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Supplier Invoicing API
  slug: pennylane-supplier-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting & Ledger API
  slug: pennylane-accounting-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Accounting Exports API
  slug: pennylane-accounting-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Banking API
  slug: pennylane-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Customers & Suppliers API
  slug: pennylane-customers-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Products Catalog API
  slug: pennylane-products-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Quotes API
  slug: pennylane-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Billing Subscriptions API
  slug: pennylane-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Direct Debit Mandates API
  slug: pennylane-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane Change Events API
  slug: pennylane-change-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
- filename: pennylane-openapi.yml
  format: yaml
  label: Pennylane E-Invoicing (Plateforme Agréée) API
  slug: pennylane-einvoicing-pa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/openapi/pennylane-openapi.yml
authorization_urls: []
description: ''
docs: https://pennylane.readme.io/docs/oauth-20-walkthrough
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Pennylane Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pennylane publishes 23 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pennylane API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pennylane
provider_slug: pennylane
schemes:
- authorizationUrl: https://app.pennylane.com/oauth/authorize
  flow: authorizationCode
  name: oauth2
  pkce: S256
  registrationUrl: https://app.pennylane.com/oauth/register
  tokenUrl: https://app.pennylane.com/oauth/token
scope_count: 23
scope_names:
- customer_invoices:readonly
- customer_invoices:all
- mcp:account:read
- mcp:changelog:read
- mcp:company:read
- mcp:customer:read
- mcp:customer_invoice:read
- mcp:customer_payment:read
- mcp:financial_report:read
- mcp:firm_file:read
- mcp:journal:read
- mcp:ledger_account:read
- mcp:ledger_entry:read
- mcp:ledger_entry_line:read
- mcp:product:read
- mcp:supplier:read
- mcp:supplier_invoice:read
- mcp:supplier_payment:read
- mcp:tax_return:read
- mcp:transaction:read
- mcp:trial_balance:read
- mcp:vat_return:read
- mcp:private_api
scopes:
- description: Read access to customer invoices.
  flows: []
  scope: customer_invoices:readonly
- description: Full access to customer invoices.
  flows: []
  scope: customer_invoices:all
- description: Read account/company profile via the MCP surface.
  flows: []
  scope: mcp:account:read
- description: ''
  flows: []
  scope: mcp:changelog:read
- description: ''
  flows: []
  scope: mcp:company:read
- description: ''
  flows: []
  scope: mcp:customer:read
- description: ''
  flows: []
  scope: mcp:customer_invoice:read
- description: ''
  flows: []
  scope: mcp:customer_payment:read
- description: ''
  flows: []
  scope: mcp:financial_report:read
- description: ''
  flows: []
  scope: mcp:firm_file:read
- description: ''
  flows: []
  scope: mcp:journal:read
- description: ''
  flows: []
  scope: mcp:ledger_account:read
- description: ''
  flows: []
  scope: mcp:ledger_entry:read
- description: ''
  flows: []
  scope: mcp:ledger_entry_line:read
- description: ''
  flows: []
  scope: mcp:product:read
- description: ''
  flows: []
  scope: mcp:supplier:read
- description: ''
  flows: []
  scope: mcp:supplier_invoice:read
- description: ''
  flows: []
  scope: mcp:supplier_payment:read
- description: ''
  flows: []
  scope: mcp:tax_return:read
- description: ''
  flows: []
  scope: mcp:transaction:read
- description: ''
  flows: []
  scope: mcp:trial_balance:read
- description: ''
  flows: []
  scope: mcp:vat_return:read
- description: Private API access grant on the MCP surface.
  flows: []
  scope: mcp:private_api
slug: pennylane-scopes
source_filename: pennylane-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource:\n- https://app.pennylane.com/.well-known/oauth-authorization-server\n- https://pennylane.readme.io/reference/getcustomerinvoices\ndocs: https://pennylane.readme.io/docs/oauth-20-walkthrough\nnotes: >-\n  Pennylane's OpenAPI declares only a Bearer (http) scheme, but the platform documents\n  OAuth 2.0 for integration partners and enforces least-privilege scopes. Two scope\n  families are in use: (1) the developer/OAuth resource scopes that gate the REST API,\n  following a <resource>:readonly / <resource>:all pattern (403 when a required scope is\n  missing); (2) a set of read-only mcp:* scopes advertised on the OAuth authorization\n  server for Pennylane's Model Context Protocol surface. Scopes marked source\n  well-known were read verbatim from the authorization-server metadata; the resource:all\n  / resource:readonly pattern is documented on the API reference.\nschemes:\n- name: oauth2\n  flow: authorizationCode\n  authorizationUrl:\
  \ https://app.pennylane.com/oauth/authorize\n  tokenUrl: https://app.pennylane.com/oauth/token\n  registrationUrl: https://app.pennylane.com/oauth/register\n  pkce: S256\nscope_pattern:\n  readonly: \"<resource>:readonly — read access to the resource\"\n  all: \"<resource>:all — full (read/write) access to the resource\"\n  example_resources:\n  - customer_invoices\n  - supplier_invoices\n  - ledger_entries\n  - transactions\n  - customers\n  - suppliers\n  - products\n  - quotes\nscopes:\n- scope: customer_invoices:readonly\n  description: Read access to customer invoices.\n  sources: [https://pennylane.readme.io/reference/getcustomerinvoices]\n- scope: customer_invoices:all\n  description: Full access to customer invoices.\n  sources: [https://pennylane.readme.io/reference/getcustomerinvoices]\n- scope: mcp:account:read\n  description: Read account/company profile via the MCP surface.\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:changelog:read\n\
  \  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:company:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:customer:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:customer_invoice:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:customer_payment:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:financial_report:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:firm_file:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:journal:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:ledger_account:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:ledger_entry:read\n  sources:\
  \ [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:ledger_entry_line:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:product:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:supplier:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:supplier_invoice:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:supplier_payment:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:tax_return:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:transaction:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:trial_balance:read\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:vat_return:read\n  sources:\
  \ [https://app.pennylane.com/.well-known/oauth-authorization-server]\n- scope: mcp:private_api\n  description: Private API access grant on the MCP surface.\n  sources: [https://app.pennylane.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pennylane/refs/heads/main/scopes/pennylane-scopes.yml
summary_line: 23 scopes
tags:
- Accounting
- Invoicing
- Fintech
- Financial Data
- Banking
- France
- SME
token_urls: []
---
