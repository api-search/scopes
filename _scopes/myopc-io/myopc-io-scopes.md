---
api_specs:
- filename: myopc-io-accounting-api-openapi.yml
  format: yaml
  label: OPC Suite Accounting API
  slug: myopc-io-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-accounting-api-openapi.yml
- filename: myopc-io-crm-api-openapi.yml
  format: yaml
  label: OPC Suite CRM API
  slug: myopc-io-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-crm-api-openapi.yml
- filename: myopc-io-hr-api-openapi.yml
  format: yaml
  label: OPC Suite HR API
  slug: myopc-io-hr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-hr-api-openapi.yml
- filename: myopc-io-inventory-api-openapi.yml
  format: yaml
  label: OPC Suite Inventory API
  slug: myopc-io-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-inventory-api-openapi.yml
- filename: myopc-io-sales-api-openapi.yml
  format: yaml
  label: OPC Suite Sales API
  slug: myopc-io-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-sales-api-openapi.yml
- filename: myopc-io-work-api-openapi.yml
  format: yaml
  label: OPC Suite Work API
  slug: myopc-io-work-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopc-io/openapi/myopc-io-work-api-openapi.yml
authorization_urls:
- https://www.myopc.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: OPC Suite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OPC Suite publishes 34 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OPC Suite API on a user''s behalf.


  Tokens are issued from https://www.myopc.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OPC Suite
provider_slug: myopc-io
schemes:
- description: OAuth 2.1 authorization code + PKCE.
  flows:
  - authorizationUrl: https://www.myopc.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.myopc.io/oauth/token
  name: oauth2
  source: openapi/myopc-io-openapi.json
scope_count: 34
scope_names:
- accounting.read
- accounting.write
- activities.read
- activities.write
- agent-tasks.read
- agent-tasks.write
- claims.read
- claims.write
- contacts.read
- contacts.write
- deals.read
- deals.write
- documents.read
- documents.write
- hrm.read
- hrm.write
- inventory.read
- inventory.write
- leads.read
- leads.write
- notes.read
- notes.write
- products.read
- products.write
- projects.read
- projects.write
- purchases.read
- purchases.write
- quotations.read
- quotations.write
- sales.read
- sales.write
- suppliers.read
- suppliers.write
scopes:
- description: ''
  flows: []
  scope: accounting.read
- description: ''
  flows: []
  scope: accounting.write
- description: ''
  flows: []
  scope: activities.read
- description: ''
  flows: []
  scope: activities.write
- description: ''
  flows: []
  scope: agent-tasks.read
- description: ''
  flows: []
  scope: agent-tasks.write
- description: ''
  flows: []
  scope: claims.read
- description: ''
  flows: []
  scope: claims.write
- description: ''
  flows: []
  scope: contacts.read
- description: ''
  flows: []
  scope: contacts.write
- description: ''
  flows: []
  scope: deals.read
- description: ''
  flows: []
  scope: deals.write
- description: ''
  flows: []
  scope: documents.read
- description: ''
  flows: []
  scope: documents.write
- description: ''
  flows: []
  scope: hrm.read
- description: ''
  flows: []
  scope: hrm.write
- description: ''
  flows: []
  scope: inventory.read
- description: ''
  flows: []
  scope: inventory.write
- description: ''
  flows: []
  scope: leads.read
- description: ''
  flows: []
  scope: leads.write
- description: ''
  flows: []
  scope: notes.read
- description: ''
  flows: []
  scope: notes.write
- description: ''
  flows: []
  scope: products.read
- description: ''
  flows: []
  scope: products.write
- description: ''
  flows: []
  scope: projects.read
- description: ''
  flows: []
  scope: projects.write
- description: ''
  flows: []
  scope: purchases.read
- description: ''
  flows: []
  scope: purchases.write
- description: ''
  flows: []
  scope: quotations.read
- description: ''
  flows: []
  scope: quotations.write
- description: ''
  flows: []
  scope: sales.read
- description: ''
  flows: []
  scope: sales.write
- description: ''
  flows: []
  scope: suppliers.read
- description: ''
  flows: []
  scope: suppliers.write
slug: myopc-io-scopes
source_filename: myopc-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myopc-io-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/myopc-io-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.myopc.io/oauth/authorize\n    tokenUrl: https://www.myopc.io/oauth/token\n  description: OAuth 2.1 authorization code + PKCE.\nscopes:\n- scope: accounting.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: accounting.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: activities.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: activities.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: agent-tasks.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: agent-tasks.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: claims.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: claims.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: contacts.read\n  sources:\n  - openapi/myopc-io-openapi.json\n\
  - scope: contacts.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: deals.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: deals.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: documents.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: documents.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: hrm.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: hrm.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: inventory.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: inventory.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: leads.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: leads.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: notes.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: notes.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: products.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: products.write\n\
  \  sources:\n  - openapi/myopc-io-openapi.json\n- scope: projects.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: projects.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: purchases.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: purchases.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: quotations.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: quotations.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: sales.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: sales.write\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: suppliers.read\n  sources:\n  - openapi/myopc-io-openapi.json\n- scope: suppliers.write\n  sources:\n  - openapi/myopc-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myopc-io/scopes/myopc-io-scopes.yml
summary_line: 34 scopes · authorizationCode
tags:
- ERP
- CRM
- Artificial Intelligence
- Business Management
- Software-as-a-Service
token_bound: false
token_urls:
- https://www.myopc.io/oauth/token
---
