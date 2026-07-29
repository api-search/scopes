---
api_specs:
- filename: cdr-register-openapi.json
  format: json
  label: CDR Register API
  slug: cdr-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-register-openapi.json
- filename: cdr-energy-openapi.json
  format: json
  label: CDR Energy API
  slug: cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-energy-openapi.json
- filename: cdr-energy-sdh-openapi.json
  format: json
  label: CDR Energy Secondary Data Holder API
  slug: cdr-energy-secondary-data-holder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-energy-sdh-openapi.json
- filename: cdr-common-openapi.json
  format: json
  label: CDR Common API
  slug: cdr-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-common-openapi.json
- filename: cdr-dcr-openapi.json
  format: json
  label: CDR Dynamic Client Registration API
  slug: cdr-dynamic-client-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-dcr-openapi.json
- filename: cdr-admin-openapi.json
  format: json
  label: CDR Admin API
  slug: cdr-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/openapi/cdr-admin-openapi.json
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cdr Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Consumer Data Right (Energy) publishes 15 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Consumer Data Right (Energy) API on a user''s behalf.


  Tokens are issued from https://secure.api.cdr.gov.au/idp/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Consumer Data Right (Energy)
provider_slug: cdr-energy
schemes:
- flows:
  - client_authentication: private_key_jwt
    discovery: <data-holder>/.well-known/openid-configuration
    flow: authorizationCode
    note: Authorisation and token endpoints are per data holder; there are 84 registered energy brands. Discover them via the CDR Register data holder brands endpoint.
    pkce: required (S256)
    profile: FAPI 1.0 Advanced
    pushed_authorization_request: required
  name: CDR consumer authorisation (data holder)
  type: oauth2
- flows:
  - client_authentication: private_key_jwt
    flow: clientCredentials
    issuer: https://api.cdr.gov.au/idp
    sender_constrained: true
    source: well-known/cdr-energy-register-openid-configuration.json
    tokenUrl: https://secure.api.cdr.gov.au/idp/connect/token
  name: CDR Register OpenID Provider
  type: oauth2
scope_count: 15
scope_names:
- openid
- profile
- cdr-register:read
- admin:metrics.basic:read
- common:customer.basic:read
- common:customer.detail:read
- energy:accounts.basic:read
- energy:accounts.detail:read
- energy:accounts.paymentschedule:read
- energy:accounts.concessions:read
- energy:billing:read
- energy:electricity.servicepoints.basic:read
- energy:electricity.servicepoints.detail:read
- energy:electricity.usage:read
- energy:electricity.der:read
scopes:
- description: Mandatory OIDC scope; requests an ID token for the consumer authorisation.
  flows: []
  scope: openid
- description: Standard OIDC profile scope supported by the CDR federation.
  flows: []
  scope: profile
- description: Read access to CDR Register endpoints for accredited data recipients, obtained through the Register's own OpenID Provider using client_credentials and private_key_jwt.
  flows:
  - clientCredentials
  scope: cdr-register:read
- description: Scope used by the ACCC to call a data holder's GET /admin/metrics reporting endpoint.
  flows: []
  scope: admin:metrics.basic:read
- description: Access to personally identifiable information about the customer. For retail customers this is information about the customer themselves; for business customers it implies the name of a specific user plus information about the business. Includes name and occupation for individuals, or name, business numbers and industry code for organisations.
  flows: []
  scope: common:customer.basic:read
- description: More detailed information about the customer - everything in Basic Customer Data plus phone, email and address information.
  flows: []
  scope: common:customer.detail:read
- description: Basic information about the customer's energy accounts with retailers - simple energy account information, basic plan information and the service points that are part of the account. Does not include detailed account information such as tailored plans, electricity contract details or discounts.
  flows: []
  scope: energy:accounts.basic:read
- description: Detailed information about the customer's energy accounts. Additional authorisation on top of Basic Energy Account Data - includes tailored tariff information and charges included in the account or plan. Does not include usage data.
  flows: []
  scope: energy:accounts.detail:read
- description: Payment schedules for energy accounts, including direct debit or credit based scheduled payments and manual payments.
  flows: []
  scope: energy:accounts.paymentschedule:read
- description: Details of any concessions applied to a customer's energy account.
  flows: []
  scope: energy:accounts.concessions:read
- description: Billing and invoice data for a customer's energy account.
  flows: []
  scope: energy:billing:read
- description: Basic standing data for the customer's service points, including the National Meter Identifier (NMI). Does not include detailed service point information such as location or meter attributes.
  flows: []
  scope: energy:electricity.servicepoints.basic:read
- description: Detailed information about the customer's service point connection. Additional authorisation on top of Basic Service Point Data - includes account identifiers and meter information. Does not include meter usage data.
  flows: []
  scope: energy:electricity.servicepoints.detail:read
- description: Electricity usage data for service points, including basic and interval meter reads. Additional authorisation on top of Basic Service Point Data.
  flows: []
  scope: energy:electricity.usage:read
- description: Data about distributed energy resources for service points, as available in AEMO's DER Register. Additional authorisation on top of Basic Service Point Data.
  flows: []
  scope: energy:electricity.der:read
slug: cdr-energy-scopes
source_filename: cdr-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  The six OpenAPI documents in this repo declare no components.securitySchemes - the Consumer Data\n  Standards keep the security model in a separate normative Security Profile section rather than in\n  the API definitions - so the mechanical derive pass produced nothing. Every scope below was read\n  from the published Authorisation Scopes tables in the standards. Scopes are requested by an\n  accredited data recipient in the authorisation request and are granted by the consumer as part of a\n  time-bounded, revocable consent; the data holder maps them to the CDR consumer-facing data cluster\n  and permission language.\noperation_mapping_provenance: derived\noperation_mapping_note: >-\n  Scope names, display names, data clusters and descriptions\
  \ below are verbatim from the published\n  standards. The `operations:` list on each scope is DERIVED - it maps the published data cluster and\n  permission language onto the operationIds in this repo's OpenAPI files. The standards do not\n  publish a per-endpoint required-scope table for the energy endpoints; the exception is\n  admin:metrics.basic:read, which the Get Metrics endpoint documentation names explicitly. Treat the\n  operation lists as our reading of the contract, not as a normative DSB statement.\nschemes:\n- name: CDR consumer authorisation (data holder)\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    profile: FAPI 1.0 Advanced\n    pushed_authorization_request: required\n    pkce: required (S256)\n    client_authentication: private_key_jwt\n    discovery: <data-holder>/.well-known/openid-configuration\n    note: >-\n      Authorisation and token endpoints are per data holder; there are 84 registered energy brands.\n      Discover them via the CDR Register data\
  \ holder brands endpoint.\n- name: CDR Register OpenID Provider\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://secure.api.cdr.gov.au/idp/connect/token\n    issuer: https://api.cdr.gov.au/idp\n    client_authentication: private_key_jwt\n    sender_constrained: true\n    source: well-known/cdr-energy-register-openid-configuration.json\nscopes:\n- scope: openid\n  category: OpenID Connect\n  description: Mandatory OIDC scope; requests an ID token for the consumer authorisation.\n- scope: profile\n  category: OpenID Connect\n  description: Standard OIDC profile scope supported by the CDR federation.\n- scope: cdr-register:read\n  category: Register\n  description: >-\n    Read access to CDR Register endpoints for accredited data recipients, obtained through the\n    Register's own OpenID Provider using client_credentials and private_key_jwt.\n  flows: [clientCredentials]\n  source: well-known/cdr-energy-register-openid-configuration.json\n- scope: admin:metrics.basic:read\n\
  \  category: Admin\n  description: >-\n    Scope used by the ACCC to call a data holder's GET /admin/metrics reporting endpoint.\n  operations: [getMetrics]\n- scope: common:customer.basic:read\n  category: Common\n  name: Basic Customer Data\n  description: >-\n    Access to personally identifiable information about the customer. For retail customers this is\n    information about the customer themselves; for business customers it implies the name of a\n    specific user plus information about the business. Includes name and occupation for individuals,\n    or name, business numbers and industry code for organisations.\n  operations: [getCustomer]\n- scope: common:customer.detail:read\n  category: Common\n  name: Detailed Customer Data\n  description: >-\n    More detailed information about the customer - everything in Basic Customer Data plus phone,\n    email and address information.\n  operations: [getCustomerDetail]\n- scope: energy:accounts.basic:read\n  category: Energy\n  name:\
  \ Basic Energy Account Data\n  data_cluster: Accounts and plans\n  description: >-\n    Basic information about the customer's energy accounts with retailers - simple energy account\n    information, basic plan information and the service points that are part of the account. Does not\n    include detailed account information such as tailored plans, electricity contract details or\n    discounts.\n  operations: [listEnergyAccounts, getEnergyAccountBalance, listEnergyAccountBalancesBulk, listEnergyAccountBalancesSpecificAccounts]\n- scope: energy:accounts.detail:read\n  category: Energy\n  name: Detailed Energy Account Data\n  data_cluster: Account and plan details\n  description: >-\n    Detailed information about the customer's energy accounts. Additional authorisation on top of\n    Basic Energy Account Data - includes tailored tariff information and charges included in the\n    account or plan. Does not include usage data.\n  operations: [getEnergyAccountDetail]\n- scope: energy:accounts.paymentschedule:read\n\
  \  category: Energy\n  name: Energy Regular Payments Data\n  description: >-\n    Payment schedules for energy accounts, including direct debit or credit based scheduled payments\n    and manual payments.\n  operations: [getEnergyAccountPaymentSchedule]\n- scope: energy:accounts.concessions:read\n  category: Energy\n  name: Energy Concession Data\n  description: Details of any concessions applied to a customer's energy account.\n  operations: [getEnergyAccountConcessions]\n- scope: energy:billing:read\n  category: Energy\n  name: Energy Billing Data\n  description: Billing and invoice data for a customer's energy account.\n  operations: [getEnergyAccountInvoices, listEnergyAccountInvoicesBulk, listEnergyInvoicesForSpecificAccounts, getBillingForEnergyAccount, listEnergyAccountBillingBulk, listEnergyAccountBillingForSpecificAccounts]\n- scope: energy:electricity.servicepoints.basic:read\n  category: Energy\n  name: Basic Service Point Data\n  description: >-\n    Basic standing data for\
  \ the customer's service points, including the National Meter Identifier\n    (NMI). Does not include detailed service point information such as location or meter attributes.\n  operations: [listElectricityServicePoints, listElectricityServicePointsSR]\n- scope: energy:electricity.servicepoints.detail:read\n  category: Energy\n  name: Detailed Service Point Data\n  description: >-\n    Detailed information about the customer's service point connection. Additional authorisation on\n    top of Basic Service Point Data - includes account identifiers and meter information. Does not\n    include meter usage data.\n  operations: [getElectricityServicePointDetail, getElectricityServicePointDetailSR]\n- scope: energy:electricity.usage:read\n  category: Energy\n  name: Electricity Usage Data\n  description: >-\n    Electricity usage data for service points, including basic and interval meter reads. Additional\n    authorisation on top of Basic Service Point Data.\n  operations: [getElectricityServicePointUsage,\
  \ listElectricityUsageBulk, listElectricityUsageForServicePoints, getElectricityServicePointUsageSR, listElectricityUsageForServicePointsSR]\n- scope: energy:electricity.der:read\n  category: Energy\n  name: Distributed Energy Resource Data\n  description: >-\n    Data about distributed energy resources for service points, as available in AEMO's DER Register.\n    Additional authorisation on top of Basic Service Point Data.\n  operations: [getElectricityDERForServicePoint, listElectricityDERBulk, listElectricityDERForSpecificServicePoints, getElectricityDERForServicePointSR, listElectricityDERForSpecificServicePointsSR]\nunauthenticated_operations:\n  note: >-\n    These operations are part of the mandated contract but sit outside the consent model entirely -\n    no scope, no token, no accreditation.\n  operations: [listEnergyPlans, getEnergyPlanDetail, getStatus, getOutages, getDataHolderBrands, getDataHolderBrandsSummary, getDataHolderStatuses, getDataRecipients, getDataRecipientsStatuses,\
  \ getSoftwareProductsStatuses, getRegisterJwks, getRegisterOpenIdProviderConfig]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdr-energy/refs/heads/main/scopes/cdr-energy-scopes.yml
summary_line: 15 scopes · authorizationCode/clientCredentials
tags:
- Energy
- Australia
- Utilities
- Electricity
- Consumer Data Right
- Open Energy
- Smart Metering
- DER
- Energy Markets
- Regulation
- Government
- Open Data
token_urls:
- https://secure.api.cdr.gov.au/idp/connect/token
---
