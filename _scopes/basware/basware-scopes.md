---
api_specs:
- filename: api-reference
  format: yaml
  label: Basware P2P API
  slug: basware-p2p-api
  spec_type: OpenAPI
  url: https://developer.basware.com/en/api/basware/api-reference
- filename: api-reference
  format: yaml
  label: Basware Network API
  slug: basware-network-api
  spec_type: OpenAPI
  url: https://developer.basware.com/en/api/network/api-reference
- filename: basware-vault-openapi.yaml
  format: yaml
  label: Basware Vault API
  slug: basware-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basware/refs/heads/main/openapi/basware-vault-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Basware Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Basware publishes 86 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Basware API on a user''s behalf.


  Tokens are issued from https://api.basware.com/v1/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Basware
provider_slug: basware
schemes:
- description: Oauth2 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.basware.com/v1/tokens
  name: oauth2authentication
  source: openapi/basware-p2p-openapi.json
- description: OAuth2 client credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.basware.com/v1/tokens
  name: oauth2authentication
  source: openapi/basware-user-permission-openapi.json
scope_count: 86
scope_names:
- accountingDocuments.delete
- accountingDocuments.read
- accountingDocuments.write
- accounts.delete
- accounts.read
- accounts.write
- advancedPermissions.delete
- advancedPermissions.read
- advancedPermissions.write
- advancedValidations.delete
- advancedValidations.read
- advancedValidations.write
- applicationGroups.read
- applicationGroups.write
- companies.read
- companies.write
- contracts.delete
- contracts.read
- contracts.write
- costCenters.delete
- costCenters.read
- costCenters.write
- errorFeedbacks.delete
- errorFeedbacks.read
- errorFeedbacks.write
- exchangeRates.delete
- exchangeRates.read
- exchangeRates.write
- exportedContractSpends.delete
- exportedContractSpends.read
- exportedContractSpends.write
- exportedContracts.delete
- exportedContracts.read
- exportedContracts.write
- exportedPurchaseOrders.delete
- exportedPurchaseOrders.read
- exportedPurchaseOrders.write
- exportedPurchaseRequisitions.delete
- exportedPurchaseRequisitions.read
- exportedPurchaseRequisitions.write
- lists.delete
- lists.read
- lists.write
- matchingOrderLines.delete
- matchingOrderLines.read
- matchingOrderLines.write
- matchingOrders.delete
- matchingOrders.read
- matchingOrders.write
- paymentTerms.delete
- paymentTerms.read
- paymentTerms.write
- projects.delete
- projects.read
- projects.write
- purchaseGoodsReceipts.delete
- purchaseGoodsReceipts.read
- purchaseGoodsReceipts.write
- purchaseOrders.delete
- purchaseOrders.read
- purchaseOrders.write
- purchaseRequisitions.delete
- purchaseRequisitions.read
- purchaseRequisitions.write
- requestStatus.read
- requestStatus.write
- subscriptions.delete
- subscriptions.read
- subscriptions.write
- taskStatus.read
- tasks.read
- taxCodes.delete
- taxCodes.read
- taxCodes.write
- userGroupAssociatedUsers.delete
- userGroupAssociatedUsers.read
- userGroupAssociatedUsers.write
- userGroups.delete
- userGroups.read
- userGroups.write
- users.delete
- users.read
- users.write
- vendors.delete
- vendors.read
- vendors.write
scopes:
- description: DELETE accountingDocuments
  flows:
  - clientCredentials
  scope: accountingDocuments.delete
- description: GET accountingDocuments
  flows:
  - clientCredentials
  scope: accountingDocuments.read
- description: POST/PATCH accountingDocuments
  flows:
  - clientCredentials
  scope: accountingDocuments.write
- description: DELETE accounts
  flows:
  - clientCredentials
  scope: accounts.delete
- description: GET accounts
  flows:
  - clientCredentials
  scope: accounts.read
- description: POST/PATCH accounts
  flows:
  - clientCredentials
  scope: accounts.write
- description: DELETE advancedPermissions
  flows:
  - clientCredentials
  scope: advancedPermissions.delete
- description: GET advancedPermissions
  flows:
  - clientCredentials
  scope: advancedPermissions.read
- description: POST/PATCH advancedPermissions
  flows:
  - clientCredentials
  scope: advancedPermissions.write
- description: DELETE advancedValidations
  flows:
  - clientCredentials
  scope: advancedValidations.delete
- description: GET advancedValidations
  flows:
  - clientCredentials
  scope: advancedValidations.read
- description: POST/PATCH advancedValidations
  flows:
  - clientCredentials
  scope: advancedValidations.write
- description: GET applicationGroups
  flows:
  - clientCredentials
  scope: applicationGroups.read
- description: POST/PATCH applicationGroups
  flows:
  - clientCredentials
  scope: applicationGroups.write
- description: GET companies
  flows:
  - clientCredentials
  scope: companies.read
- description: POST/PATCH companies
  flows:
  - clientCredentials
  scope: companies.write
- description: DELETE contracts
  flows:
  - clientCredentials
  scope: contracts.delete
- description: GET contracts
  flows:
  - clientCredentials
  scope: contracts.read
- description: POST/PATCH contracts
  flows:
  - clientCredentials
  scope: contracts.write
- description: DELETE costCenters
  flows:
  - clientCredentials
  scope: costCenters.delete
- description: GET costCenters
  flows:
  - clientCredentials
  scope: costCenters.read
- description: POST/PATCH costCenters
  flows:
  - clientCredentials
  scope: costCenters.write
- description: DELETE errorFeedbacks
  flows:
  - clientCredentials
  scope: errorFeedbacks.delete
- description: GET errorFeedbacks
  flows:
  - clientCredentials
  scope: errorFeedbacks.read
- description: POST/PATCH errorFeedbacks
  flows:
  - clientCredentials
  scope: errorFeedbacks.write
- description: DELETE exchangeRates
  flows:
  - clientCredentials
  scope: exchangeRates.delete
- description: GET exchangeRates
  flows:
  - clientCredentials
  scope: exchangeRates.read
- description: POST/PATCH exchangeRates
  flows:
  - clientCredentials
  scope: exchangeRates.write
- description: DELETE exportedContractSpends
  flows:
  - clientCredentials
  scope: exportedContractSpends.delete
- description: GET exportedContractSpends
  flows:
  - clientCredentials
  scope: exportedContractSpends.read
- description: POST/PATCH exportedContractSpends
  flows:
  - clientCredentials
  scope: exportedContractSpends.write
- description: DELETE exportedContracts
  flows:
  - clientCredentials
  scope: exportedContracts.delete
- description: GET exportedContracts
  flows:
  - clientCredentials
  scope: exportedContracts.read
- description: POST/PATCH exportedContracts
  flows:
  - clientCredentials
  scope: exportedContracts.write
- description: DELETE exportedPurchaseOrders
  flows:
  - clientCredentials
  scope: exportedPurchaseOrders.delete
- description: GET exportedPurchaseOrders
  flows:
  - clientCredentials
  scope: exportedPurchaseOrders.read
- description: POST/PATCH exportedPurchaseOrders
  flows:
  - clientCredentials
  scope: exportedPurchaseOrders.write
- description: DELETE exportedPurchaseRequisitions
  flows:
  - clientCredentials
  scope: exportedPurchaseRequisitions.delete
- description: GET exportedPurchaseRequisitions
  flows:
  - clientCredentials
  scope: exportedPurchaseRequisitions.read
- description: POST/PATCH exportedPurchaseRequisitions
  flows:
  - clientCredentials
  scope: exportedPurchaseRequisitions.write
- description: DELETE lists
  flows:
  - clientCredentials
  scope: lists.delete
- description: GET lists
  flows:
  - clientCredentials
  scope: lists.read
- description: POST/PATCH lists
  flows:
  - clientCredentials
  scope: lists.write
- description: DELETE matchingOrderLines
  flows:
  - clientCredentials
  scope: matchingOrderLines.delete
- description: GET matchingOrderLines
  flows:
  - clientCredentials
  scope: matchingOrderLines.read
- description: POST/PATCH matchingOrderLines
  flows:
  - clientCredentials
  scope: matchingOrderLines.write
- description: DELETE matchingOrders
  flows:
  - clientCredentials
  scope: matchingOrders.delete
- description: GET matchingOrders
  flows:
  - clientCredentials
  scope: matchingOrders.read
- description: POST/PATCH matchingOrders
  flows:
  - clientCredentials
  scope: matchingOrders.write
- description: DELETE paymentTerms
  flows:
  - clientCredentials
  scope: paymentTerms.delete
- description: GET paymentTerms
  flows:
  - clientCredentials
  scope: paymentTerms.read
- description: POST/PATCH paymentTerms
  flows:
  - clientCredentials
  scope: paymentTerms.write
- description: DELETE projects
  flows:
  - clientCredentials
  scope: projects.delete
- description: GET projects
  flows:
  - clientCredentials
  scope: projects.read
- description: POST/PATCH projects
  flows:
  - clientCredentials
  scope: projects.write
- description: DELETE purchaseGoodsReceipts
  flows:
  - clientCredentials
  scope: purchaseGoodsReceipts.delete
- description: GET purchaseGoodsReceipts
  flows:
  - clientCredentials
  scope: purchaseGoodsReceipts.read
- description: POST/PATCH purchaseGoodsReceipts
  flows:
  - clientCredentials
  scope: purchaseGoodsReceipts.write
- description: DELETE purchaseOrders
  flows:
  - clientCredentials
  scope: purchaseOrders.delete
- description: GET purchaseOrders
  flows:
  - clientCredentials
  scope: purchaseOrders.read
- description: POST/PATCH purchaseOrders
  flows:
  - clientCredentials
  scope: purchaseOrders.write
- description: DELETE purchaseRequisitions
  flows:
  - clientCredentials
  scope: purchaseRequisitions.delete
- description: GET purchaseRequisitions
  flows:
  - clientCredentials
  scope: purchaseRequisitions.read
- description: POST/PATCH purchaseRequisitions
  flows:
  - clientCredentials
  scope: purchaseRequisitions.write
- description: GET requestStatus
  flows:
  - clientCredentials
  scope: requestStatus.read
- description: POST/PATCH requestStatus
  flows:
  - clientCredentials
  scope: requestStatus.write
- description: DELETE subscriptions
  flows:
  - clientCredentials
  scope: subscriptions.delete
- description: GET subscriptions
  flows:
  - clientCredentials
  scope: subscriptions.read
- description: POST/PATCH subscriptions
  flows:
  - clientCredentials
  scope: subscriptions.write
- description: GET taskStatus
  flows:
  - clientCredentials
  scope: taskStatus.read
- description: GET tasks
  flows:
  - clientCredentials
  scope: tasks.read
- description: DELETE taxCodes
  flows:
  - clientCredentials
  scope: taxCodes.delete
- description: GET taxCodes
  flows:
  - clientCredentials
  scope: taxCodes.read
- description: POST/PATCH taxCodes
  flows:
  - clientCredentials
  scope: taxCodes.write
- description: DELETE user associations from user group
  flows:
  - clientCredentials
  scope: userGroupAssociatedUsers.delete
- description: GET user associations with user group
  flows:
  - clientCredentials
  scope: userGroupAssociatedUsers.read
- description: POST user associations to user group
  flows:
  - clientCredentials
  scope: userGroupAssociatedUsers.write
- description: DELETE user groups
  flows:
  - clientCredentials
  scope: userGroups.delete
- description: GET user groups
  flows:
  - clientCredentials
  scope: userGroups.read
- description: POST user groups
  flows:
  - clientCredentials
  scope: userGroups.write
- description: DELETE users
  flows:
  - clientCredentials
  scope: users.delete
- description: GET users
  flows:
  - clientCredentials
  scope: users.read
- description: POST/PATCH users
  flows:
  - clientCredentials
  scope: users.write
- description: DELETE vendors
  flows:
  - clientCredentials
  scope: vendors.delete
- description: GET vendors
  flows:
  - clientCredentials
  scope: vendors.read
- description: POST/PATCH vendors
  flows:
  - clientCredentials
  scope: vendors.write
slug: basware-scopes
source_filename: basware-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basware-p2p-openapi.json, openapi/basware-user-permission-openapi.json\nschemes:\n- name: oauth2authentication\n  source: openapi/basware-p2p-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.basware.com/v1/tokens\n  description: Oauth2 client credentials flow.\n- name: oauth2authentication\n  source: openapi/basware-user-permission-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.basware.com/v1/tokens\n  description: OAuth2 client credentials flow.\nscopes:\n- scope: accountingDocuments.delete\n  description: DELETE accountingDocuments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: accountingDocuments.read\n  description: GET accountingDocuments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: accountingDocuments.write\n  description: POST/PATCH accountingDocuments\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: accounts.delete\n  description: DELETE accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: accounts.read\n  description: GET accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: accounts.write\n  description: POST/PATCH accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: advancedPermissions.delete\n  description: DELETE advancedPermissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: advancedPermissions.read\n  description: GET advancedPermissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: advancedPermissions.write\n  description: POST/PATCH advancedPermissions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: advancedValidations.delete\n\
  \  description: DELETE advancedValidations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: advancedValidations.read\n  description: GET advancedValidations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: advancedValidations.write\n  description: POST/PATCH advancedValidations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: applicationGroups.read\n  description: GET applicationGroups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: applicationGroups.write\n  description: POST/PATCH applicationGroups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: companies.read\n  description: GET companies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: companies.write\n  description: POST/PATCH companies\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: contracts.delete\n  description: DELETE contracts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: contracts.read\n  description: GET contracts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: contracts.write\n  description: POST/PATCH contracts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: costCenters.delete\n  description: DELETE costCenters\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: costCenters.read\n  description: GET costCenters\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: costCenters.write\n  description: POST/PATCH costCenters\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: errorFeedbacks.delete\n  description: DELETE errorFeedbacks\n  flows:\n  -\
  \ clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: errorFeedbacks.read\n  description: GET errorFeedbacks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: errorFeedbacks.write\n  description: POST/PATCH errorFeedbacks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exchangeRates.delete\n  description: DELETE exchangeRates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exchangeRates.read\n  description: GET exchangeRates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exchangeRates.write\n  description: POST/PATCH exchangeRates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedContractSpends.delete\n  description: DELETE exportedContractSpends\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope:\
  \ exportedContractSpends.read\n  description: GET exportedContractSpends\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedContractSpends.write\n  description: POST/PATCH exportedContractSpends\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedContracts.delete\n  description: DELETE exportedContracts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedContracts.read\n  description: GET exportedContracts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedContracts.write\n  description: POST/PATCH exportedContracts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedPurchaseOrders.delete\n  description: DELETE exportedPurchaseOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedPurchaseOrders.read\n\
  \  description: GET exportedPurchaseOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedPurchaseOrders.write\n  description: POST/PATCH exportedPurchaseOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedPurchaseRequisitions.delete\n  description: DELETE exportedPurchaseRequisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedPurchaseRequisitions.read\n  description: GET exportedPurchaseRequisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: exportedPurchaseRequisitions.write\n  description: POST/PATCH exportedPurchaseRequisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: lists.delete\n  description: DELETE lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: lists.read\n  description:\
  \ GET lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: lists.write\n  description: POST/PATCH lists\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: matchingOrderLines.delete\n  description: DELETE matchingOrderLines\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: matchingOrderLines.read\n  description: GET matchingOrderLines\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: matchingOrderLines.write\n  description: POST/PATCH matchingOrderLines\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: matchingOrders.delete\n  description: DELETE matchingOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: matchingOrders.read\n  description: GET matchingOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n\
  - scope: matchingOrders.write\n  description: POST/PATCH matchingOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: paymentTerms.delete\n  description: DELETE paymentTerms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: paymentTerms.read\n  description: GET paymentTerms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: paymentTerms.write\n  description: POST/PATCH paymentTerms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: projects.delete\n  description: DELETE projects\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: projects.read\n  description: GET projects\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: projects.write\n  description: POST/PATCH projects\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n\
  - scope: purchaseGoodsReceipts.delete\n  description: DELETE purchaseGoodsReceipts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseGoodsReceipts.read\n  description: GET purchaseGoodsReceipts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseGoodsReceipts.write\n  description: POST/PATCH purchaseGoodsReceipts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseOrders.delete\n  description: DELETE purchaseOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseOrders.read\n  description: GET purchaseOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseOrders.write\n  description: POST/PATCH purchaseOrders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseRequisitions.delete\n  description:\
  \ DELETE purchaseRequisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseRequisitions.read\n  description: GET purchaseRequisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: purchaseRequisitions.write\n  description: POST/PATCH purchaseRequisitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: requestStatus.read\n  description: GET requestStatus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: requestStatus.write\n  description: POST/PATCH requestStatus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: subscriptions.delete\n  description: DELETE subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: subscriptions.read\n  description: GET subscriptions\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/basware-p2p-openapi.json\n- scope: subscriptions.write\n  description: POST/PATCH subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: taskStatus.read\n  description: GET taskStatus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: tasks.read\n  description: GET tasks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: taxCodes.delete\n  description: DELETE taxCodes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: taxCodes.read\n  description: GET taxCodes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: taxCodes.write\n  description: POST/PATCH taxCodes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: userGroupAssociatedUsers.delete\n  description: DELETE user associations from user group\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/basware-user-permission-openapi.json\n- scope: userGroupAssociatedUsers.read\n  description: GET user associations with user group\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-user-permission-openapi.json\n- scope: userGroupAssociatedUsers.write\n  description: POST user associations to user group\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-user-permission-openapi.json\n- scope: userGroups.delete\n  description: DELETE user groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-user-permission-openapi.json\n- scope: userGroups.read\n  description: GET user groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-user-permission-openapi.json\n- scope: userGroups.write\n  description: POST user groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-user-permission-openapi.json\n- scope: users.delete\n  description: DELETE users\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/basware-p2p-openapi.json\n- scope: users.read\n  description: GET users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: users.write\n  description: POST/PATCH users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: vendors.delete\n  description: DELETE vendors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: vendors.read\n  description: GET vendors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n- scope: vendors.write\n  description: POST/PATCH vendors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basware-p2p-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basware/refs/heads/main/scopes/basware-scopes.yml
summary_line: 86 scopes · clientCredentials
tags:
- E-Invoicing
- Purchase-to-Pay
- Accounts Payable
- Procurement
- Electronic Invoicing
- Finance Automation
- B2B Payments
token_urls:
- https://api.basware.com/v1/tokens
---
