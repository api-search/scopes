---
api_specs:
- filename: energyaustralia-data-holder-customers-api-openapi.yml
  format: yaml
  label: EnergyAustralia Data Holder Customers API
  slug: energyaustralia-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-data-holder-customers-api-openapi.yml
- filename: energyaustralia-data-holder-operations-api-openapi.yml
  format: yaml
  label: EnergyAustralia Data Holder Operations API
  slug: energyaustralia-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-data-holder-operations-api-openapi.yml
- filename: energyaustralia-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: EnergyAustralia Distributed Energy Resources API
  slug: energyaustralia-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-distributed-energy-resources-api-openapi.yml
- filename: energyaustralia-electricity-service-points-api-openapi.yml
  format: yaml
  label: EnergyAustralia Electricity Service Points API
  slug: energyaustralia-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-electricity-service-points-api-openapi.yml
- filename: energyaustralia-electricity-usage-api-openapi.yml
  format: yaml
  label: EnergyAustralia Electricity Usage API
  slug: energyaustralia-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-electricity-usage-api-openapi.yml
- filename: energyaustralia-energy-account-balances-api-openapi.yml
  format: yaml
  label: EnergyAustralia Energy Account Balances API
  slug: energyaustralia-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-energy-account-balances-api-openapi.yml
- filename: energyaustralia-energy-account-billing-api-openapi.yml
  format: yaml
  label: EnergyAustralia Energy Account Billing API
  slug: energyaustralia-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-energy-account-billing-api-openapi.yml
- filename: energyaustralia-energy-accounts-api-openapi.yml
  format: yaml
  label: EnergyAustralia Energy Accounts API
  slug: energyaustralia-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-energy-accounts-api-openapi.yml
- filename: energyaustralia-energy-plans-api-openapi.yml
  format: yaml
  label: EnergyAustralia Energy Plans API
  slug: energyaustralia-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-energy-plans-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Energyaustralia Scopes
name_suffix: OAuth Scopes
note: Derived from the per-operation `x-scopes` extension in the Consumer Data Standards CDR Energy API 1.36.0 and CDR Common API 1.36.0. The CDS OpenAPI documents do NOT declare `components.securitySchemes` — authorisation is specified out-of-band in the CDR Information Security profile (FAPI 1.0 Advanced), and the resource-server scopes are carried per operation as `x-scopes`. `derive-oauth-scopes.py` therefore returns zero for this provider; this file was derived by reading `x-scopes` directly. EnergyAustralia is a live registered CDR energy data holder (ACCC CDR Register dataHolderBrandId 1cc7833a-b834-ed11-a832-000d3a8830d6), so these are the scopes an accredited Data Recipient requests against its publicBaseUri. The scope values are ecosystem-wide CDR values, identical for every energy data holder — EnergyAustralia publishes no proprietary scope reference.
overview: 'EnergyAustralia publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EnergyAustralia API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EnergyAustralia
provider_slug: energyaustralia
schemes:
- flows:
  - authorizationUrl: null
    flow: authorizationCode
    note: Endpoints are discoverable only via the data holder's OIDC discovery document, which requires CDR Register-issued mTLS client certificates to reach.
    par: true
    pkce: true
    tokenUrl: null
  name: CDR OAuth2 / OIDC (FAPI 1.0 Advanced)
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: oauth2
scope_count: 12
scope_names:
- openid
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
- description: Mandatory OpenID Connect base scope. Required on every CDR authorisation request.
  flows:
  - authorizationCode
  scope: openid
- description: Name and occupation for an individual customer; agent name and role plus organisation name, industry code and ABN/ACN for a non-individual customer.
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: The basic customer data plus phone, email, mail address and residential address.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Account identifiers, account numbers, display names, creation date, plan overview and open/closed status for the consumer's energy accounts.
  flows:
  - authorizationCode
  scope: energy:accounts.basic:read
- description: Full account detail including the plan detail, linked service point (NMI) ids and authorised contacts on the account.
  flows:
  - authorizationCode
  scope: energy:accounts.detail:read
- description: The agreed payment schedule for an account — card debit, direct debit, digital wallet or manual payment, with frequency and calculation type.
  flows:
  - authorizationCode
  scope: energy:accounts.paymentschedule:read
- description: Concessions and rebates applied to an energy account.
  flows:
  - authorizationCode
  scope: energy:accounts.concessions:read
- description: Account balances, invoices and billing transactions — the widest-fanout energy scope, backing nine operations across balance, invoice and billing resources.
  flows:
  - authorizationCode
  scope: energy:billing:read
- description: Basic electricity service point (NMI) data — service point id, classification, jurisdiction and status.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.basic:read
- description: Detailed service point data including the NMI standing data held by AEMO as secondary data holder — meters, registers and related participants.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.detail:read
- description: Interval and accumulated electricity usage reads for the consumer's service points.
  flows:
  - authorizationCode
  scope: energy:electricity.usage:read
- description: Distributed Energy Resource register data — solar PV, battery and inverter device records associated with the consumer's service points.
  flows:
  - authorizationCode
  scope: energy:electricity.der:read
slug: energyaustralia-scopes
source_filename: energyaustralia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/energyaustralia-cds-energy-api-openapi.yml, openapi/energyaustralia-cds-common-api-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  Derived from the per-operation `x-scopes` extension in the Consumer Data Standards\n  CDR Energy API 1.36.0 and CDR Common API 1.36.0. The CDS OpenAPI documents do NOT\n  declare `components.securitySchemes` — authorisation is specified out-of-band in the\n  CDR Information Security profile (FAPI 1.0 Advanced), and the resource-server scopes\n  are carried per operation as `x-scopes`. `derive-oauth-scopes.py` therefore returns\n  zero for this provider; this file was derived by reading `x-scopes` directly.\n  EnergyAustralia is a live registered CDR energy data holder (ACCC CDR Register\n  dataHolderBrandId 1cc7833a-b834-ed11-a832-000d3a8830d6), so these are the scopes an\n  accredited Data Recipient requests against its publicBaseUri.\
  \ The scope values are\n  ecosystem-wide CDR values, identical for every energy data holder — EnergyAustralia\n  publishes no proprietary scope reference.\nauthorization_model:\n  profile: FAPI 1.0 Advanced (CDR Information Security profile)\n  protocol: OAuth 2.0 + OpenID Connect\n  consent: Per-consumer authorisation with an explicit CDR consent and sharing duration\n  authorization_server: >-\n    Published per data holder brand in the ACCC CDR Register. EnergyAustralia's\n    publicBaseUri is https://authncdr.energyaustralia.com.au; its OIDC discovery\n    document was NOT anonymously readable (HTTP 404 on\n    /.well-known/openid-configuration, probed 2026-07-27), so authorizationUrl and\n    tokenUrl could not be captured without ACCC accreditation.\n  discovery_gated: true\nschemes:\n- name: CDR OAuth2 / OIDC (FAPI 1.0 Advanced)\n  type: oauth2\n  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  flows:\n  - flow: authorizationCode\n    pkce:\
  \ true\n    par: true\n    authorizationUrl: null\n    tokenUrl: null\n    note: >-\n      Endpoints are discoverable only via the data holder's OIDC discovery document,\n      which requires CDR Register-issued mTLS client certificates to reach.\nscopes:\n- scope: openid\n  description: >-\n    Mandatory OpenID Connect base scope. Required on every CDR authorisation request.\n  flows: [authorizationCode]\n  sources: [https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes]\n- scope: common:customer.basic:read\n  description: >-\n    Name and occupation for an individual customer; agent name and role plus\n    organisation name, industry code and ABN/ACN for a non-individual customer.\n  flows: [authorizationCode]\n  operations: [getCustomer]\n  sources: [openapi/energyaustralia-cds-common-api-openapi.yml]\n- scope: common:customer.detail:read\n  description: >-\n    The basic customer data plus phone, email, mail address and residential address.\n  flows: [authorizationCode]\n\
  \  operations: [getCustomerDetail]\n  sources: [openapi/energyaustralia-cds-common-api-openapi.yml]\n- scope: energy:accounts.basic:read\n  description: >-\n    Account identifiers, account numbers, display names, creation date, plan overview\n    and open/closed status for the consumer's energy accounts.\n  flows: [authorizationCode]\n  operations: [listEnergyAccounts]\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:accounts.detail:read\n  description: >-\n    Full account detail including the plan detail, linked service point (NMI) ids and\n    authorised contacts on the account.\n  flows: [authorizationCode]\n  operations: [getEnergyAccountDetail]\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:accounts.paymentschedule:read\n  description: >-\n    The agreed payment schedule for an account — card debit, direct debit, digital\n    wallet or manual payment, with frequency and calculation type.\n  flows: [authorizationCode]\n\
  \  operations: [getEnergyAccountPaymentSchedule]\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:accounts.concessions:read\n  description: >-\n    Concessions and rebates applied to an energy account.\n  flows: [authorizationCode]\n  operations: [getEnergyAccountConcessions]\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:billing:read\n  description: >-\n    Account balances, invoices and billing transactions — the widest-fanout energy\n    scope, backing nine operations across balance, invoice and billing resources.\n  flows: [authorizationCode]\n  operations:\n  - getEnergyAccountBalance\n  - listEnergyAccountBalancesBulk\n  - listEnergyAccountBalancesSpecificAccounts\n  - getEnergyAccountInvoices\n  - listEnergyAccountInvoicesBulk\n  - listEnergyInvoicesForSpecificAccounts\n  - getBillingForEnergyAccount\n  - listEnergyAccountBillingBulk\n  - listEnergyAccountBillingForSpecificAccounts\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n\
  - scope: energy:electricity.servicepoints.basic:read\n  description: >-\n    Basic electricity service point (NMI) data — service point id, classification,\n    jurisdiction and status.\n  flows: [authorizationCode]\n  operations: [listElectricityServicePoints]\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:electricity.servicepoints.detail:read\n  description: >-\n    Detailed service point data including the NMI standing data held by AEMO as\n    secondary data holder — meters, registers and related participants.\n  flows: [authorizationCode]\n  operations: [getElectricityServicePointDetail]\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:electricity.usage:read\n  description: >-\n    Interval and accumulated electricity usage reads for the consumer's service points.\n  flows: [authorizationCode]\n  operations:\n  - getElectricityServicePointUsage\n  - listElectricityUsageBulk\n  - listElectricityUsageForServicePoints\n\
  \  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\n- scope: energy:electricity.der:read\n  description: >-\n    Distributed Energy Resource register data — solar PV, battery and inverter device\n    records associated with the consumer's service points.\n  flows: [authorizationCode]\n  operations:\n  - getElectricityDERForServicePoint\n  - listElectricityDERBulk\n  - listElectricityDERForSpecificServicePoints\n  sources: [openapi/energyaustralia-cds-energy-api-openapi.yml]\nunauthenticated_operations:\n  note: >-\n    These operations carry no `x-scopes` and are served publicly on the AER Energy Made\n    Easy CDR gateway at the EnergyAustralia brand path. Verified HTTP 200 on 2026-07-27.\n  operations: [listEnergyPlans, getEnergyPlanDetail, getStatus, getOutages]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/scopes/energyaustralia-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Energy Markets
- Renewables
token_urls: []
---
