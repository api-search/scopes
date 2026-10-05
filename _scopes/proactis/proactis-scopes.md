---
authorization_urls: []
description: Proactis issues OAuth 2.0 client-credentials access tokens from Amazon Cognito. Scopes are resource-server scopes expressed as absolute URIs under the https://api.proactiscloud.com/ resource identifier, one per API service. The list below is read from the decoded payload of the example access token Proactis publishes on its own authentication page — it is what Proactis shows a client actually receives.
docs: https://docs.proactis.com/using-the-api/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Proactis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Proactis publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Proactis API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Proactis
provider_slug: proactis
schemes: []
scope_count: 6
scope_names:
- https://api.proactiscloud.com/orders
- https://api.proactiscloud.com/invoices
- https://api.proactiscloud.com/receipts
- https://api.proactiscloud.com/suppliers
- https://api.proactiscloud.com/accounting
- https://api.proactiscloud.com/einvoicing
scopes:
- description: Create and retrieve ERP orders.
  flows: []
  scope: https://api.proactiscloud.com/orders
- description: Create or retrieve invoices and update payment status.
  flows: []
  scope: https://api.proactiscloud.com/invoices
- description: Create and retrieve receipts.
  flows: []
  scope: https://api.proactiscloud.com/receipts
- description: Create, modify and retrieve suppliers.
  flows: []
  scope: https://api.proactiscloud.com/suppliers
- description: Configure departments, cost centers, cost accounts and cost dimensions.
  flows: []
  scope: https://api.proactiscloud.com/accounting
- description: Import UBL 2.1 invoices into Proactis.
  flows: []
  scope: https://api.proactiscloud.com/einvoicing
slug: proactis-scopes
source_filename: proactis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.proactis.com/using-the-api/authentication\ndocs: https://docs.proactis.com/using-the-api/authentication\nprovider: Proactis\nproviderId: proactis\nname: Proactis OAuth 2.0 scopes\ndescription: >-\n  Proactis issues OAuth 2.0 client-credentials access tokens from Amazon Cognito. Scopes\n  are resource-server scopes expressed as absolute URIs under the\n  https://api.proactiscloud.com/ resource identifier, one per API service. The list below\n  is read from the decoded payload of the example access token Proactis publishes on its\n  own authentication page — it is what Proactis shows a client actually receives.\nflow: clientCredentials\ntokenEndpoint: >-\n  Regional. The docs example uses Host apius.proactiscloud.com; the equivalent UK, EU and\n  NL hosts are apiuk.proactiscloud.com, regos2p-eu1-api.proactiscloud.com and api.esize.nl.\nresourceServer: https://api.proactiscloud.com\nauthorizationServer: https://cognito-idp.eu-west-2.amazonaws.com/<user-pool-id>\n\
  scope_count: 6\nscopes:\n  - name: https://api.proactiscloud.com/orders\n    short: orders\n    api: Order API\n    description: Create and retrieve ERP orders.\n  - name: https://api.proactiscloud.com/invoices\n    short: invoices\n    api: Invoice API\n    description: Create or retrieve invoices and update payment status.\n  - name: https://api.proactiscloud.com/receipts\n    short: receipts\n    api: Receipt API\n    description: Create and retrieve receipts.\n  - name: https://api.proactiscloud.com/suppliers\n    short: suppliers\n    api: Supplier API\n    description: Create, modify and retrieve suppliers.\n  - name: https://api.proactiscloud.com/accounting\n    short: accounting\n    api: Accounting API\n    description: Configure departments, cost centers, cost accounts and cost dimensions.\n  - name: https://api.proactiscloud.com/einvoicing\n    short: einvoicing\n    api: eInvoice API\n    description: Import UBL 2.1 invoices into Proactis.\ngaps:\n  - >-\n    Proactis documents\
  \ ten API services (accounting, contract, eInvoice, invoice, order,\n    receipt, requisition, supplier, timecard, user/SCIM) but the published example token\n    carries only six scopes. No scope URI is published for the Contract, Requisition,\n    Timecard or User (SCIM) APIs. Whether those services use additional scopes, reuse an\n    existing one, or are gated another way is not stated anywhere in the public docs.\n  - >-\n    There is no published scope reference page. Scopes had to be recovered by decoding the\n    example JWT on the authentication page. A dedicated permissions/scopes table would make\n    least-privilege token requests possible without reverse-engineering a sample.\n  - >-\n    No granularity below the service level is documented — there is no read-only vs\n    read-write split, so a token that can retrieve suppliers can also modify them.\nnotes:\n  - >-\n    Scopes are also referenced in the opposite direction: when Proactis pushes documents to\n    a customer\
  \ endpoint using OAUTH2, Communication Settings accept an optional space-separated\n    `scope` value for the customer's own authorization server.\n    See https://docs.proactis.com/using-the-api/transactions/push-transactions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proactis/refs/heads/main/scopes/proactis-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Procurement
- Purchase-To-Pay
- Source-to-Pay
- Spend Management
- Contract Management
- E-Invoicing
- Accounts Payable
- Supplier Management
- eSourcing
- cXML
- UBL
- SCIM
token_bound: false
token_urls: []
---
