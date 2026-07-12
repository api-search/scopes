---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Coupa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Coupa publishes 8 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coupa API on a user''s behalf.


  Tokens are issued from https://{instance}.coupahost.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coupa
provider_slug: coupa
schemes:
- description: OAuth 2.0 authentication. Coupa supports the client_credentials grant type. Obtain client credentials from Coupa instance setup.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{instance}.coupahost.com/oauth2/token
  name: oauth2
  source: openapi/coupa-core-api-openapi.yml
scope_count: 8
scope_names:
- core.invoices.read
- core.invoices.write
- core.purchase_orders.read
- core.purchase_orders.write
- core.requisitions.read
- core.requisitions.write
- core.suppliers.read
- core.suppliers.write
scopes:
- description: Read invoices
  flows:
  - clientCredentials
  scope: core.invoices.read
- description: Create and update invoices
  flows:
  - clientCredentials
  scope: core.invoices.write
- description: Read purchase orders
  flows:
  - clientCredentials
  scope: core.purchase_orders.read
- description: Create and update purchase orders
  flows:
  - clientCredentials
  scope: core.purchase_orders.write
- description: Read requisitions
  flows:
  - clientCredentials
  scope: core.requisitions.read
- description: Create and update requisitions
  flows:
  - clientCredentials
  scope: core.requisitions.write
- description: Read suppliers
  flows:
  - clientCredentials
  scope: core.suppliers.read
- description: Create and update suppliers
  flows:
  - clientCredentials
  scope: core.suppliers.write
slug: coupa-scopes
source_filename: coupa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coupa-core-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/coupa-core-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{instance}.coupahost.com/oauth2/token\n  description: OAuth 2.0 authentication. Coupa supports the client_credentials grant type. Obtain\n    client credentials from Coupa instance setup.\nscopes:\n- scope: core.invoices.read\n  description: Read invoices\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.invoices.write\n  description: Create and update invoices\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.purchase_orders.read\n  description: Read purchase orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.purchase_orders.write\n  description: Create and update purchase orders\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.requisitions.read\n  description: Read requisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.requisitions.write\n  description: Create and update requisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.suppliers.read\n  description: Read suppliers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- scope: core.suppliers.write\n  description: Create and update suppliers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/scopes/coupa-scopes.yml
summary_line: 8 scopes · clientCredentials
tags:
- BSM
- Business Spend Management
- Cloud Platform
- Enterprise
- Financial Management
- Invoicing
- Procurement
- Supply Chain
token_urls:
- https://{instance}.coupahost.com/oauth2/token
---
