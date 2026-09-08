---
api_specs:
- filename: accela-records-openapi.yml
  format: yaml
  label: Accela Construct API (V4)
  slug: accela-construct-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/openapi/accela-records-openapi.yml
- filename: accela-authentication-openapi.yml
  format: yaml
  label: Accela Authentication API (OAuth 2.0)
  slug: accela-authentication-api-oauth-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/openapi/accela-authentication-openapi.yml
authorization_urls: []
description: ''
docs:
- https://developer.accela.com/docs/construct-permissionScopes.html
- https://developer.accela.com/docs/construct-apiAuth.html
- https://developer.accela.com/docs/api_reference/api-index.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Accela Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Accela uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accela
provider_slug: accela
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: accela-scopes
source_filename: accela-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developer.accela.com/docs/construct-permissionScopes.html\ndocs:\n- https://developer.accela.com/docs/construct-permissionScopes.html\n- https://developer.accela.com/docs/construct-apiAuth.html\n- https://developer.accela.com/docs/api_reference/api-index.html\nsummary: Accela Construct permission scopes. Each scope represents a group of API resources an access token may\n  reach; a token is requested with an explicit scope list and the user is prompted to consent to it. The scope registry\n  is not published as a standalone reference page and does not appear in any securityDefinitions block — Accela\n  declares the scope for each operation inline, as a \"**Scope**:\" line in that operation's description in the published\n  Swagger 2.0 documents. This file is that registry, extracted operation by operation from all fifteen specs in\n  openapi/ and cross-checked against the docs page that describes how scopes are consented\
  \ to.\nflows:\n- authorization_code\n- implicit\n- password\nconsent: An app requests a scope list at token time; the user is shown the list and must Allow. The get_civicid_profile\n  scope is always included whether or not it is requested.\nalways_granted:\n- get_civicid_profile\nscope_count: 32\noperations_mapped: 411\nunmapped_operations: 6\nunmapped_note: Operations with no \"**Scope**:\" line in their published description. Most are the three oauth2 endpoints\n  on auth.accela.com, which are not scope-gated, plus a small number of operations whose description omits the field.\nscopes:\n- name: records\n  description: Transactional records (permits, licenses, service requests, applications) and every child resource\n    that hangs off a record — addresses, contacts, conditions, comments, costs, fees, documents, owners, parcels,\n    professionals, workflows and votes.\n  operations: 117\n  specs:\n  - accela-assets-assessments-openapi.yml\n  - accela-records-openapi.yml\n  - accela-search-openapi.yml\n\
  \  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.assets.records\n  - v4.get.records\n  - v4.post.records\n- name: inspections\n  description: Inspections, inspection scheduling and results, checklists and checklist items, inspection conditions\n    and approvals, inspectors and inspection time accounting.\n  operations: 68\n  specs:\n  - accela-inspections-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.inspections\n  - v4.get.inspections.ids\n  - v4.delete.inspections.ids\n- name: contacts\n  description: Reference contacts and their addresses, conditions, custom forms and custom tables.\n  operations: 27\n  specs:\n  - accela-contacts-professionals-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.contacts\n  - v4.post.contacts\n  - v4.get.contacts.ids\n- name: settings\n  description: 'Read-only Civic Platform Administration configuration: standard\
  \ choices, record/inspection/asset\n    types, departments, priorities, statuses, pick lists and drilldowns.'\n  operations: 25\n  specs:\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.settings.activities.priorities\n  - v4.get.settings.activities.statuses\n  - v4.get.settings.activities.types\n- name: users\n  description: Citizen Access user accounts, self-registration, delegates and delegate privileges, and CivicID-linked\n    citizen profiles.\n  operations: 23\n  specs:\n  - accela-citizens-openapi.yml\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.post.citizenaccess.register\n  - v4.get.civicid.citizenaccess.profile\n  - v4.get.civicid.citizenaccess.contacts\n- name: assets\n  description: Assets, asset attributes, linked assets, asset documents and the records attached to an asset.\n  operations: 20\n  specs:\n  - accela-assets-assessments-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n\
  \  - v4.get.assets\n  - v4.get.assets.ids\n  - v4.delete.assets.ids\n- name: documents\n  description: Document metadata, upload, download and thumbnails, plus the document review surface and document\n    settings.\n  operations: 20\n  specs:\n  - accela-addresses-parcels-owners-openapi.yml\n  - accela-documents-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.delete.parcels.id.documents.ids\n  - v4.get.documents.documentIds\n  - v4.get.documents.documentId.download\n- name: addresses\n  description: Reference addresses, their conditions, the parcels and records they are attached to.\n  operations: 16\n  specs:\n  - accela-addresses-parcels-owners-openapi.yml\n  - accela-records-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.addresses\n  - v4.get.addresses.id\n  - v4.put.addresses.id\n- name: professionals\n  description: Licensed professionals, their conditions and the records they appear on.\n\
  \  operations: 16\n  specs:\n  - accela-contacts-professionals-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.professionals\n  - v4.get.professionals.ids\n  - v4.delete.professionals.ids\n- name: assessments\n  description: Condition assessments against assets — observations, attributes, documents and generated work orders.\n  operations: 15\n  specs:\n  - accela-assets-assessments-openapi.yml\n  - accela-search-openapi.yml\n  example_operations:\n  - v4.post.assets.id.assessments\n  - v4.get.assessments.mine\n  - v4.get.assessments.id\n- name: parcels\n  description: Reference parcels, their conditions, owners, addresses and records.\n  operations: 8\n  specs:\n  - accela-addresses-parcels-owners-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.parcels\n  - v4.get.parcels.id\n  - v4.get.parcels.id.addresses\n- name: agencies\n  description: Agency directory, agency\
  \ environments, environment status and agency logo.\n  operations: 6\n  specs:\n  - accela-agencies-openapi.yml\n  - accela-search-openapi.yml\n  example_operations:\n  - v4.get.agencies\n  - v4.get.agencies.name\n  - v4.get.agencies.name.logo\n- name: conditions\n  description: Standard conditions and standard approval conditions defined at the agency level.\n  operations: 6\n  specs:\n  - accela-miscellaneous-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.conditions.standard\n  - v4.get.conditionApprovals.standard\n  - v4.get.settings.conditionApprovals.statuses\n- name: civicid\n  description: CivicId accounts and profile — the cross-agency identity that links multiple agency Citizen Access\n    accounts to one login.\n  operations: 5\n  specs:\n  - accela-civicid-openapi.yml\n  example_operations:\n  - v4.post.civicid.accounts\n  - v4.get.civicid.accounts.id\n  - v4.delete.civicid.accounts.id\n- name: owners\n  description: Reference property owners\
  \ and their conditions.\n  operations: 5\n  specs:\n  - accela-addresses-parcels-owners-openapi.yml\n  - accela-search-openapi.yml\n  - accela-settings-openapi.yml\n  example_operations:\n  - v4.get.owners\n  - v4.get.owners.id\n  - v4.get.owners.ownerId.conditions\n- name: shoppingcart\n  description: Citizen shopping carts used to assemble fees before payment.\n  operations: 5\n  specs:\n  - accela-payments-openapi.yml\n  example_operations:\n  - v4.get.shoppingCart\n  - v4.post.shoppingCart\n  - v4.get.shoppingCart.ids\n- name: payments\n  description: Payment initialization, commit and void, and transaction fees.\n  operations: 4\n  specs:\n  - accela-payments-openapi.yml\n  example_operations:\n  - v4.post.payments.initialize\n  - v4.put.payments.id\n  - v4.put.payments.paymentId.void\n- name: reports\n  description: Report definitions, report categories and report execution.\n  operations: 4\n  specs:\n  - accela-reports-openapi.yml\n  example_operations:\n  - v4.post.reports.reportId\n\
  \  - v4.get.settings.reports.categories\n  - v4.get.settings.reports.definitions\n- name: timeaccounting\n  description: Time accounting entries against records and inspections.\n  operations: 4\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.get.timeAccounting\n  - v4.post.timeAccounting\n  - v4.delete.timeAccounting.ids\n- name: announcements\n  description: Agency announcements shown to citizens, and marking them read.\n  operations: 2\n  specs:\n  - accela-citizens-openapi.yml\n  example_operations:\n  - v4.get.announcements\n  - v4.put.announcements.ids.read\n- name: app_data\n  description: App settings and Civic Platform server properties (AA version).\n  operations: 2\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.get.serverProperties\n  - v4.get.appsettings\n- name: filters\n  description: Saved filters and filter result execution.\n  operations: 2\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n\
  \  - v4.get.filters\n  - v4.post.filters.id.results\n- name: gis\n  description: Reverse geocoding and GIS dynamic themes.\n  operations: 2\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.get.geo.geocode.reverse\n  - v4.get.gis.dynamic.themes\n- name: batch_request\n  description: The batch endpoint, which composes multiple Construct calls into one request.\n  operations: 1\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.post.batch\n- name: costs\n  description: Record cost items.\n  operations: 1\n  specs:\n  - accela-records-openapi.yml\n  example_operations:\n  - v4.put.records.recordId.costs.id\n- name: global_search\n  description: The cross-object global search endpoint.\n  operations: 1\n  specs:\n  - accela-search-openapi.yml\n  example_operations:\n  - v4.get.search.global\n- name: invoices\n  description: Invoices attached to records.\n  operations: 1\n  specs:\n  - accela-payments-openapi.yml\n  example_operations:\n\
  \  - v4.get.invoices.invoiceIds\n- name: mileage\n  description: Mileage entries created by field staff.\n  operations: 1\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.post.mileage\n- name: parts\n  description: The parts search endpoint.\n  operations: 1\n  specs:\n  - accela-search-openapi.yml\n  example_operations:\n  - v4.post.search.parts\n- name: search_costs\n  description: The cost search endpoint.\n  operations: 1\n  specs:\n  - accela-search-openapi.yml\n  example_operations:\n  - v4.post.search.costs\n- name: trustaccounts\n  description: Citizen and record trust accounts.\n  operations: 1\n  specs:\n  - accela-payments-openapi.yml\n  example_operations:\n  - v4.get.trustAccounts\n- name: workflows\n  description: Workflow tasks assigned to the authenticated user.\n  operations: 1\n  specs:\n  - accela-miscellaneous-openapi.yml\n  example_operations:\n  - v4.get.workflowTasks.mine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/scopes/accela-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- GovTech
- Government
- Permitting
- Licensing
- Code Enforcement
- Inspections
- Asset Management
- Citizen Engagement
- Land Management
- Civic Platform
- Public Sector
- SaaS
token_urls: []
---
