---
api_specs:
- filename: simply-energy-cds-energy-openapi.yml
  format: yaml
  label: Simply Energy (ENGIE) CDR Energy Generic Plans API
  slug: simply-energy-cdr-energy-generic-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-cds-energy-openapi.yml
- filename: simply-energy-cds-common-openapi.yml
  format: yaml
  label: Simply Energy (ENGIE) CDR Discovery API
  slug: simply-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-cds-common-openapi.yml
- filename: simply-energy-cds-energy-openapi.yml
  format: yaml
  label: Simply Energy (ENGIE) CDR Energy Consumer Data API
  slug: simply-energy-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-cds-energy-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Simply Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Simply Energy publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Simply Energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Simply Energy
provider_slug: simply-energy
schemes:
- flows:
  - authorizationUrl: null
    flow: authorizationCode
    note: 'The authorisation and token endpoints of an energy data holder are published only via

      the authenticated portion of the CDR Register and are not anonymously discoverable.

      See authentication/simply-energy-authentication.yml.

      '
    tokenUrl: null
  name: CDR Security Profile (OAuth 2.0 + OpenID Connect, FAPI 1.0 Advanced)
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
scope_count: 13
scope_names:
- openid
- profile
- common:customer.basic:read
- common:customer.detail:read
- energy:accounts.basic:read
- energy:accounts.detail:read
- energy:accounts.concessions:read
- energy:accounts.paymentschedule:read
- energy:billing:read
- energy:electricity.servicepoints.basic:read
- energy:electricity.servicepoints.detail:read
- energy:electricity.usage:read
- energy:electricity.der:read
scopes:
- description: Required OpenID Connect scope. Establishes the authenticated CDR session.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect end-user data. In the CDR this is restricted to the standard claims defined by the Profile Scope and Standard Claims standard.
  flows:
  - authorizationCode
  scope: profile
- description: Basic information on the customer who authorised the session - name and customer type.
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Detailed information on the authorised customer, adding contact details.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Energy accounts and plans.
  flows:
  - authorizationCode
  scope: energy:accounts.basic:read
- description: Energy account and plan details.
  flows:
  - authorizationCode
  scope: energy:accounts.detail:read
- description: Concessions and assistance applied to the account.
  flows:
  - authorizationCode
  scope: energy:accounts.concessions:read
- description: Agreed payment schedule and payment preferences.
  flows:
  - authorizationCode
  scope: energy:accounts.paymentschedule:read
- description: Billing, balances, invoices and payment history.
  flows:
  - authorizationCode
  scope: energy:billing:read
- description: Electricity connection - the NMI standing data basic set.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.basic:read
- description: Electricity connection and meter - the NMI standing data detail set.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.detail:read
- description: Electricity usage reads for the consented service points.
  flows:
  - authorizationCode
  scope: energy:electricity.usage:read
- description: Distributed energy resources - generation and storage devices behind the meter.
  flows:
  - authorizationCode
  scope: energy:electricity.der:read
slug: simply-energy-scopes
source_filename: simply-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/simply-energy-cds-energy-openapi.yml, openapi/simply-energy-cds-common-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nprovider_published: false\nprovenance_note: |\n  `derive-oauth-scopes.py` returned zero, because the shared Consumer Data Standards OpenAPI\n  documents carry no oauth2 securitySchemes. The scopes are nevertheless present and\n  machine-readable in the spec: every operation declares an `x-scopes` extension. The ten\n  scopes below were extracted from those `x-scopes` values and then enriched with the\n  consumer-facing data cluster and permission language published in the CDR Data Language\n  Standards. This is the normative scope set for an Australian energy data holder; this\n  retailer publishes no scope reference of its own.\nschemes:\n- name: CDR Security Profile (OAuth 2.0 + OpenID Connect, FAPI 1.0 Advanced)\n  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: null\n    tokenUrl: null\n    note: |\n      The authorisation and token endpoints of an energy data holder are published only via\n      the authenticated portion of the CDR Register and are not anonymously discoverable.\n      See authentication/simply-energy-authentication.yml.\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope. Establishes the authenticated CDR session.\n  category: openid-connect\n  flows: [authorizationCode]\n- scope: profile\n  description: OpenID Connect end-user data. In the CDR this is restricted to the standard\n    claims defined by the Profile Scope and Standard Claims standard.\n  category: openid-connect\n  flows: [authorizationCode]\n- scope: common:customer.basic:read\n  description: Basic information on the customer who authorised the session - name and\n    customer type.\n  data_cluster_language: Name and occupation / Organisation profile\n  category: common\n  operations:\
  \ [getCustomer]\n  sources: [openapi/simply-energy-cds-common-openapi.yml]\n  flows: [authorizationCode]\n- scope: common:customer.detail:read\n  description: Detailed information on the authorised customer, adding contact details.\n  data_cluster_language: Contact details\n  category: common\n  operations: [getCustomerDetail]\n  sources: [openapi/simply-energy-cds-common-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:accounts.basic:read\n  description: Energy accounts and plans.\n  data_cluster_language: Accounts and plans\n  permission_language: Account and plan information\n  category: energy-accounts\n  operations: [listEnergyAccounts]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:accounts.detail:read\n  description: Energy account and plan details.\n  data_cluster_language: Account and plan details\n  permission_language: Account type; Fees, features, rates, and discounts; Additional account\n    users\n  category:\
  \ energy-accounts\n  operations: [getEnergyAccountDetail]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:accounts.concessions:read\n  description: Concessions and assistance applied to the account.\n  data_cluster_language: Concessions and assistance\n  permission_language: Concession type; Concession information\n  category: energy-accounts\n  operations: [getEnergyAccountConcessions]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:accounts.paymentschedule:read\n  description: Agreed payment schedule and payment preferences.\n  data_cluster_language: Payment preferences\n  permission_language: Payment and billing frequency; Any scheduled payment details\n  category: energy-accounts\n  operations: [getEnergyAccountPaymentSchedule]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:billing:read\n  description: Billing,\
  \ balances, invoices and payment history.\n  data_cluster_language: Billing payments and history\n  permission_language: Account balance; Payment method; Payment status; Charges, discounts,\n    credits; Billing date; Usage for billing period; Payment date; Invoice number\n  category: energy-billing\n  operations: [getEnergyAccountBalance, listEnergyAccountBalancesBulk, listEnergyAccountBalancesSpecificAccounts,\n    getEnergyAccountInvoices, listEnergyAccountInvoicesBulk, listEnergyInvoicesForSpecificAccounts,\n    getBillingForEnergyAccount, listEnergyAccountBillingBulk, listEnergyAccountBillingForSpecificAccounts]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:electricity.servicepoints.basic:read\n  description: Electricity connection - the NMI standing data basic set.\n  data_cluster_language: Electricity connection\n  permission_language: National Meter Identifier (NMI); Customer type; Connection point details\n  category:\
  \ energy-servicepoints\n  operations: [listElectricityServicePoints]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:electricity.servicepoints.detail:read\n  description: Electricity connection and meter - the NMI standing data detail set.\n  data_cluster_language: Electricity meter\n  permission_language: Supply address; Meter details; Associated service providers\n  category: energy-servicepoints\n  operations: [getElectricityServicePointDetail]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\n- scope: energy:electricity.usage:read\n  description: Electricity usage reads for the consented service points.\n  data_cluster_language: Electricity usage\n  permission_language: Usage; Meter details\n  category: energy-usage\n  operations: [getElectricityServicePointUsage, listElectricityUsageBulk, listElectricityUsageForServicePoints]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n\
  \  flows: [authorizationCode]\n- scope: energy:electricity.der:read\n  description: Distributed energy resources - generation and storage devices behind the meter.\n  data_cluster_language: Energy generation and storage\n  permission_language: Generation information; Generation or storage device type; Device\n    characteristics; Devices that can operate without the grid; Energy conversion information\n  category: energy-der\n  operations: [getElectricityDERForServicePoint, listElectricityDERBulk, listElectricityDERForSpecificServicePoints]\n  sources: [openapi/simply-energy-cds-energy-openapi.yml]\n  flows: [authorizationCode]\nunscoped_operations:\n- {operationId: listEnergyPlans, reason: public unauthenticated generic tariff data}\n- {operationId: getEnergyPlanDetail, reason: public unauthenticated generic tariff data}\n- {operationId: getStatus, reason: public unauthenticated discovery endpoint}\n- {operationId: getOutages, reason: public unauthenticated discovery endpoint}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/scopes/simply-energy-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Smart Metering
- Energy Markets
token_urls: []
---
