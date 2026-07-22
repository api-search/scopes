---
api_specs:
- filename: xentral-api-openapi-original.json
  format: json
  label: Xentral API
  slug: xentral-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/openapi/xentral-api-openapi-original.json
- filename: xentral-documents-api-openapi-original.json
  format: json
  label: Xentral Business Documents API v3
  slug: xentral-business-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/openapi/xentral-documents-api-openapi-original.json
authorization_urls: []
description: ''
docs: https://developer.xentral.com/reference/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Xentral Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xentral publishes 100 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xentral API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xentral
provider_slug: xentral
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/xentral-api-openapi-original.json
  - openapi/xentral-documents-api-openapi-original.json
  type: http
scope_count: 100
scope_names:
- creditNote:create
- creditNote:delete
- creditNote:read
- creditNote:release
- creditNote:removeWriteProtection
- creditNote:send
- creditNote:setWriteProtection
- creditNote:update
- customer:create
- customer:delete
- customer:read
- customer:update
- deliveryNote:cancel
- deliveryNote:complete
- deliveryNote:create
- deliveryNote:delete
- deliveryNote:read
- deliveryNote:release
- deliveryNote:removeWriteProtection
- deliveryNote:send
- deliveryNote:setWriteProtection
- deliveryNote:update
- deliveryThreshold:create
- invoice:create
- invoice:delete
- invoice:read
- invoice:release
- invoice:removeWriteProtection
- invoice:send
- invoice:setWriteProtection
- invoice:update
- mailAcct:sendEmail
- offer:cancel
- offer:create
- offer:delete
- offer:read
- offer:release
- offer:removeWriteProtection
- offer:send
- offer:setWriteProtection
- offer:update
- priceInquiry:update
- productCalculation:create
- productCalculation:delete
- productCalculation:read
- productCalculation:update
- production:create
- production:delete
- production:read
- production:release
- production:start
- production:update
- proformaInvoice:create
- proformaInvoice:delete
- proformaInvoice:read
- proformaInvoice:release
- proformaInvoice:removeWriteProtection
- proformaInvoice:send
- proformaInvoice:setWriteProtection
- proformaInvoice:update
- purchaseOrder:cancel
- purchaseOrder:complete
- purchaseOrder:create
- purchaseOrder:delete
- purchaseOrder:read
- purchaseOrder:release
- purchaseOrder:removeWriteProtection
- purchaseOrder:send
- purchaseOrder:setWriteProtection
- purchaseOrder:update
- return:cancel
- return:complete
- return:create
- return:delete
- return:read
- return:release
- return:removeWriteProtection
- return:send
- return:setWriteProtection
- return:update
- salesOrder:cancel
- salesOrder:complete
- salesOrder:create
- salesOrder:delete
- salesOrder:read
- salesOrder:release
- salesOrder:removeWriteProtection
- salesOrder:send
- salesOrder:setWriteProtection
- salesOrder:update
- salesPrice:create
- salesPrice:delete
- salesPrice:read
- salesPrice:update
- serviceOrder:update
- supplier:create
- supplier:delete
- supplier:read
- supplier:update
- supplierInvoice:update
scopes:
- description: Grants the create action on creditNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:create
- description: Grants the delete action on creditNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:delete
- description: Grants the read action on creditNote resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:read
- description: Grants the release action on creditNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:release
- description: Grants the removeWriteProtection action on creditNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:removeWriteProtection
- description: Grants the send action on creditNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:send
- description: Grants the setWriteProtection action on creditNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:setWriteProtection
- description: Grants the update action on creditNote resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: creditNote:update
- description: Grants the create action on customer resources (required by 2 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: customer:create
- description: Grants the delete action on customer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: customer:delete
- description: Grants the read action on customer resources (required by 6 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: customer:read
- description: Grants the update action on customer resources (required by 6 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: customer:update
- description: Grants the cancel action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:cancel
- description: Grants the complete action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:complete
- description: Grants the create action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:create
- description: Grants the delete action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:delete
- description: Grants the read action on deliveryNote resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:read
- description: Grants the release action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:release
- description: Grants the removeWriteProtection action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:removeWriteProtection
- description: Grants the send action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:send
- description: Grants the setWriteProtection action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:setWriteProtection
- description: Grants the update action on deliveryNote resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryNote:update
- description: Grants the create action on deliveryThreshold resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: deliveryThreshold:create
- description: Grants the create action on invoice resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:create
- description: Grants the delete action on invoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:delete
- description: Grants the read action on invoice resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:read
- description: Grants the release action on invoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:release
- description: Grants the removeWriteProtection action on invoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:removeWriteProtection
- description: Grants the send action on invoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:send
- description: Grants the setWriteProtection action on invoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:setWriteProtection
- description: Grants the update action on invoice resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: invoice:update
- description: Grants the sendEmail action on mailAcct resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: mailAcct:sendEmail
- description: Grants the cancel action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:cancel
- description: Grants the create action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:create
- description: Grants the delete action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:delete
- description: Grants the read action on offer resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:read
- description: Grants the release action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:release
- description: Grants the removeWriteProtection action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:removeWriteProtection
- description: Grants the send action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:send
- description: Grants the setWriteProtection action on offer resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:setWriteProtection
- description: Grants the update action on offer resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: offer:update
- description: Grants the update action on priceInquiry resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: priceInquiry:update
- description: Grants the create action on productCalculation resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: productCalculation:create
- description: Grants the delete action on productCalculation resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: productCalculation:delete
- description: Grants the read action on productCalculation resources (required by 2 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: productCalculation:read
- description: Grants the update action on productCalculation resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: productCalculation:update
- description: Grants the create action on production resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: production:create
- description: Grants the delete action on production resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: production:delete
- description: Grants the read action on production resources (required by 2 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: production:read
- description: Grants the release action on production resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: production:release
- description: Grants the start action on production resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: production:start
- description: Grants the update action on production resources (required by 4 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: production:update
- description: Grants the create action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:create
- description: Grants the delete action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:delete
- description: Grants the read action on proformaInvoice resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:read
- description: Grants the release action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:release
- description: Grants the removeWriteProtection action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:removeWriteProtection
- description: Grants the send action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:send
- description: Grants the setWriteProtection action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:setWriteProtection
- description: Grants the update action on proformaInvoice resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: proformaInvoice:update
- description: Grants the cancel action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:cancel
- description: Grants the complete action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:complete
- description: Grants the create action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:create
- description: Grants the delete action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:delete
- description: Grants the read action on purchaseOrder resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:read
- description: Grants the release action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:release
- description: Grants the removeWriteProtection action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:removeWriteProtection
- description: Grants the send action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:send
- description: Grants the setWriteProtection action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:setWriteProtection
- description: Grants the update action on purchaseOrder resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: purchaseOrder:update
- description: Grants the cancel action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:cancel
- description: Grants the complete action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:complete
- description: Grants the create action on return resources (required by 2 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:create
- description: Grants the delete action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:delete
- description: Grants the read action on return resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:read
- description: Grants the release action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:release
- description: Grants the removeWriteProtection action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:removeWriteProtection
- description: Grants the send action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:send
- description: Grants the setWriteProtection action on return resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:setWriteProtection
- description: Grants the update action on return resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: return:update
- description: Grants the cancel action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:cancel
- description: Grants the complete action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:complete
- description: Grants the create action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:create
- description: Grants the delete action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:delete
- description: Grants the read action on salesOrder resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:read
- description: Grants the release action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:release
- description: Grants the removeWriteProtection action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:removeWriteProtection
- description: Grants the send action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:send
- description: Grants the setWriteProtection action on salesOrder resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:setWriteProtection
- description: Grants the update action on salesOrder resources (required by 8 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesOrder:update
- description: Grants the create action on salesPrice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesPrice:create
- description: Grants the delete action on salesPrice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesPrice:delete
- description: Grants the read action on salesPrice resources (required by 2 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesPrice:read
- description: Grants the update action on salesPrice resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: salesPrice:update
- description: Grants the update action on serviceOrder resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: serviceOrder:update
- description: Grants the create action on supplier resources (required by 2 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: supplier:create
- description: Grants the delete action on supplier resources (required by 1 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: supplier:delete
- description: Grants the read action on supplier resources (required by 6 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: supplier:read
- description: Grants the update action on supplier resources (required by 6 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: supplier:update
- description: Grants the update action on supplierInvoice resources (required by 3 endpoint(s) in the Business Documents API v3).
  flows: []
  scope: supplierInvoice:update
slug: xentral-scopes
source_filename: xentral-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/xentral/api-spec-public (endpoint scope requirements documented per operation in the\n  official OpenAPI)\ndocs: https://developer.xentral.com/reference/authentication\nnotes: Xentral authenticates with Personal Access Tokens (Bearer). The Business Documents API v3 documents a required\n  scope per endpoint (resource:action form); the v1/v2 API documents no scopes. No oauth2 flows are declared in\n  the OpenAPI.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/xentral-api-openapi-original.json\n  - openapi/xentral-documents-api-openapi-original.json\nscopes:\n- scope: creditNote:create\n  description: Grants the create action on creditNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/creditNotes\n- scope: creditNote:delete\n  description: Grants the delete action on creditNote resources (required by 1 endpoint(s)\
  \ in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/creditNotes/{id}\n- scope: creditNote:read\n  description: Grants the read action on creditNote resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/creditNotes\n  - GET /api/v3/creditNotes/{id}\n  - GET /api/v3/creditNotes/{id}/lineItems/{lineItemId}\n- scope: creditNote:release\n  description: Grants the release action on creditNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/creditNotes/{id}/actions/release\n- scope: creditNote:removeWriteProtection\n  description: Grants the removeWriteProtection action on creditNote resources (required by 1 endpoint(s) in the\n    Business Documents API v3).\n  operations:\n  - PATCH /api/v3/creditNotes/{id}/actions/removeWriteProtection\n- scope: creditNote:send\n  description: Grants the send action on creditNote resources (required by 1 endpoint(s)\
  \ in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/creditNotes/{id}/actions/send\n- scope: creditNote:setWriteProtection\n  description: Grants the setWriteProtection action on creditNote resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/creditNotes/{id}/actions/setWriteProtection\n- scope: creditNote:update\n  description: Grants the update action on creditNote resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/creditNotes/{id}/files/{fileId}\n  - DELETE /api/v3/creditNotes/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/creditNotes/{id}\n  - PATCH /api/v3/creditNotes/{id}/actions/logActivity\n  - PATCH /api/v3/creditNotes/{id}/files/{fileId}\n  - PATCH /api/v3/creditNotes/{id}/lineItems/{lineItemId}\n  - POST /api/v3/creditNotes/{id}/files\n  - POST /api/v3/creditNotes/{id}/lineItems\n- scope: customer:create\n  description: Grants the create\
  \ action on customer resources (required by 2 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/customers\n  - POST /api/v3/customers/{customerId}/contactPersons\n- scope: customer:delete\n  description: Grants the delete action on customer resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/customers/{id}\n- scope: customer:read\n  description: Grants the read action on customer resources (required by 6 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/customers\n  - GET /api/v3/customers/{customerId}/contactPersons\n  - GET /api/v3/customers/{customerId}/contactPersons/{contactPersonId}\n  - GET /api/v3/customers/{customerId}/deliveryAddresses\n  - GET /api/v3/customers/{customerId}/deliveryAddresses/{deliveryAddressId}\n  - GET /api/v3/customers/{id}\n- scope: customer:update\n  description: Grants the update action on customer resources (required by 6 endpoint(s)\
  \ in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/customers/{customerId}/contactPersons/{contactPersonId}\n  - DELETE /api/v3/customers/{customerId}/deliveryAddresses/{deliveryAddressId}\n  - PATCH /api/v3/customers/{customerId}/contactPersons/{contactPersonId}\n  - PATCH /api/v3/customers/{customerId}/deliveryAddresses/{deliveryAddressId}\n  - PATCH /api/v3/customers/{id}\n  - POST /api/v3/customers/{customerId}/deliveryAddresses\n- scope: deliveryNote:cancel\n  description: Grants the cancel action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/deliveryNotes/{id}/actions/cancel\n- scope: deliveryNote:complete\n  description: Grants the complete action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/deliveryNotes/{id}/actions/complete\n- scope: deliveryNote:create\n  description: Grants the create action\
  \ on deliveryNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/deliveryNotes\n- scope: deliveryNote:delete\n  description: Grants the delete action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/deliveryNotes/{id}\n- scope: deliveryNote:read\n  description: Grants the read action on deliveryNote resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/deliveryNotes\n  - GET /api/v3/deliveryNotes/{id}\n  - GET /api/v3/deliveryNotes/{id}/lineItems/{lineItemId}\n- scope: deliveryNote:release\n  description: Grants the release action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/deliveryNotes/{id}/actions/release\n- scope: deliveryNote:removeWriteProtection\n  description: Grants the removeWriteProtection action on\
  \ deliveryNote resources (required by 1 endpoint(s) in the\n    Business Documents API v3).\n  operations:\n  - PATCH /api/v3/deliveryNotes/{id}/actions/removeWriteProtection\n- scope: deliveryNote:send\n  description: Grants the send action on deliveryNote resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/deliveryNotes/{id}/actions/send\n- scope: deliveryNote:setWriteProtection\n  description: Grants the setWriteProtection action on deliveryNote resources (required by 1 endpoint(s) in the\n    Business Documents API v3).\n  operations:\n  - PATCH /api/v3/deliveryNotes/{id}/actions/setWriteProtection\n- scope: deliveryNote:update\n  description: Grants the update action on deliveryNote resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/deliveryNotes/{id}/files/{fileId}\n  - DELETE /api/v3/deliveryNotes/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/deliveryNotes/{id}\n\
  \  - PATCH /api/v3/deliveryNotes/{id}/actions/logActivity\n  - PATCH /api/v3/deliveryNotes/{id}/files/{fileId}\n  - PATCH /api/v3/deliveryNotes/{id}/lineItems/{lineItemId}\n  - POST /api/v3/deliveryNotes/{id}/files\n  - POST /api/v3/deliveryNotes/{id}/lineItems\n- scope: deliveryThreshold:create\n  description: Grants the create action on deliveryThreshold resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - POST /api/v3/products/{productId}/deliveryThresholds\n- scope: invoice:create\n  description: Grants the create action on invoice resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/invoices\n  - POST /api/v3/invoices/actions/createFromDeliveryNote\n  - POST /api/v3/invoices/actions/createFromSalesOrder\n- scope: invoice:delete\n  description: Grants the delete action on invoice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE\
  \ /api/v3/invoices/{id}\n- scope: invoice:read\n  description: Grants the read action on invoice resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/invoices\n  - GET /api/v3/invoices/{id}\n  - GET /api/v3/invoices/{id}/lineItems/{lineItemId}\n- scope: invoice:release\n  description: Grants the release action on invoice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/invoices/{id}/actions/release\n- scope: invoice:removeWriteProtection\n  description: Grants the removeWriteProtection action on invoice resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/invoices/{id}/actions/removeWriteProtection\n- scope: invoice:send\n  description: Grants the send action on invoice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/invoices/{id}/actions/send\n- scope:\
  \ invoice:setWriteProtection\n  description: Grants the setWriteProtection action on invoice resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/invoices/{id}/actions/setWriteProtection\n- scope: invoice:update\n  description: Grants the update action on invoice resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/invoices/{id}/files/{fileId}\n  - DELETE /api/v3/invoices/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/invoices/{id}\n  - PATCH /api/v3/invoices/{id}/actions/logActivity\n  - PATCH /api/v3/invoices/{id}/files/{fileId}\n  - PATCH /api/v3/invoices/{id}/lineItems/{lineItemId}\n  - POST /api/v3/invoices/{id}/files\n  - POST /api/v3/invoices/{id}/lineItems\n- scope: mailAcct:sendEmail\n  description: Grants the sendEmail action on mailAcct resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/emailAccounts/{id}/actions/sendEmail\n\
  - scope: offer:cancel\n  description: Grants the cancel action on offer resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/offers/{id}/actions/cancel\n- scope: offer:create\n  description: Grants the create action on offer resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/offers\n- scope: offer:delete\n  description: Grants the delete action on offer resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/offers/{id}\n- scope: offer:read\n  description: Grants the read action on offer resources (required by 3 endpoint(s) in the Business Documents API\n    v3).\n  operations:\n  - GET /api/v3/offers\n  - GET /api/v3/offers/{id}\n  - GET /api/v3/offers/{id}/lineItems/{lineItemId}\n- scope: offer:release\n  description: Grants the release action on offer resources (required by 1 endpoint(s) in the Business Documents\n\
  \    API v3).\n  operations:\n  - PATCH /api/v3/offers/{id}/actions/release\n- scope: offer:removeWriteProtection\n  description: Grants the removeWriteProtection action on offer resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/offers/{id}/actions/removeWriteProtection\n- scope: offer:send\n  description: Grants the send action on offer resources (required by 1 endpoint(s) in the Business Documents API\n    v3).\n  operations:\n  - PATCH /api/v3/offers/{id}/actions/send\n- scope: offer:setWriteProtection\n  description: Grants the setWriteProtection action on offer resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/offers/{id}/actions/setWriteProtection\n- scope: offer:update\n  description: Grants the update action on offer resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/offers/{id}/files/{fileId}\n  -\
  \ DELETE /api/v3/offers/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/offers/{id}\n  - PATCH /api/v3/offers/{id}/actions/logActivity\n  - PATCH /api/v3/offers/{id}/files/{fileId}\n  - PATCH /api/v3/offers/{id}/lineItems/{lineItemId}\n  - POST /api/v3/offers/{id}/files\n  - POST /api/v3/offers/{id}/lineItems\n- scope: priceInquiry:update\n  description: Grants the update action on priceInquiry resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/priceInquiries/{id}/files/{fileId}\n  - PATCH /api/v3/priceInquiries/{id}/files/{fileId}\n  - POST /api/v3/priceInquiries/{id}/files\n- scope: productCalculation:create\n  description: Grants the create action on productCalculation resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - POST /api/v3/products/{id}/calculationItems\n- scope: productCalculation:delete\n  description: Grants the delete action on productCalculation resources (required\
  \ by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - DELETE /api/v3/products/{id}/calculationItems/{itemId}\n- scope: productCalculation:read\n  description: Grants the read action on productCalculation resources (required by 2 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - GET /api/v3/products/{id}/calculationItems\n  - GET /api/v3/products/{id}/calculationItems/{itemId}\n- scope: productCalculation:update\n  description: Grants the update action on productCalculation resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/products/{id}/calculationItems/{itemId}\n- scope: production:create\n  description: Grants the create action on production resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/productions\n- scope: production:delete\n  description: Grants the delete action on production resources (required by 1 endpoint(s)\
  \ in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/productions/{id}\n- scope: production:read\n  description: Grants the read action on production resources (required by 2 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/productions\n  - GET /api/v3/productions/{id}\n- scope: production:release\n  description: Grants the release action on production resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/productions/{id}/actions/release\n- scope: production:start\n  description: Grants the start action on production resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/productions/{id}/actions/start\n- scope: production:update\n  description: Grants the update action on production resources (required by 4 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/productions/{id}/files/{fileId}\n\
  \  - PATCH /api/v3/productions/{id}/actions/logActivity\n  - PATCH /api/v3/productions/{id}/files/{fileId}\n  - POST /api/v3/productions/{id}/files\n- scope: proformaInvoice:create\n  description: Grants the create action on proformaInvoice resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - POST /api/v3/proformaInvoices\n- scope: proformaInvoice:delete\n  description: Grants the delete action on proformaInvoice resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - DELETE /api/v3/proformaInvoices/{id}\n- scope: proformaInvoice:read\n  description: Grants the read action on proformaInvoice resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/proformaInvoices\n  - GET /api/v3/proformaInvoices/{id}\n  - GET /api/v3/proformaInvoices/{id}/lineItems/{lineItemId}\n- scope: proformaInvoice:release\n  description: Grants the release action on proformaInvoice\
  \ resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/proformaInvoices/{id}/actions/release\n- scope: proformaInvoice:removeWriteProtection\n  description: Grants the removeWriteProtection action on proformaInvoice resources (required by 1 endpoint(s) in\n    the Business Documents API v3).\n  operations:\n  - PATCH /api/v3/proformaInvoices/{id}/actions/removeWriteProtection\n- scope: proformaInvoice:send\n  description: Grants the send action on proformaInvoice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/proformaInvoices/{id}/actions/send\n- scope: proformaInvoice:setWriteProtection\n  description: Grants the setWriteProtection action on proformaInvoice resources (required by 1 endpoint(s) in the\n    Business Documents API v3).\n  operations:\n  - PATCH /api/v3/proformaInvoices/{id}/actions/setWriteProtection\n- scope: proformaInvoice:update\n  description: Grants\
  \ the update action on proformaInvoice resources (required by 8 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - DELETE /api/v3/proformaInvoices/{id}/files/{fileId}\n  - DELETE /api/v3/proformaInvoices/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/proformaInvoices/{id}\n  - PATCH /api/v3/proformaInvoices/{id}/actions/logActivity\n  - PATCH /api/v3/proformaInvoices/{id}/files/{fileId}\n  - PATCH /api/v3/proformaInvoices/{id}/lineItems/{lineItemId}\n  - POST /api/v3/proformaInvoices/{id}/files\n  - POST /api/v3/proformaInvoices/{id}/lineItems\n- scope: purchaseOrder:cancel\n  description: Grants the cancel action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/purchaseOrders/{id}/actions/cancel\n- scope: purchaseOrder:complete\n  description: Grants the complete action on purchaseOrder resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH\
  \ /api/v3/purchaseOrders/{id}/actions/complete\n- scope: purchaseOrder:create\n  description: Grants the create action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/purchaseOrders\n- scope: purchaseOrder:delete\n  description: Grants the delete action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/purchaseOrders/{id}\n- scope: purchaseOrder:read\n  description: Grants the read action on purchaseOrder resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/purchaseOrders\n  - GET /api/v3/purchaseOrders/{id}\n  - GET /api/v3/purchaseOrders/{id}/lineItems/{lineItemId}\n- scope: purchaseOrder:release\n  description: Grants the release action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/purchaseOrders/{id}/actions/release\n\
  - scope: purchaseOrder:removeWriteProtection\n  description: Grants the removeWriteProtection action on purchaseOrder resources (required by 1 endpoint(s) in\n    the Business Documents API v3).\n  operations:\n  - PATCH /api/v3/purchaseOrders/{id}/actions/removeWriteProtection\n- scope: purchaseOrder:send\n  description: Grants the send action on purchaseOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/purchaseOrders/{id}/actions/send\n- scope: purchaseOrder:setWriteProtection\n  description: Grants the setWriteProtection action on purchaseOrder resources (required by 1 endpoint(s) in the\n    Business Documents API v3).\n  operations:\n  - PATCH /api/v3/purchaseOrders/{id}/actions/setWriteProtection\n- scope: purchaseOrder:update\n  description: Grants the update action on purchaseOrder resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/purchaseOrders/{id}/files/{fileId}\n\
  \  - DELETE /api/v3/purchaseOrders/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/purchaseOrders/{id}\n  - PATCH /api/v3/purchaseOrders/{id}/actions/logActivity\n  - PATCH /api/v3/purchaseOrders/{id}/files/{fileId}\n  - PATCH /api/v3/purchaseOrders/{id}/lineItems/{lineItemId}\n  - POST /api/v3/purchaseOrders/{id}/files\n  - POST /api/v3/purchaseOrders/{id}/lineItems\n- scope: return:cancel\n  description: Grants the cancel action on return resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/returnOrders/{id}/actions/cancel\n- scope: return:complete\n  description: Grants the complete action on return resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/returnOrders/{id}/actions/complete\n- scope: return:create\n  description: Grants the create action on return resources (required by 2 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/returnOrders\n\
  \  - POST /api/v3/returnOrders/actions/createFromDeliveryNote\n- scope: return:delete\n  description: Grants the delete action on return resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/returnOrders/{id}\n- scope: return:read\n  description: Grants the read action on return resources (required by 3 endpoint(s) in the Business Documents API\n    v3).\n  operations:\n  - GET /api/v3/returnOrders\n  - GET /api/v3/returnOrders/{id}\n  - GET /api/v3/returnOrders/{id}/lineItems/{lineItemId}\n- scope: return:release\n  description: Grants the release action on return resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/returnOrders/{id}/actions/release\n- scope: return:removeWriteProtection\n  description: Grants the removeWriteProtection action on return resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/returnOrders/{id}/actions/removeWriteProtection\n\
  - scope: return:send\n  description: Grants the send action on return resources (required by 1 endpoint(s) in the Business Documents API\n    v3).\n  operations:\n  - PATCH /api/v3/returnOrders/{id}/actions/send\n- scope: return:setWriteProtection\n  description: Grants the setWriteProtection action on return resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/returnOrders/{id}/actions/setWriteProtection\n- scope: return:update\n  description: Grants the update action on return resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/returnOrders/{id}/files/{fileId}\n  - DELETE /api/v3/returnOrders/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/returnOrders/{id}\n  - PATCH /api/v3/returnOrders/{id}/actions/logActivity\n  - PATCH /api/v3/returnOrders/{id}/files/{fileId}\n  - PATCH /api/v3/returnOrders/{id}/lineItems/{lineItemId}\n  - POST /api/v3/returnOrders/{id}/files\n  -\
  \ POST /api/v3/returnOrders/{id}/lineItems\n- scope: salesOrder:cancel\n  description: Grants the cancel action on salesOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/salesOrders/{id}/actions/cancel\n- scope: salesOrder:complete\n  description: Grants the complete action on salesOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/salesOrders/{id}/actions/complete\n- scope: salesOrder:create\n  description: Grants the create action on salesOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/salesOrders\n- scope: salesOrder:delete\n  description: Grants the delete action on salesOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/salesOrders/{id}\n- scope: salesOrder:read\n  description: Grants the read action on salesOrder resources\
  \ (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/salesOrders\n  - GET /api/v3/salesOrders/{id}\n  - GET /api/v3/salesOrders/{id}/lineItems/{lineItemId}\n- scope: salesOrder:release\n  description: Grants the release action on salesOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/salesOrders/{id}/actions/release\n- scope: salesOrder:removeWriteProtection\n  description: Grants the removeWriteProtection action on salesOrder resources (required by 1 endpoint(s) in the\n    Business Documents API v3).\n  operations:\n  - PATCH /api/v3/salesOrders/{id}/actions/removeWriteProtection\n- scope: salesOrder:send\n  description: Grants the send action on salesOrder resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/salesOrders/{id}/actions/send\n- scope: salesOrder:setWriteProtection\n  description: Grants the setWriteProtection\
  \ action on salesOrder resources (required by 1 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - PATCH /api/v3/salesOrders/{id}/actions/setWriteProtection\n- scope: salesOrder:update\n  description: Grants the update action on salesOrder resources (required by 8 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/salesOrders/{id}/files/{fileId}\n  - DELETE /api/v3/salesOrders/{id}/lineItems/{lineItemId}\n  - PATCH /api/v3/salesOrders/{id}\n  - PATCH /api/v3/salesOrders/{id}/actions/logActivity\n  - PATCH /api/v3/salesOrders/{id}/files/{fileId}\n  - PATCH /api/v3/salesOrders/{id}/lineItems/{lineItemId}\n  - POST /api/v3/salesOrders/{id}/files\n  - POST /api/v3/salesOrders/{id}/lineItems\n- scope: salesPrice:create\n  description: Grants the create action on salesPrice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/salesPrices\n- scope: salesPrice:delete\n  description:\
  \ Grants the delete action on salesPrice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/salesPrices/{id}\n- scope: salesPrice:read\n  description: Grants the read action on salesPrice resources (required by 2 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/salesPrices\n  - GET /api/v3/salesPrices/{id}\n- scope: salesPrice:update\n  description: Grants the update action on salesPrice resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - PATCH /api/v3/salesPrices\n- scope: serviceOrder:update\n  description: Grants the update action on serviceOrder resources (required by 3 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/serviceOrders/{id}/files/{fileId}\n  - PATCH /api/v3/serviceOrders/{id}/files/{fileId}\n  - POST /api/v3/serviceOrders/{id}/files\n- scope: supplier:create\n  description: Grants the create action\
  \ on supplier resources (required by 2 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - POST /api/v3/suppliers\n  - POST /api/v3/suppliers/{supplierId}/contactPersons\n- scope: supplier:delete\n  description: Grants the delete action on supplier resources (required by 1 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/suppliers/{id}\n- scope: supplier:read\n  description: Grants the read action on supplier resources (required by 6 endpoint(s) in the Business Documents\n    API v3).\n  operations:\n  - GET /api/v3/suppliers\n  - GET /api/v3/suppliers/{id}\n  - GET /api/v3/suppliers/{supplierId}/contactPersons\n  - GET /api/v3/suppliers/{supplierId}/contactPersons/{contactPersonId}\n  - GET /api/v3/suppliers/{supplierId}/deliveryAddresses\n  - GET /api/v3/suppliers/{supplierId}/deliveryAddresses/{deliveryAddressId}\n- scope: supplier:update\n  description: Grants the update action on supplier resources (required by 6 endpoint(s)\
  \ in the Business Documents\n    API v3).\n  operations:\n  - DELETE /api/v3/suppliers/{supplierId}/contactPersons/{contactPersonId}\n  - DELETE /api/v3/suppliers/{supplierId}/deliveryAddresses/{deliveryAddressId}\n  - PATCH /api/v3/suppliers/{id}\n  - PATCH /api/v3/suppliers/{supplierId}/contactPersons/{contactPersonId}\n  - PATCH /api/v3/suppliers/{supplierId}/deliveryAddresses/{deliveryAddressId}\n  - POST /api/v3/suppliers/{supplierId}/deliveryAddresses\n- scope: supplierInvoice:update\n  description: Grants the update action on supplierInvoice resources (required by 3 endpoint(s) in the Business\n    Documents API v3).\n  operations:\n  - DELETE /api/v3/supplierInvoices/{id}/files/{fileId}\n  - PATCH /api/v3/supplierInvoices/{id}/files/{fileId}\n  - POST /api/v3/supplierInvoices/{id}/files\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xentral/refs/heads/main/scopes/xentral-scopes.yml
summary_line: 100 scopes
tags:
- Company
- ERP
- eCommerce
- Fulfillment
- Warehousing
- Invoicing
- Accounting
- Orders
- Products
- Germany
token_urls: []
---
