---
api_specs:
- filename: powershop-data-holder-customers-api-openapi.yml
  format: yaml
  label: Powershop Data Holder Customers API
  slug: powershop-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-data-holder-customers-api-openapi.yml
- filename: powershop-data-holder-operations-api-openapi.yml
  format: yaml
  label: Powershop Data Holder Operations API
  slug: powershop-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-data-holder-operations-api-openapi.yml
- filename: powershop-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Powershop Distributed Energy Resources API
  slug: powershop-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-distributed-energy-resources-api-openapi.yml
- filename: powershop-electricity-service-points-api-openapi.yml
  format: yaml
  label: Powershop Electricity Service Points API
  slug: powershop-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-electricity-service-points-api-openapi.yml
- filename: powershop-electricity-usage-api-openapi.yml
  format: yaml
  label: Powershop Electricity Usage API
  slug: powershop-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-electricity-usage-api-openapi.yml
- filename: powershop-energy-account-balances-api-openapi.yml
  format: yaml
  label: Powershop Energy Account Balances API
  slug: powershop-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-account-balances-api-openapi.yml
- filename: powershop-energy-account-billing-api-openapi.yml
  format: yaml
  label: Powershop Energy Account Billing API
  slug: powershop-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-account-billing-api-openapi.yml
- filename: powershop-energy-accounts-api-openapi.yml
  format: yaml
  label: Powershop Energy Accounts API
  slug: powershop-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-accounts-api-openapi.yml
- filename: powershop-energy-plans-api-openapi.yml
  format: yaml
  label: Powershop Energy Plans API
  slug: powershop-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-energy-plans-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Powershop Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Powershop publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Powershop API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Powershop
provider_slug: powershop
schemes: []
scope_count: 11
scope_names:
- energy:accounts.basic:read
- energy:accounts.detail:read
- energy:accounts.concessions:read
- energy:accounts.paymentschedule:read
- energy:billing:read
- energy:electricity.servicepoints.basic:read
- energy:electricity.servicepoints.detail:read
- energy:electricity.usage:read
- energy:electricity.der:read
- common:customer.basic:read
- common:customer.detail:read
scopes:
- description: Read basic energy account information — account ID, account number, display name, open/closed status, creation date, and the plan(s) and service point IDs attached to each account.
  flows: []
  scope: energy:accounts.basic:read
- description: Read detailed energy account information — the full plan detail per account including fuel type, contingent-plan flag, metering charges, and the gas and electricity contract terms, plus authorised contacts.
  flows: []
  scope: energy:accounts.detail:read
- description: Read concessions and rebates applied to the account — type, display name, discount frequency, amount or percentage, applicability period and what the concession is applied to.
  flows: []
  scope: energy:accounts.concessions:read
- description: Read the payment schedule for an account — amount and method (card debit, direct debit, digital wallet or manual payment) with payment frequency and calculation type.
  flows: []
  scope: energy:accounts.paymentschedule:read
- description: Read account balances, invoices and billing transactions — including usage, demand, once-off, other-charge and payment transaction types, invoice periods, GST and pay-on-time discounts.
  flows: []
  scope: energy:billing:read
- description: Read basic electricity service point data — the NMI-level service point list the consumer has authorised.
  flows: []
  scope: energy:electricity.servicepoints.basic:read
- description: Read detailed electricity service point data — NMI standing data sourced from AEMO as secondary data holder.
  flows: []
  scope: energy:electricity.servicepoints.detail:read
- description: Read interval metering (usage) data for authorised service points, sourced from AEMO as secondary data holder.
  flows: []
  scope: energy:electricity.usage:read
- description: Read Distributed Energy Resource (rooftop solar, inverter and battery) register data for authorised service points — approved capacity, phase counts, islandable installation, protection mode, AC connections and DER devices. Sourced from the AEMO DER register.
  flows: []
  scope: energy:electricity.der:read
- description: Read basic customer information — name or business/organisation name for the authorising consumer.
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer information — contact details, supply address, and for business customers the business name and ABN.
  flows: []
  scope: common:customer.detail:read
slug: powershop-scopes
source_filename: powershop-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  openapi/powershop-cdr-energy-api-openapi.json and\n  openapi/powershop-cdr-common-api-openapi.json (x-scopes extension declared\n  per operation) + DSB Consumer Data Standards authorisation scopes\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nsummary: >-\n  OAuth 2.0 authorisation scopes governing the consented, accreditation-gated\n  half of Powershop's Consumer Data Right obligation. These are the standard\n  Data Standards Body CDR energy and common scopes, declared per-operation in\n  the shared sector OpenAPI via the x-scopes extension — Powershop defines no\n  proprietary scopes and publishes no scope documentation of its own. They apply\n  to the OpenID Connect / FAPI authorisation flow brokered by an ACCC accredited\n  data recipient, NOT to the public unauthenticated surfaces: the CDS Discovery\n  endpoints (getStatus, getOutages) and the Generic Tariff endpoints\n \
  \ (listEnergyPlans, getEnergyPlanDetail) declare no x-scopes and require none.\nflow:\n  grant: authorization_code\n  profile: FAPI / OpenID Connect with PAR, JARM and mutual-TLS sender-constrained tokens\n  registry: CDR Register (ACCC) / Data Standards Body security profile\n  cross_link: authentication/powershop-authentication.yml\nschemes: []\nschemes_note: >-\n  Neither shared CDS OpenAPI declares components.securitySchemes, so no oauth2\n  flow object with authorizationUrl/tokenUrl can be derived. Powershop's\n  authorisation and token endpoints are not published anonymously; they are\n  resolved through the CDR Register by accredited participants.\nscopes:\n- scope: energy:accounts.basic:read\n  description: >-\n    Read basic energy account information — account ID, account number, display\n    name, open/closed status, creation date, and the plan(s) and service point\n    IDs attached to each account.\n  operations: [listEnergyAccounts]\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n\
  - scope: energy:accounts.detail:read\n  description: >-\n    Read detailed energy account information — the full plan detail per account\n    including fuel type, contingent-plan flag, metering charges, and the gas and\n    electricity contract terms, plus authorised contacts.\n  operations: [getEnergyAccountDetail]\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: energy:accounts.concessions:read\n  description: >-\n    Read concessions and rebates applied to the account — type, display name,\n    discount frequency, amount or percentage, applicability period and what the\n    concession is applied to.\n  operations: [getEnergyAccountConcessions]\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: energy:accounts.paymentschedule:read\n  description: >-\n    Read the payment schedule for an account — amount and method (card debit,\n    direct debit, digital wallet or manual payment) with payment frequency and\n    calculation type.\n  operations: [getEnergyAccountPaymentSchedule]\n\
  \  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: energy:billing:read\n  description: >-\n    Read account balances, invoices and billing transactions — including usage,\n    demand, once-off, other-charge and payment transaction types, invoice\n    periods, GST and pay-on-time discounts.\n  operations:\n  - getEnergyAccountBalance\n  - listEnergyAccountBalancesBulk\n  - listEnergyAccountBalancesSpecificAccounts\n  - getEnergyAccountInvoices\n  - listEnergyAccountInvoicesBulk\n  - listEnergyInvoicesForSpecificAccounts\n  - getBillingForEnergyAccount\n  - listEnergyAccountBillingBulk\n  - listEnergyAccountBillingForSpecificAccounts\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: energy:electricity.servicepoints.basic:read\n  description: >-\n    Read basic electricity service point data — the NMI-level service point list\n    the consumer has authorised.\n  operations: [listElectricityServicePoints]\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n\
  - scope: energy:electricity.servicepoints.detail:read\n  description: >-\n    Read detailed electricity service point data — NMI standing data sourced\n    from AEMO as secondary data holder.\n  operations: [getElectricityServicePointDetail]\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: energy:electricity.usage:read\n  description: >-\n    Read interval metering (usage) data for authorised service points, sourced\n    from AEMO as secondary data holder.\n  operations:\n  - getElectricityServicePointUsage\n  - listElectricityUsageBulk\n  - listElectricityUsageForServicePoints\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: energy:electricity.der:read\n  description: >-\n    Read Distributed Energy Resource (rooftop solar, inverter and battery)\n    register data for authorised service points — approved capacity, phase\n    counts, islandable installation, protection mode, AC connections and DER\n    devices. Sourced from the AEMO DER register.\n\
  \  operations:\n  - getElectricityDERForServicePoint\n  - listElectricityDERBulk\n  - listElectricityDERForSpecificServicePoints\n  sources: [openapi/powershop-cdr-energy-api-openapi.json]\n- scope: common:customer.basic:read\n  description: >-\n    Read basic customer information — name or business/organisation name for the\n    authorising consumer.\n  operations: [getCustomer]\n  sources: [openapi/powershop-cdr-common-api-openapi.json]\n- scope: common:customer.detail:read\n  description: >-\n    Read detailed customer information — contact details, supply address, and\n    for business customers the business name and ABN.\n  operations: [getCustomerDetail]\n  sources: [openapi/powershop-cdr-common-api-openapi.json]\nunscoped_operations:\n  note: Public endpoints that declare no x-scopes and require no authorisation.\n  operations: [listEnergyPlans, getEnergyPlanDetail, getStatus, getOutages]\ndata_clusters_per_powershop_policy:\n  source: https://www.powershop.com.au/privacy-policy/cdr-policy\n\
  \  note: >-\n    Powershop's own CDR policy names the data it shares in consumer language,\n    which maps onto the scopes above.\n  clusters:\n  - Customer data — name, contact details, supply address, business name, ABN\n  - Account data — account number, creation date, identifiers, product data, payment arrangements, concessions and rebates\n  - Invoice and billing data\n  - AEMO data — metering (usage) data, NMI standing data, DER (solar) register data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/scopes/powershop-scopes.yml
summary_line: 11 scopes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Consumer Data Right
- Energy Retail
- Smart Metering
- Solar
- Tariffs
- Open Data
token_urls: []
---
