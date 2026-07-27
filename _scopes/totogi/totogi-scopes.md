---
authorization_urls: []
description: ''
docs: https://docs.api.totogi.com/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Totogi Scopes
name_suffix: OAuth Scopes
note: Totogi CaaS does not expose OAuth scope strings in its public reference. Authorization is expressed as NAMED ROLES, published per operation as "Authorized Roles" in the GraphQL reference, and carried on the OAuth 2.0 client-credentials token minted for a tenant client. The roles below are transcribed verbatim from the published per-operation authorization statements.
overview: 'Totogi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://oauth.totogi.io/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Totogi
provider_slug: totogi
schemes:
- flows:
  - flow: clientCredentials
    note: Scope value is transcribed verbatim from Totogi's own published demo client; it reads as an AWS Cognito resource-server identifier and is very likely environment-specific. No canonical scope reference page is published.
    scope_example: https://myresourceserver1.com/marketplace
    tokenUrl: https://oauth.totogi.io/oauth2/token
  name: OAuth2 client credentials
  source: https://github.com/totogi/marketplace-api-demo (Totogi-published demo)
scope_count: 0
scope_names: []
scopes: []
slug: totogi-scopes
source_filename: totogi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://docs.api.totogi.com/\ndocs: https://docs.api.totogi.com/\nmodel: named-roles\nnote: Totogi CaaS does not expose OAuth scope strings in its public reference. Authorization is expressed\n  as NAMED ROLES, published per operation as \"Authorized Roles\" in the GraphQL reference, and carried\n  on the OAuth 2.0 client-credentials token minted for a tenant client. The roles below are transcribed\n  verbatim from the published per-operation authorization statements.\nschemes:\n- name: OAuth2 client credentials\n  source: https://github.com/totogi/marketplace-api-demo (Totogi-published demo)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.totogi.io/oauth2/token\n    scope_example: https://myresourceserver1.com/marketplace\n    note: Scope value is transcribed verbatim from Totogi's own published demo client; it reads as an\n      AWS Cognito resource-server identifier and is very likely environment-specific.\
  \ No canonical scope\n      reference page is published.\nroles:\n- role: Plan_Designer\n  operations: 29\n  sample_operations:\n  - mutation.archivePlanVersion\n  - mutation.createPlan\n  - mutation.createPlanFromInitialRecurringFirstUsageTemplate\n  - mutation.createPlanFromInitialTemplate\n  - mutation.createPlanVersionFromInitialRecurringFirstUsageTemplate\n  - mutation.createPlanVersionFromInitialTemplate\n- role: Plan_Admin\n  operations: 24\n  sample_operations:\n  - mutation.createBalanceType\n  - mutation.createLifecycle\n  - mutation.createPolicyCounter\n  - mutation.deleteBalanceType\n  - mutation.deleteBalanceTypeCounter\n  - mutation.deleteLifecycle\n- role: Account_Admin\n  operations: 20\n  sample_operations:\n  - mutation.cancelPlanSubscription\n  - mutation.createAccount\n  - mutation.createBalance\n  - mutation.createDevice\n  - mutation.deleteAccount\n  - mutation.deleteAccountBalanceTypeCounter\n- role: Plan_Publisher\n  operations: 20\n  sample_operations:\n  - mutation.deployPlan\n\
  \  - mutation.makePlanAssignable\n  - query.getBalanceType\n  - query.getBalanceTypeCounters\n  - query.getBalanceTypes\n  - query.getDeployedFieldMappings\n- role: Plan_Query\n  operations: 18\n  sample_operations:\n  - query.getBalanceType\n  - query.getBalanceTypeCounters\n  - query.getBalanceTypes\n  - query.getDeployedFieldMappings\n  - query.getFieldMappings\n  - query.getLifecycle\n- role: Tenant_Admin\n  operations: 15\n  sample_operations:\n  - mutation.createClientCredentials\n  - mutation.createUser\n  - mutation.deleteClientCredentials\n  - mutation.deleteUser\n  - mutation.resetUserPassword\n  - mutation.updateArchivingPolicy\n- role: Network_Admin\n  operations: 15\n  sample_operations:\n  - mutation.createQoSProfile\n  - mutation.deleteQoSProfile\n  - mutation.deployFieldMappings\n  - mutation.updateMyProviderConfig\n  - mutation.updateQoSProfile\n  - mutation.updateRatingGroupHierarchy\n- role: Network_Operator\n  operations: 8\n  sample_operations:\n  - mutation.createFieldMapping\n\
  \  - mutation.deleteFieldMapping\n  - mutation.updateFieldMapping\n  - mutation.updateSGSNTable\n  - query.getDeployedFieldMappings\n  - query.getFieldMappings\n- role: Data_Admin\n  operations: 7\n  sample_operations:\n  - query.getAccount\n  - query.getAccountBalanceTypeCounters\n  - query.getDevice\n  - query.getEventDataRecordsByAccount\n  - query.getEventDataRecordsByDevice\n  - query.getMyProviderConfig\n- role: Account_Query\n  operations: 5\n  sample_operations:\n  - query.getAccount\n  - query.getAccountBalanceTypeCounters\n  - query.getDevice\n  - query.getMyProviderConfig\n  - query.getRelatedAccountsByDevice\n- role: All\n  operations: 2\n  sample_operations:\n  - mutation.updateUserProfile\n  - query.getCurrentUser\n- role: Dashboard_Reader\n  operations: 1\n  sample_operations:\n  - query.getMyDashboard\n- role: Product_Admin\n  operations: 1\n  sample_operations:\n  - mutation.exportCustomerDB\n- role: System_Admin\n  operations: 1\n  sample_operations:\n  - mutation.exportCustomerDB\n\
  - role: Infrastructure\n  operations: 1\n  sample_operations:\n  - mutation.triggerRar\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/totogi/refs/heads/main/scopes/totogi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Telecommunications
- United States
- BSS
- OSS
- Charging
- Messaging
- SMS
- A2P
- 5G
- TM Forum
- Standards
- Network Vendor
- Vertical AI
- GraphQL
- Policy Control
token_urls:
- https://oauth.totogi.io/oauth2/token
---
