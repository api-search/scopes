---
api_specs:
- filename: red-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Customers API
  slug: red-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-customers-api-openapi.yml
- filename: red-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: Red Energy Data Holder Operations API
  slug: red-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-data-holder-operations-api-openapi.yml
- filename: red-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Red Energy Distributed Energy Resources API
  slug: red-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-distributed-energy-resources-api-openapi.yml
- filename: red-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Service Points API
  slug: red-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-service-points-api-openapi.yml
- filename: red-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: Red Energy Electricity Usage API
  slug: red-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-electricity-usage-api-openapi.yml
- filename: red-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: Red Energy Energy Account Balances API
  slug: red-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-balances-api-openapi.yml
- filename: red-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: Red Energy Energy Account Billing API
  slug: red-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-account-billing-api-openapi.yml
- filename: red-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: Red Energy Energy Accounts API
  slug: red-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-accounts-api-openapi.yml
- filename: red-energy-energy-plans-api-openapi.yml
  format: yaml
  label: Red Energy Energy Plans API
  slug: red-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/openapi/red-energy-energy-plans-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Red Energy Scopes
name_suffix: OAuth Scopes
note: These are the CDR authorisation scopes Red Energy is bound to honour as a designated energy data holder. They apply ONLY to the consumer-authorised half of the surface, requested by an accredited data recipient in an OIDC authorisation request and granted by the individual customer. The anonymous half — listEnergyPlans, getEnergyPlanDetail, getStatus, getOutages — carries no scope at all. Scope-to-endpoint binding is the standard's, not Red Energy's; Red Energy publishes no scope documentation of its own.
overview: 'Red Energy publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Red Energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Red Energy
provider_slug: red-energy
schemes:
- flows:
  - authorizationUrl: null
    flow: authorizationCode
    note: Endpoints are published per-data-holder through the authenticated CDR Register, not anonymously. See authentication/red-energy-authentication.yml.
    tokenUrl: null
  name: CDR OAuth2 / OIDC (FAPI 1.0 Advanced)
  source: openapi/red-energy-cds-energy-openapi.yml
scope_count: 11
scope_names:
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
- description: Personally identifiable information about the customer. For individuals, name and occupation; for business customers, organisation name, ABN/ACN, charity status, establishment date, industry, organisation type and country of registration, plus the agent's name and role.
  flows: []
  scope: common:customer.basic:read
- description: Everything in Basic Customer Data plus contact details — phone, email address, mail address and residential (or organisation) address.
  flows: []
  scope: common:customer.detail:read
- description: Basic information about the customer's energy accounts with the retailer — simple account information, basic plan information and the service points that are part of the account. Excludes tailored plans, electricity contract detail and discounts.
  flows: []
  scope: energy:accounts.basic:read
- description: Additional authorisation on top of Basic Energy Account Data. Account type, fees, features, rates and discounts, and additional account users. Only meaningful when the basic scope is also authorised.
  flows: []
  scope: energy:accounts.detail:read
- description: Details of any concessions applied to a customer's energy account.
  flows: []
  scope: energy:accounts.concessions:read
- description: Payment schedules for energy accounts, including direct debit or credit based scheduled payments and manual payments.
  flows: []
  scope: energy:accounts.paymentschedule:read
- description: Billing and invoice data for a customer's energy account — account balance, payment method, payment status, charges, discounts and credits, billing date, usage for the billing period, payment date and invoice number.
  flows: []
  scope: energy:billing:read
- description: Basic standing data for the customer's service points, including the National Meter Identifier (NMI), customer type and connection point details. Excludes location and meter attributes.
  flows: []
  scope: energy:electricity.servicepoints.basic:read
- description: Additional authorisation on top of Basic Service Point Data — supply address, meter details and associated service providers. Only meaningful when the basic scope is also authorised.
  flows: []
  scope: energy:electricity.servicepoints.detail:read
- description: Electricity usage data for service points, including basic and interval meter reads. Additional authorisation on top of Basic Service Point Data.
  flows: []
  scope: energy:electricity.usage:read
- description: Data about distributed energy resources at the customer's service points — generation information, generation or storage device type, device characteristics, islandable devices and energy conversion information. Additional authorisation on top of Basic Service Point Data.
  flows: []
  scope: energy:electricity.der:read
slug: red-energy-scopes
source_filename: red-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Baseline DERIVED from the x-scopes vendor extension on every operation in\n  openapi/red-energy-cds-energy-openapi.yml and\n  openapi/red-energy-cds-common-openapi.yml (the DSB cds_energy / cds_common\n  v1.36.0 documents declare no components.securitySchemes, so\n  0-working/derive-oauth-scopes.py found nothing to aggregate), then SEARCHED\n  and enriched from the Consumer Data Standards \"Authorisation Scopes\" and\n  \"Data Language Standards\" reference.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ncx_docs: https://consumerdatastandardsaustralia.github.io/standards/#data-language-standards\nprovider: Red Energy\nproviderId: red-energy\n\nnote: >-\n  These are the CDR authorisation scopes Red Energy is bound to honour as a\n  designated energy data holder. They apply ONLY to the consumer-authorised half\n  of the surface, requested by an accredited data recipient in an OIDC\n\
  \  authorisation request and granted by the individual customer. The anonymous\n  half — listEnergyPlans, getEnergyPlanDetail, getStatus, getOutages — carries no\n  scope at all. Scope-to-endpoint binding is the standard's, not Red Energy's;\n  Red Energy publishes no scope documentation of its own.\n\nschemes:\n  - name: CDR OAuth2 / OIDC (FAPI 1.0 Advanced)\n    source: openapi/red-energy-cds-energy-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: null\n        tokenUrl: null\n        note: >-\n          Endpoints are published per-data-holder through the authenticated CDR\n          Register, not anonymously. See authentication/red-energy-authentication.yml.\n\noidc_scopes:\n  - scope: openid\n    description: Required OIDC scope; requests an ID Token for the authenticated consumer.\n  - scope: profile\n    description: >-\n      Standard OIDC profile scope. Under the CDS, name-related claims may be\n      requested either via the profile scope or\
  \ as individual OIDC claims\n      (name, given_name, family_name, updated_at).\n\nscopes:\n  - scope: common:customer.basic:read\n    name: Basic Customer Data\n    description: >-\n      Personally identifiable information about the customer. For individuals,\n      name and occupation; for business customers, organisation name, ABN/ACN,\n      charity status, establishment date, industry, organisation type and country\n      of registration, plus the agent's name and role.\n    data_cluster_language: Name and occupation / Organisation profile\n    operations: [getCustomer]\n    sources: [openapi/red-energy-cds-common-openapi.yml]\n  - scope: common:customer.detail:read\n    name: Detailed Customer Data\n    description: >-\n      Everything in Basic Customer Data plus contact details — phone, email\n      address, mail address and residential (or organisation) address.\n    data_cluster_language: Contact details / Organisation contact details\n    operations: [getCustomerDetail]\n \
  \   sources: [openapi/red-energy-cds-common-openapi.yml]\n  - scope: energy:accounts.basic:read\n    name: Basic Energy Account Data\n    description: >-\n      Basic information about the customer's energy accounts with the retailer —\n      simple account information, basic plan information and the service points\n      that are part of the account. Excludes tailored plans, electricity contract\n      detail and discounts.\n    data_cluster_language: Accounts and plans\n    operations: [listEnergyAccounts]\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:accounts.detail:read\n    name: Detailed Energy Account Data\n    description: >-\n      Additional authorisation on top of Basic Energy Account Data. Account type,\n      fees, features, rates and discounts, and additional account users. Only\n      meaningful when the basic scope is also authorised.\n    data_cluster_language: Account and plan details\n    operations: [getEnergyAccountDetail]\n    sources:\
  \ [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:accounts.concessions:read\n    name: Energy Concession Data\n    description: Details of any concessions applied to a customer's energy account.\n    data_cluster_language: Concessions and assistance\n    operations: [getEnergyAccountConcessions]\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:accounts.paymentschedule:read\n    name: Energy Regular Payments Data\n    description: >-\n      Payment schedules for energy accounts, including direct debit or credit\n      based scheduled payments and manual payments.\n    data_cluster_language: Payment preferences\n    operations: [getEnergyAccountPaymentSchedule]\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:billing:read\n    name: Energy Billing Data\n    description: >-\n      Billing and invoice data for a customer's energy account — account balance,\n      payment method, payment status, charges, discounts and credits,\
  \ billing\n      date, usage for the billing period, payment date and invoice number.\n    data_cluster_language: Billing payments and history\n    operations:\n      - getEnergyAccountBalance\n      - listEnergyAccountBalancesBulk\n      - listEnergyAccountBalancesSpecificAccounts\n      - getBillingForEnergyAccount\n      - listEnergyAccountBillingBulk\n      - listEnergyAccountBillingForSpecificAccounts\n      - getEnergyAccountInvoices\n      - listEnergyAccountInvoicesBulk\n      - listEnergyInvoicesForSpecificAccounts\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:electricity.servicepoints.basic:read\n    name: Basic Service Point Data\n    description: >-\n      Basic standing data for the customer's service points, including the\n      National Meter Identifier (NMI), customer type and connection point\n      details. Excludes location and meter attributes.\n    data_cluster_language: Electricity connection\n    operations: [listElectricityServicePoints]\n\
  \    sources: [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:electricity.servicepoints.detail:read\n    name: Detailed Service Point Data\n    description: >-\n      Additional authorisation on top of Basic Service Point Data — supply\n      address, meter details and associated service providers. Only meaningful\n      when the basic scope is also authorised.\n    data_cluster_language: Electricity meter\n    operations: [getElectricityServicePointDetail]\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n  - scope: energy:electricity.usage:read\n    name: Electricity Usage Data\n    description: >-\n      Electricity usage data for service points, including basic and interval\n      meter reads. Additional authorisation on top of Basic Service Point Data.\n    data_cluster_language: Electricity usage\n    operations:\n      - listElectricityUsageBulk\n      - getElectricityServicePointUsage\n      - listElectricityUsageForServicePoints\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n\
  \  - scope: energy:electricity.der:read\n    name: Distributed Energy Resource Data\n    description: >-\n      Data about distributed energy resources at the customer's service points —\n      generation information, generation or storage device type, device\n      characteristics, islandable devices and energy conversion information.\n      Additional authorisation on top of Basic Service Point Data.\n    data_cluster_language: Energy generation and storage\n    operations:\n      - listElectricityDERBulk\n      - getElectricityDERForServicePoint\n      - listElectricityDERForSpecificServicePoints\n    sources: [openapi/red-energy-cds-energy-openapi.yml]\n\nunscoped_operations:\n  - operationId: listEnergyPlans\n    reason: Unauthenticated CDR Product Reference Data. No scope, no token, no accreditation.\n  - operationId: getEnergyPlanDetail\n    reason: Unauthenticated CDR Product Reference Data.\n  - operationId: getStatus\n    reason: Unauthenticated CDR Common Data Holder Operations\
  \ endpoint.\n  - operationId: getOutages\n    reason: Unauthenticated CDR Common Data Holder Operations endpoint.\n\nsecondary_data_holder_note: >-\n  Interval metering data behind energy:electricity.usage:read and the NMI\n  standing data behind the service point scopes ultimately originate with AEMO\n  as the CDR secondary data holder. Red Energy is the primary data holder for\n  the account, billing and tariff side and makes a Shared Responsibility Data\n  Request for the rest.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-energy/refs/heads/main/scopes/red-energy-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Open Data
token_urls: []
---
