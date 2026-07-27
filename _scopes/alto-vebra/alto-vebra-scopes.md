---
api_specs:
- filename: alto-api-openapi.json
  format: json
  label: Alto API
  slug: alto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/alto-api-openapi.json
- filename: zoopla-leads-api-openapi.json
  format: json
  label: Zoopla Leads API
  slug: zoopla-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-leads-api-openapi.json
- filename: zoopla-premium-listing-activations-openapi.json
  format: json
  label: Zoopla Premium Listing Activations API
  slug: zoopla-premium-listing-activations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-premium-listing-activations-openapi.json
- filename: zoopla-weekly-featured-property-openapi.json
  format: json
  label: Zoopla Weekly Featured Property (WFP) Activations API
  slug: zoopla-weekly-featured-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/openapi/zoopla-weekly-featured-property-openapi.json
authorization_urls: []
description: ''
docs:
- https://developers.vebraalto.com/api
- https://developers.vebraalto.com/guides/authenticating-your-requests/
- https://developers.zoopla.co.uk/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Alto Vebra Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alto (Vebra / Zoopla) publishes 104 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alto (Vebra / Zoopla) API on a user''s behalf.


  Tokens are issued from https://api.alto.zoopladev.co.uk/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alto (Vebra / Zoopla)
provider_slug: alto-vebra
schemes:
- description: Documented in prose only; the Alto OpenAPI declares the credential as an apiKey-in-header scheme named Bearer and models no OAuth flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.alto.zoopladev.co.uk/token
  name: alto-token
  source: https://developers.vebraalto.com/guides/authenticating-your-requests/
- flows:
  - flow: clientCredentials
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: OAuth2
  source: openapi/zoopla-leads-api-openapi.json
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: oAuthSample
  source: openapi/zoopla-premium-listing-activations-openapi.json
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token
  name: oAuthSample
  source: openapi/zoopla-weekly-featured-property-openapi.json
scope_count: 104
scope_names:
- leads/list:applicant-leads
- leads/list:appraisal-leads
- api/api_access
- alto/read:appointments
- alto/read:contact_bank_accounts
- alto/read:contacts
- alto/read:leads
- alto/route:delete-contacts-contactid-relationship-contactrelationshipid
- alto/route:delete-inventory-inventoryid-keyset-keysetid
- alto/route:delete-media-item-mediaitemid
- alto/route:get-appointments-appointmentid-instanceid
- alto/route:get-appointments-negotiators
- alto/route:get-appointments-valuations
- alto/route:get-branches
- alto/route:get-branches-branchid
- alto/route:get-clients
- alto/route:get-contacts
- alto/route:get-contacts-all
- alto/route:get-contacts-contactid
- alto/route:get-contacts-contactid-bank-accounts
- alto/route:get-contacts-contactid-persons
- alto/route:get-contacts-contactid-relationship
- alto/route:get-contacts-search
- alto/route:get-documents
- alto/route:get-documents-documentid-content
- alto/route:get-file-notes-filenoteid
- alto/route:get-file-notes-search
- alto/route:get-guarantorids
- alto/route:get-inventory
- alto/route:get-inventory-filter
- alto/route:get-inventory-inventoryid
- alto/route:get-inventory-inventoryid-documents
- alto/route:get-inventory-inventoryid-keysets
- alto/route:get-inventory-inventoryid-landlords
- alto/route:get-inventory-inventoryid-management-events
- alto/route:get-inventory-inventoryid-suppliers
- alto/route:get-inventory-inventoryid-work-orders
- alto/route:get-inventory-items
- alto/route:get-inventory-propertyid-file-notes
- alto/route:get-inventory-search
- alto/route:get-landlords
- alto/route:get-leads
- alto/route:get-leads-leadid
- alto/route:get-listing-filter
- alto/route:get-listing-property-items
- alto/route:get-listing-property-propertyid
- alto/route:get-listing-property-propertyid-images
- alto/route:get-listing-property-propertyid-images-imageid
- alto/route:get-management-events
- alto/route:get-management-events-eventid
- alto/route:get-negotiators
- alto/route:get-negotiators-negotiatorid
- alto/route:get-offers-sales-offer-offerid
- alto/route:get-opt-out-status-linkedtype-linkedid
- alto/route:get-owners
- alto/route:get-parameters-appointment-subtypes
- alto/route:get-parameters-client-disposal-statuses
- alto/route:get-parameters-client-intentions
- alto/route:get-parameters-client-positions
- alto/route:get-parameters-lead-sources
- alto/route:get-parameters-property-types
- alto/route:get-partners-integration
- alto/route:get-referencechecks
- alto/route:get-referrals-referralid
- alto/route:get-sales-progressions
- alto/route:get-sales-progressions-offerid
- alto/route:get-suppliers
- alto/route:get-suppliers-supplierid
- alto/route:get-tenancies
- alto/route:get-tenancies-tenancyid
- alto/route:get-tenancies-tenancyid-meter-readings
- alto/route:get-tenancies-tenancyid-tenantids
- alto/route:get-work-orders-id
- alto/route:get-work-orders-workorderid-documents
- alto/route:patch-appointments-general-appointmentid
- alto/route:patch-appointments-viewings-appointmentid
- alto/route:patch-contacts-contactid-applicant-requirements-requirementid
- alto/route:patch-contacts-contactid-persons-personid
- alto/route:patch-inventory-propertyid-appraisal
- alto/route:patch-listing-property-propertyid-rooms
- alto/route:patch-listing-property-propertyid-summary
- alto/route:patch-referencechecks-referencecheckid
- alto/route:patch-tenancies-tenancyid-meter-readings-utilitytype
- alto/route:post-appointments-general
- alto/route:post-appointments-viewings
- alto/route:post-appraisals
- alto/route:post-contacts-contactid-applicant-requirements
- alto/route:post-contacts-contactid-forwarding-address
- alto/route:post-contacts-contactid-preferences
- alto/route:post-documents-post
- alto/route:post-file-notes
- alto/route:post-inventory-inventoryid-keyset
- alto/route:post-inventory-inventoryid-media-link
- alto/route:post-inventory-inventoryid-owner
- alto/route:post-inventory-inventoryid-tenancies
- alto/route:post-inventory-new
- alto/route:post-inventory-propertyid-charges
- alto/route:post-media-item
- alto/route:post-partners-integration-status
- alto/route:post-tenancies-tenancyid-charges
- alto/route:post-work-orders
- alto/update:leads
- alto/write:appointments_general
- alto/write:appointments_viewings
scopes:
- description: Grants read access to applicant lead lists
  flows:
  - clientCredentials
  scope: leads/list:applicant-leads
- description: Grants read access to appraisal lead lists
  flows:
  - clientCredentials
  scope: leads/list:appraisal-leads
- description: access to the API — a single undifferentiated scope covering every Premium Listing and WFP operation, read and write alike
  flows:
  - clientCredentials
  scope: api/api_access
- description: ''
  flows:
  - clientCredentials
  scope: alto/read:appointments
- description: ''
  flows:
  - clientCredentials
  scope: alto/read:contact_bank_accounts
- description: ''
  flows:
  - clientCredentials
  scope: alto/read:contacts
- description: ''
  flows:
  - clientCredentials
  scope: alto/read:leads
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:delete-contacts-contactid-relationship-contactrelationshipid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:delete-inventory-inventoryid-keyset-keysetid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:delete-media-item-mediaitemid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-appointments-appointmentid-instanceid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-appointments-negotiators
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-appointments-valuations
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-branches
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-branches-branchid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-clients
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts-all
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts-contactid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts-contactid-bank-accounts
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts-contactid-persons
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts-contactid-relationship
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-contacts-search
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-documents
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-documents-documentid-content
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-file-notes-filenoteid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-file-notes-search
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-guarantorids
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-filter
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid-documents
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid-keysets
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid-landlords
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid-management-events
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid-suppliers
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-inventoryid-work-orders
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-items
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-propertyid-file-notes
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-inventory-search
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-landlords
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-leads
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-leads-leadid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-listing-filter
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-listing-property-items
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-listing-property-propertyid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-listing-property-propertyid-images
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-listing-property-propertyid-images-imageid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-management-events
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-management-events-eventid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-negotiators
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-negotiators-negotiatorid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-offers-sales-offer-offerid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-opt-out-status-linkedtype-linkedid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-owners
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-parameters-appointment-subtypes
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-parameters-client-disposal-statuses
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-parameters-client-intentions
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-parameters-client-positions
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-parameters-lead-sources
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-parameters-property-types
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-partners-integration
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-referencechecks
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-referrals-referralid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-sales-progressions
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-sales-progressions-offerid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-suppliers
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-suppliers-supplierid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-tenancies
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-tenancies-tenancyid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-tenancies-tenancyid-meter-readings
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-tenancies-tenancyid-tenantids
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-work-orders-id
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:get-work-orders-workorderid-documents
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-appointments-general-appointmentid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-appointments-viewings-appointmentid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-contacts-contactid-applicant-requirements-requirementid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-contacts-contactid-persons-personid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-inventory-propertyid-appraisal
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-listing-property-propertyid-rooms
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-listing-property-propertyid-summary
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-referencechecks-referencecheckid
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:patch-tenancies-tenancyid-meter-readings-utilitytype
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-appointments-general
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-appointments-viewings
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-appraisals
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-contacts-contactid-applicant-requirements
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-contacts-contactid-forwarding-address
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-contacts-contactid-preferences
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-documents-post
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-file-notes
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-inventory-inventoryid-keyset
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-inventory-inventoryid-media-link
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-inventory-inventoryid-owner
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-inventory-inventoryid-tenancies
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-inventory-new
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-inventory-propertyid-charges
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-media-item
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-partners-integration-status
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-tenancies-tenancyid-charges
- description: ''
  flows:
  - clientCredentials
  scope: alto/route:post-work-orders
- description: ''
  flows:
  - clientCredentials
  scope: alto/update:leads
- description: ''
  flows:
  - clientCredentials
  scope: alto/write:appointments_general
- description: ''
  flows:
  - clientCredentials
  scope: alto/write:appointments_viewings
slug: alto-vebra-scopes
source_filename: alto-vebra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/alto-api-openapi.json, openapi/zoopla-leads-api-openapi.json, openapi/zoopla-premium-listing-activations-openapi.json,\n  openapi/zoopla-weekly-featured-property-openapi.json\ndocs:\n- https://developers.vebraalto.com/api\n- https://developers.vebraalto.com/guides/authenticating-your-requests/\n- https://developers.zoopla.co.uk/docs/authentication\nsummary:\n  total: 104\n  alto: 101\n  zoopla: 3\n  declaration_style: 'Alto scopes are published in prose inside each operation description (\"Required\n    scope: alto/read:contacts\"), NOT in an OpenAPI securitySchemes flow object — a generated client will\n    not see them. Zoopla scopes are declared properly in securityDefinitions/securitySchemes.'\n  naming_generations:\n  - pattern: alto/<verb>:<resource>\n    example: alto/read:contacts\n    count: 6\n    note: Semantic, human-readable, groups several operations under one grant.\n  - pattern: alto/route:<method>-<path-with-dashes>\n\
  \    example: alto/route:get-inventory-inventoryid-tenancies\n    count: 95\n    note: Mechanical one-scope-per-route generation. Least-privilege by construction but unreadable, unstable\n      against any URL change, and effectively a permission per endpoint.\n  coverage: 111 of the 112 Alto operations carry at least one published scope string in their description.\n  observation: Two naming generations coexist in the same live contract. Six semantic scopes cover appointments,\n    contacts, leads and contact bank accounts; every other operation is gated by its own generated route\n    scope. The Zoopla product APIs sit at the opposite extreme — one coarse api/api_access scope authorises\n    both read and write across Premium Listings and WFP.\nschemes:\n- name: alto-token\n  source: https://developers.vebraalto.com/guides/authenticating-your-requests/\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.alto.zoopladev.co.uk/token\n  description: Documented in prose only;\
  \ the Alto OpenAPI declares the credential as an apiKey-in-header\n    scheme named Bearer and models no OAuth flow.\n- name: OAuth2\n  source: openapi/zoopla-leads-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n- name: oAuthSample\n  source: openapi/zoopla-premium-listing-activations-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n  description: This API uses OAuth 2 with the client credentials grant flow.\n- name: oAuthSample\n  source: openapi/zoopla-weekly-featured-property-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://services-auth.services.zoopla.co.uk/oauth2/token\n  description: This API uses OAuth 2 with the client credentials grant flow.\ntenancy_note: Scope is not the whole authorization story on Alto. Every call also carries an AgencyRef\n  header that scopes the token to one activating agency;\
  \ a valid token with the right scope and the wrong\n  AgencyRef returns 403. See authentication/alto-vebra-authentication.yml.\nscopes:\n- scope: leads/list:applicant-leads\n  api: Zoopla Leads API\n  kind: semantic\n  description: Grants read access to applicant lead lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zoopla-leads-api-openapi.json\n  operations:\n  - operation: GET /applicant-leads\n- scope: leads/list:appraisal-leads\n  api: Zoopla Leads API\n  kind: semantic\n  description: Grants read access to appraisal lead lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zoopla-leads-api-openapi.json\n  operations:\n  - operation: GET /appraisal-leads\n- scope: api/api_access\n  api: Zoopla Premium Listing Activations API, Zoopla Weekly Featured Property (WFP) Activations API\n  kind: coarse\n  description: access to the API — a single undifferentiated scope covering every Premium Listing and\n    WFP operation, read and write alike\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/zoopla-premium-listing-activations-openapi.json\n  - openapi/zoopla-weekly-featured-property-openapi.json\n  operations:\n  - operation: GET /products/premium-listings\n  - operation: POST /products/premium-listings\n  - operation: GET /products/premium-listings/{uuid}\n  - operation: PATCH /products/premium-listings/{uuid}\n  - operation: GET /products/weekly-featured-properties\n  - operation: POST /products/weekly-featured-properties\n  - operation: GET /products/weekly-featured-properties/{uuid}\n- scope: alto/read:appointments\n  api: Alto API\n  kind: semantic\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  - Parameters\n  operations:\n  - operation: GET /appointments/{appointmentId}/{instanceId}\n  - operation: GET /appointments/negotiators\n  - operation: GET /parameters/appointment-subtypes\n- scope: alto/read:contact_bank_accounts\n  api: Alto API\n  kind: semantic\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/{contactId}/bank-accounts\n    operationId: ListBankAccounts\n- scope: alto/read:contacts\n  api: Alto API\n  kind: semantic\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Owners\n  operations:\n  - operation: GET /owners\n    operationId: GetOwners\n- scope: alto/read:leads\n  api: Alto API\n  kind: semantic\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Leads\n  operations:\n  - operation: GET /leads\n- scope: alto/route:delete-contacts-contactid-relationship-contactrelationshipid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: DELETE /contacts/{contactId}/relationship/{contactRelationshipId}\n\
  \    operationId: DeleteContactRelationship\n- scope: alto/route:delete-inventory-inventoryid-keyset-keysetid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: PATCH /inventory/{inventoryId}/keyset/{keySetId}\n  - operation: DELETE /inventory/{inventoryId}/keyset/{keySetId}\n- scope: alto/route:delete-media-item-mediaitemid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Media\n  operations:\n  - operation: DELETE /media-item/{mediaItemId}\n- scope: alto/route:get-appointments-appointmentid-instanceid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: GET /appointments/{appointmentId}/{instanceId}\n- scope: alto/route:get-appointments-negotiators\n\
  \  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: GET /appointments/negotiators\n- scope: alto/route:get-appointments-valuations\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: GET /appointments/valuations\n- scope: alto/route:get-branches\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Branches\n  operations:\n  - operation: GET /branches\n- scope: alto/route:get-branches-branchid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Branches\n  operations:\n  - operation: GET /branches/{branchId}\n- scope: alto/route:get-clients\n  api: Alto API\n\
  \  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Clients\n  operations:\n  - operation: GET /clients\n- scope: alto/route:get-contacts\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts\n    operationId: GetContactsById\n  - operation: POST /contacts\n    operationId: CreateContact\n- scope: alto/route:get-contacts-all\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/all\n    operationId: GetAllContacts\n- scope: alto/route:get-contacts-contactid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/{contactId}\n\
  \    operationId: GetContact\n  - operation: PATCH /contacts/{contactId}\n    operationId: UpdateContact\n- scope: alto/route:get-contacts-contactid-bank-accounts\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/{contactId}/bank-accounts\n    operationId: ListBankAccounts\n- scope: alto/route:get-contacts-contactid-persons\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/{contactId}/persons\n    operationId: GetPersons\n- scope: alto/route:get-contacts-contactid-relationship\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/{contactId}/relationship\n    operationId:\
  \ GetContactRelationship\n  - operation: POST /contacts/{contactId}/relationship\n    operationId: CreateContactRelationship\n- scope: alto/route:get-contacts-search\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/search\n- scope: alto/route:get-documents\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Documents\n  operations:\n  - operation: GET /documents\n    operationId: GetDocumentsByType\n- scope: alto/route:get-documents-documentid-content\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Documents\n  operations:\n  - operation: GET /documents/{documentId}/content\n- scope: alto/route:get-file-notes-filenoteid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - FileNotes\n  operations:\n  - operation: GET /file-notes/{fileNoteId}\n    operationId: GetFileNote\n  - operation: PATCH /file-notes/{fileNoteId}\n    operationId: PatchFileNote\n- scope: alto/route:get-file-notes-search\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - FileNotes\n  operations:\n  - operation: GET /file-notes/search\n    operationId: SearchFileNotes\n- scope: alto/route:get-guarantorids\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - LettingsProgression\n  operations:\n  - operation: GET /guarantorIds\n- scope: alto/route:get-inventory\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: GET /inventory\n\
  - scope: alto/route:get-inventory-filter\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: GET /inventory/filter\n- scope: alto/route:get-inventory-inventoryid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: GET /inventory/{inventoryId}\n  - operation: PATCH /inventory/{inventoryId}\n- scope: alto/route:get-inventory-inventoryid-documents\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Documents\n  operations:\n  - operation: GET /inventory/{inventoryId}/documents\n- scope: alto/route:get-inventory-inventoryid-keysets\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n\
  \  - Inventory\n  operations:\n  - operation: GET /inventory/{inventoryId}/keysets\n- scope: alto/route:get-inventory-inventoryid-landlords\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Landlords\n  operations:\n  - operation: GET /inventory/{inventoryId}/landlords\n- scope: alto/route:get-inventory-inventoryid-management-events\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - ManagementEvents\n  operations:\n  - operation: GET /inventory/{inventoryId}/management-events\n- scope: alto/route:get-inventory-inventoryid-suppliers\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Suppliers\n  operations:\n  - operation: GET /inventory/{inventoryId}/suppliers\n- scope: alto/route:get-inventory-inventoryid-work-orders\n  api:\
  \ Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - WorkOrders\n  operations:\n  - operation: GET /inventory/{inventoryId}/work-orders\n- scope: alto/route:get-inventory-items\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: GET /inventory/items\n- scope: alto/route:get-inventory-propertyid-file-notes\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - FileNotes\n  operations:\n  - operation: GET /inventory/{propertyId}/file-notes\n    operationId: GetFileNotesByProperty\n- scope: alto/route:get-inventory-search\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: GET\
  \ /inventory/search\n- scope: alto/route:get-landlords\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Landlords\n  operations:\n  - operation: GET /landlords\n- scope: alto/route:get-leads\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Leads\n  operations:\n  - operation: GET /leads\n  - operation: POST /leads\n- scope: alto/route:get-leads-leadid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Leads\n  operations:\n  - operation: GET /leads/{leadId}\n    operationId: GetById\n  - operation: PATCH /leads/{leadId}\n    operationId: UpdateLead\n- scope: alto/route:get-listing-filter\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n \
  \ - Listing\n  operations:\n  - operation: GET /listing/filter\n- scope: alto/route:get-listing-property-items\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Listing\n  operations:\n  - operation: GET /listing/property/items\n- scope: alto/route:get-listing-property-propertyid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Listing\n  operations:\n  - operation: GET /listing/property/{propertyId}\n- scope: alto/route:get-listing-property-propertyid-images\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Listing\n  operations:\n  - operation: GET /listing/property/{propertyId}/images\n- scope: alto/route:get-listing-property-propertyid-images-imageid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/alto-api-openapi.json\n  resource_families:\n  - Listing\n  operations:\n  - operation: GET /listing/property/{propertyId}/images/{imageId}\n- scope: alto/route:get-management-events\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - ManagementEvents\n  operations:\n  - operation: GET /management-events\n  - operation: POST /management-events\n- scope: alto/route:get-management-events-eventid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - ManagementEvents\n  operations:\n  - operation: GET /management-events/{eventId}\n  - operation: PATCH /management-events/{eventId}\n- scope: alto/route:get-negotiators\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Negotiators\n  operations:\n  - operation: GET /negotiators\n\
  - scope: alto/route:get-negotiators-negotiatorid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Negotiators\n  operations:\n  - operation: GET /negotiators/{negotiatorId}\n- scope: alto/route:get-offers-sales-offer-offerid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Offers\n  operations:\n  - operation: GET /offers/sales-offer/{offerId}\n- scope: alto/route:get-opt-out-status-linkedtype-linkedid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Partners\n  operations:\n  - operation: GET /opt-out-status/{linkedType}/{linkedId}\n    operationId: GetIntegrationOptOutStatus\n- scope: alto/route:get-owners\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n\
  \  resource_families:\n  - Owners\n  operations:\n  - operation: GET /owners\n    operationId: GetOwners\n- scope: alto/route:get-parameters-appointment-subtypes\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Parameters\n  operations:\n  - operation: GET /parameters/appointment-subtypes\n- scope: alto/route:get-parameters-client-disposal-statuses\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Parameters\n  operations:\n  - operation: GET /parameters/client-disposal-statuses\n    operationId: GetClientDisposalStatuses\n- scope: alto/route:get-parameters-client-intentions\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Parameters\n  operations:\n  - operation: GET /parameters/client-intentions\n    operationId: GetIntentions\n\
  - scope: alto/route:get-parameters-client-positions\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Parameters\n  operations:\n  - operation: GET /parameters/client-positions\n    operationId: GetPositions\n- scope: alto/route:get-parameters-lead-sources\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Parameters\n  operations:\n  - operation: GET /parameters/lead-sources\n    operationId: GetLeadSources\n- scope: alto/route:get-parameters-property-types\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Parameters\n  operations:\n  - operation: GET /parameters/property-types\n    operationId: GetPropertyTypes\n- scope: alto/route:get-partners-integration\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Partners\n  operations:\n  - operation: GET /partners/integration\n- scope: alto/route:get-referencechecks\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - ReferenceChecks\n  operations:\n  - operation: GET /ReferenceChecks\n- scope: alto/route:get-referrals-referralid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Referrals\n  operations:\n  - operation: GET /referrals/{referralId}\n  - operation: PATCH /referrals/{referralId}\n- scope: alto/route:get-sales-progressions\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - SalesProgression\n  operations:\n  - operation: GET /sales-progressions\n- scope: alto/route:get-sales-progressions-offerid\n  api:\
  \ Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - SalesProgression\n  operations:\n  - operation: GET /sales-progressions/{offerId}\n- scope: alto/route:get-suppliers\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Suppliers\n  operations:\n  - operation: GET /suppliers\n- scope: alto/route:get-suppliers-supplierid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Suppliers\n  operations:\n  - operation: GET /suppliers/{supplierId}\n- scope: alto/route:get-tenancies\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Tenancies\n  operations:\n  - operation: GET /tenancies\n- scope: alto/route:get-tenancies-tenancyid\n  api: Alto API\n  kind:\
  \ route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Tenancies\n  operations:\n  - operation: GET /tenancies/{tenancyId}\n  - operation: PATCH /tenancies/{tenancyId}\n- scope: alto/route:get-tenancies-tenancyid-meter-readings\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Tenancies\n  operations:\n  - operation: GET /tenancies/{tenancyId}/meter-readings\n  - operation: POST /tenancies/{tenancyId}/meter-readings\n- scope: alto/route:get-tenancies-tenancyid-tenantids\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Tenancies\n  operations:\n  - operation: GET /tenancies/{tenancyId}/tenantIds\n- scope: alto/route:get-work-orders-id\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n\
  \  - WorkOrders\n  operations:\n  - operation: GET /work-orders/{id}\n  - operation: PATCH /work-orders/{id}\n- scope: alto/route:get-work-orders-workorderid-documents\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Documents\n  operations:\n  - operation: GET /work-orders/{workOrderId}/documents\n- scope: alto/route:patch-appointments-general-appointmentid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: PATCH /appointments/general/{appointmentId}\n- scope: alto/route:patch-appointments-viewings-appointmentid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: PATCH /appointments/viewings/{appointmentId}\n- scope: alto/route:patch-contacts-contactid-applicant-requirements-requirementid\n\
  \  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: PATCH /contacts/{contactId}/applicant-requirements/{requirementId}\n    operationId: UpdateApplicantRequirement\n- scope: alto/route:patch-contacts-contactid-persons-personid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: PATCH /contacts/{contactId}/persons/{personId}\n    operationId: UpdatePerson\n  - operation: GET /contacts/{contactId}/persons/{personId}\n    operationId: GetPerson\n- scope: alto/route:patch-inventory-propertyid-appraisal\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appraisals\n  operations:\n  - operation: PATCH /inventory/{propertyId}/appraisal\n    operationId: PatchAppraisal\n\
  - scope: alto/route:patch-listing-property-propertyid-rooms\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Listing\n  operations:\n  - operation: PATCH /listing/property/{propertyId}/rooms\n    operationId: PatchListingRooms\n- scope: alto/route:patch-listing-property-propertyid-summary\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Listing\n  operations:\n  - operation: PATCH /listing/property/{propertyId}/summary\n    operationId: PatchListingSummary\n- scope: alto/route:patch-referencechecks-referencecheckid\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - ReferenceChecks\n  operations:\n  - operation: PATCH /ReferenceChecks/{referenceCheckId}\n- scope: alto/route:patch-tenancies-tenancyid-meter-readings-utilitytype\n\
  \  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Tenancies\n  operations:\n  - operation: PATCH /tenancies/{tenancyId}/meter-readings/{utilityType}\n- scope: alto/route:post-appointments-general\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: POST /appointments/general\n- scope: alto/route:post-appointments-viewings\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: POST /appointments/viewings\n- scope: alto/route:post-appraisals\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appraisals\n  operations:\n  - operation: POST /appraisals\n    operationId:\
  \ CreateAppraisal\n- scope: alto/route:post-contacts-contactid-applicant-requirements\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: POST /contacts/{contactId}/applicant-requirements\n    operationId: CreateApplicantRequirement\n- scope: alto/route:post-contacts-contactid-forwarding-address\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: POST /contacts/{contactId}/forwarding-address\n    operationId: CreateForwardingAddress\n- scope: alto/route:post-contacts-contactid-preferences\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Contacts\n  operations:\n  - operation: GET /contacts/{contactId}/preferences\n    operationId: GetPreferences\n\
  \  - operation: POST /contacts/{contactId}/preferences\n- scope: alto/route:post-documents-post\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Documents\n  operations:\n  - operation: POST /documents/post\n- scope: alto/route:post-file-notes\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - FileNotes\n  operations:\n  - operation: POST /file-notes\n    operationId: CreateFileNote\n- scope: alto/route:post-inventory-inventoryid-keyset\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: POST /inventory/{inventoryId}/keyset\n- scope: alto/route:post-inventory-inventoryid-media-link\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n\
  \  resource_families:\n  - Media\n  operations:\n  - operation: POST /inventory/{inventoryId}/media-link\n- scope: alto/route:post-inventory-inventoryid-owner\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: POST /inventory/{inventoryId}/owner\n- scope: alto/route:post-inventory-inventoryid-tenancies\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Tenancies\n  operations:\n  - operation: GET /inventory/{inventoryId}/tenancies\n  - operation: POST /inventory/{inventoryId}/tenancies\n- scope: alto/route:post-inventory-new\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Inventory\n  operations:\n  - operation: POST /inventory/new\n- scope: alto/route:post-inventory-propertyid-charges\n\
  \  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Charges\n  operations:\n  - operation: POST /inventory/{propertyId}/charges\n- scope: alto/route:post-media-item\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Media\n  operations:\n  - operation: POST /media-item\n- scope: alto/route:post-partners-integration-status\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Partners\n  operations:\n  - operation: POST /partners/integration/status\n- scope: alto/route:post-tenancies-tenancyid-charges\n  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Charges\n  operations:\n  - operation: POST /tenancies/{tenancyId}/charges\n- scope: alto/route:post-work-orders\n\
  \  api: Alto API\n  kind: route\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - WorkOrders\n  operations:\n  - operation: POST /work-orders\n- scope: alto/update:leads\n  api: Alto API\n  kind: semantic\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Leads\n  operations:\n  - operation: PATCH /leads/{leadId}\n    operationId: UpdateLead\n- scope: alto/write:appointments_general\n  api: Alto API\n  kind: semantic\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation: POST /appointments/general\n  - operation: PATCH /appointments/general/{appointmentId}\n- scope: alto/write:appointments_viewings\n  api: Alto API\n  kind: semantic\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/alto-api-openapi.json\n  resource_families:\n  - Appointments\n  operations:\n  - operation:\
  \ POST /appointments/viewings\n  - operation: PATCH /appointments/viewings/{appointmentId}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alto-vebra/refs/heads/main/scopes/alto-vebra-scopes.yml
summary_line: 104 scopes · clientCredentials
tags:
- Real Estate
- United Kingdom
- PropTech
- Property Listings
- CRM
- Property Management
- Rentals
- Conveyancing
- Estate Agency
- Tenancy
- Webhooks
- Events
- Lettings
- Sales Progression
- Property Data
- Real Estate Software
token_urls:
- https://api.alto.zoopladev.co.uk/token
- https://services-auth.services.zoopla.co.uk/oauth2/token
---
