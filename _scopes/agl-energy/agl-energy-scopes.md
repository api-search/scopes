---
api_specs:
- filename: agl-energy-cds-energy-openapi.json
  format: json
  label: AGL CDR Energy API
  slug: agl-cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-cds-energy-openapi.json
- filename: agl-energy-cds-common-openapi.json
  format: json
  label: AGL CDR Discovery (Common) API
  slug: agl-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-cds-common-openapi.json
- filename: agl-energy-cds-energy-openapi.json
  format: json
  label: AGL Energy Product Reference Data (PRD) API
  slug: agl-energy-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-cds-energy-openapi.json
authorization_urls: []
description: The eleven CDR consent scopes that govern AGL's consumer energy data. These are not declared in an OpenAPI securityScheme — the harvested Consumer Data Standards documents ship an empty components.securitySchemes — they are carried per operation in the DSB's x-scopes extension and defined normatively in the standards. A consumer authorises a subset of these scopes through AGL's CDR consent flow; the Accredited Data Recipient's access token then carries only what was consented, for the duration the consumer chose.
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Agl Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AGL Energy publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the AGL Energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AGL Energy
provider_slug: agl-energy
schemes: []
scope_count: 11
scope_names:
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
- description: Name and occupation for an individual, or agent name and role for a non-individual customer.
  flows: []
  scope: common:customer.basic:read
- description: Customer contact details — phone, email, mail address, residential address.
  flows: []
  scope: common:customer.detail:read
- description: Account identifiers, display name, open/closed status and plan overview for the consumer's energy accounts.
  flows: []
  scope: energy:accounts.basic:read
- description: Full account detail including plan detail, tariffs, authorised contacts and associated service points.
  flows: []
  scope: energy:accounts.detail:read
- description: The agreed payment schedule for an account — direct debit, card debit, digital wallet or manual payment arrangements.
  flows: []
  scope: energy:accounts.paymentschedule:read
- description: Concessions and rebates applied to the consumer's energy account.
  flows: []
  scope: energy:accounts.concessions:read
- description: Account balances, invoices and billing transactions — the money side of the account.
  flows: []
  scope: energy:billing:read
- description: The NMIs (service points) associated with the consumer, with basic status and classification.
  flows: []
  scope: energy:electricity.servicepoints.basic:read
- description: Service point detail — meters, registers, distribution loss factor, related market participants, technical specifications.
  flows: []
  scope: energy:electricity.servicepoints.detail:read
- description: Interval and basic meter reads for a service point — the consumption data itself.
  flows: []
  scope: energy:electricity.usage:read
- description: Distributed Energy Resource register detail — solar PV, batteries, inverters, AC connections and protection modes.
  flows: []
  scope: energy:electricity.der:read
slug: agl-energy-scopes
source_filename: agl-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: >-\n  x-scopes extensions on every operation in\n  openapi/agl-energy-cds-energy-openapi.json and\n  openapi/agl-energy-cds-common-openapi.json (CDR Energy API + CDR Common API\n  v1.36.0), cross-checked against the Consumer Data Standards authorisation\n  scopes documentation.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndescription: >-\n  The eleven CDR consent scopes that govern AGL's consumer energy data. These are\n  not declared in an OpenAPI securityScheme — the harvested Consumer Data\n  Standards documents ship an empty components.securitySchemes — they are carried\n  per operation in the DSB's x-scopes extension and defined normatively in the\n  standards. A consumer authorises a subset of these scopes through AGL's CDR\n  consent flow; the Accredited Data Recipient's access token then carries only\n  what was consented, for the duration the consumer chose.\nscheme:\n  type:\
  \ oauth2\n  flow: authorizationCode\n  profile: FAPI 1.0 Advanced (CDR Security Profile)\n  authorizationUrl: null\n  tokenUrl: null\n  endpoint_note: >-\n    AGL's authorisation and token endpoints are not published anonymously. They\n    are distributed to Accredited Data Recipients through the CDR Register. No\n    URL is recorded here rather than guessed.\nscope_count: 11\nscopes:\n- scope: common:customer.basic:read\n  description: Name and occupation for an individual, or agent name and role for a non-individual customer.\n  sources: [openapi/agl-energy-cds-common-openapi.json]\n  operations: [getCustomer]\n- scope: common:customer.detail:read\n  description: Customer contact details — phone, email, mail address, residential address.\n  sources: [openapi/agl-energy-cds-common-openapi.json]\n  operations: [getCustomerDetail]\n- scope: energy:accounts.basic:read\n  description: Account identifiers, display name, open/closed status and plan overview for the consumer's energy accounts.\n\
  \  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations: [listEnergyAccounts]\n- scope: energy:accounts.detail:read\n  description: Full account detail including plan detail, tariffs, authorised contacts and associated service points.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations: [getEnergyAccountDetail]\n- scope: energy:accounts.paymentschedule:read\n  description: The agreed payment schedule for an account — direct debit, card debit, digital wallet or manual payment arrangements.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations: [getEnergyAccountPaymentSchedule]\n- scope: energy:accounts.concessions:read\n  description: Concessions and rebates applied to the consumer's energy account.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations: [getEnergyAccountConcessions]\n- scope: energy:billing:read\n  description: Account balances, invoices and billing transactions — the money side of the account.\n  sources:\
  \ [openapi/agl-energy-cds-energy-openapi.json]\n  operations:\n  - getEnergyAccountBalance\n  - listEnergyAccountBalancesBulk\n  - listEnergyAccountBalancesSpecificAccounts\n  - getEnergyAccountInvoices\n  - listEnergyAccountInvoicesBulk\n  - listEnergyInvoicesForSpecificAccounts\n  - getBillingForEnergyAccount\n  - listEnergyAccountBillingBulk\n  - listEnergyAccountBillingForSpecificAccounts\n- scope: energy:electricity.servicepoints.basic:read\n  description: The NMIs (service points) associated with the consumer, with basic status and classification.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations: [listElectricityServicePoints]\n- scope: energy:electricity.servicepoints.detail:read\n  description: Service point detail — meters, registers, distribution loss factor, related market participants, technical specifications.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations: [getElectricityServicePointDetail]\n- scope: energy:electricity.usage:read\n\
  \  description: Interval and basic meter reads for a service point — the consumption data itself.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations:\n  - getElectricityServicePointUsage\n  - listElectricityUsageBulk\n  - listElectricityUsageForServicePoints\n- scope: energy:electricity.der:read\n  description: Distributed Energy Resource register detail — solar PV, batteries, inverters, AC connections and protection modes.\n  sources: [openapi/agl-energy-cds-energy-openapi.json]\n  operations:\n  - getElectricityDERForServicePoint\n  - listElectricityDERBulk\n  - listElectricityDERForSpecificServicePoints\nunscoped_operations:\n  note: >-\n    Four operations carry no x-scopes because they are unauthenticated under the\n    Consumer Data Standards.\n  operations:\n  - {operationId: getStatus, surface: AGL CDR Discovery, auth: none}\n  - {operationId: getOutages, surface: AGL CDR Discovery, auth: none}\n  - {operationId: listEnergyPlans, surface: Product Reference Data\
  \ (AER-hosted), auth: none}\n  - {operationId: getEnergyPlanDetail, surface: Product Reference Data (AER-hosted), auth: none}\nsecondary_data_holder:\n  party: AEMO\n  role: >-\n    Secondary data holder for NMI standing data and metering data. AGL requests\n    it from AEMO on the consumer's behalf under the same consent; errors\n    propagated from AEMO are flagged with isSecondaryDataHolderError on the CDS\n    error object.\n  docs: https://www.aemo.com.au/energy-systems/electricity/cdr-at-aemo/about-cdr\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/scopes/agl-energy-scopes.yml
summary_line: 11 scopes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Smart Metering
- Solar
- DER
- Renewables
- Energy Markets
token_urls: []
---
