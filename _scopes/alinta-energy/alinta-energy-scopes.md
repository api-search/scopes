---
api_specs:
- filename: alinta-energy-cds-common-api-openapi.yml
  format: yaml
  label: Alinta Energy CDR Discovery API
  slug: alinta-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-cds-common-api-openapi.yml
- filename: alinta-energy-cds-energy-api-openapi.yml
  format: yaml
  label: Alinta Energy CDR Generic Plan Data API
  slug: alinta-energy-cdr-generic-plan-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-cds-energy-api-openapi.yml
- filename: alinta-energy-cds-energy-api-openapi.yml
  format: yaml
  label: Alinta Energy CDR Energy API
  slug: alinta-energy-cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-cds-energy-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alinta Energy Scopes
name_suffix: OAuth Scopes
note: 'Alinta''s publicly callable endpoints require NO scope: the CDR discovery pair (/discovery/status, /discovery/outages) and the generic plan data endpoints (/energy/plans, /energy/plans/{planId}) are unauthenticated and carry no x-scopes. The scopes below govern the consumer-data-sharing operations in the shared DSB Consumer Data Standards contract that Alinta implements as a designated energy data holder, and are only obtainable by an ACCC-accredited Data Recipient holding a valid consumer consent. Scope strings are captured verbatim from the specs'' per-operation x-scopes extension; descriptions are from the Consumer Data Standards authorisation scopes reference.'
overview: 'Alinta Energy publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alinta Energy API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alinta Energy
provider_slug: alinta-energy
schemes:
- flows:
  - flow: authorizationCode
    note: 'OIDC Hybrid / authorization code flow with PAR + PKCE. Authorisation and token URLs are disclosed per data holder via the CDR Register data holder brand detail endpoint (accredited access only), so no concrete URLs can be recorded here.

      '
  name: CDR-FAPI-OAuth2
  profile: FAPI 1.0 Advanced
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
scope_count: 11
scope_names:
- energy:accounts.basic:read
- energy:accounts.detail:read
- energy:accounts.paymentschedule:read
- energy:accounts.concessions:read
- energy:billing:read
- energy:electricity.servicepoints.basic:read
- energy:electricity.servicepoints.detail:read
- energy:electricity.usage:read
- energy:electricity.der:read
- common:customer.basic:read
- common:customer.detail:read
scopes:
- description: Basic information about the customer's energy accounts with the retailer, including simple plan information and the service points that are part of the account. Does not include detailed account information.
  flows:
  - authorizationCode
  scope: energy:accounts.basic:read
- description: Detailed energy account information. Additional authorisation on top of the basic energy account scope.
  flows:
  - authorizationCode
  scope: energy:accounts.detail:read
- description: The agreed payment schedule for the customer's energy accounts.
  flows:
  - authorizationCode
  scope: energy:accounts.paymentschedule:read
- description: Concessions and rebates applied to the customer's energy accounts.
  flows:
  - authorizationCode
  scope: energy:accounts.concessions:read
- description: Billing data for the customer's energy accounts — account balances, invoices and billing transactions.
  flows:
  - authorizationCode
  scope: energy:billing:read
- description: Basic standing data for the customer's electricity service points, including the National Meter Identifier (NMI). Excludes location and meter attributes.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.basic:read
- description: Detailed service point connection information including meter information. Additional authorisation on top of the basic service point scope. Excludes meter usage data.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.detail:read
- description: Electricity usage data for the customer's service points, including basic and interval meter reads.
  flows:
  - authorizationCode
  scope: energy:electricity.usage:read
- description: Distributed energy resource data for the customer's service points, as available in AEMO's DER Register.
  flows:
  - authorizationCode
  scope: energy:electricity.der:read
- description: Basic information about the authorised customer (name or organisation, customer type).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Detailed customer information including contact details (phone numbers, email addresses, physical addresses).
  flows:
  - authorizationCode
  scope: common:customer.detail:read
slug: alinta-energy-scopes
source_filename: alinta-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/alinta-energy-cds-energy-api-openapi.yml + openapi/alinta-energy-cds-common-api-openapi.yml (x-scopes extension)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >\n  Alinta's publicly callable endpoints require NO scope: the CDR discovery pair\n  (/discovery/status, /discovery/outages) and the generic plan data endpoints\n  (/energy/plans, /energy/plans/{planId}) are unauthenticated and carry no x-scopes.\n  The scopes below govern the consumer-data-sharing operations in the shared DSB\n  Consumer Data Standards contract that Alinta implements as a designated energy data\n  holder, and are only obtainable by an ACCC-accredited Data Recipient holding a valid\n  consumer consent. Scope strings are captured verbatim from the specs' per-operation\n  x-scopes extension; descriptions are from the Consumer Data Standards authorisation\n  scopes reference.\nschemes:\n- name: CDR-FAPI-OAuth2\n\
  \  profile: FAPI 1.0 Advanced\n  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  flows:\n  - flow: authorizationCode\n    note: >\n      OIDC Hybrid / authorization code flow with PAR + PKCE. Authorisation and token\n      URLs are disclosed per data holder via the CDR Register data holder brand detail\n      endpoint (accredited access only), so no concrete URLs can be recorded here.\npublic_scope:\n  scope: Public\n  scope_id: N/A\n  description: >\n    Openly accessible information; a customer never grants this scope. Applies to the\n    generic plan data and discovery endpoints Alinta (and the AER on Alinta's behalf)\n    serve anonymously.\nscopes:\n- scope: energy:accounts.basic:read\n  description: >\n    Basic information about the customer's energy accounts with the retailer, including\n    simple plan information and the service points that are part of the account. Does not\n    include detailed account information.\n  flows: [authorizationCode]\n\
  \  operations: [listEnergyAccounts]\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:accounts.detail:read\n  description: >\n    Detailed energy account information. Additional authorisation on top of the basic\n    energy account scope.\n  flows: [authorizationCode]\n  operations: [getEnergyAccountDetail]\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:accounts.paymentschedule:read\n  description: The agreed payment schedule for the customer's energy accounts.\n  flows: [authorizationCode]\n  operations: [getEnergyAccountPaymentSchedule]\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:accounts.concessions:read\n  description: Concessions and rebates applied to the customer's energy accounts.\n  flows: [authorizationCode]\n  operations: [getEnergyAccountConcessions]\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:billing:read\n  description: >\n    Billing data\
  \ for the customer's energy accounts — account balances, invoices and\n    billing transactions.\n  flows: [authorizationCode]\n  operations:\n  - getEnergyAccountBalance\n  - listEnergyAccountBalancesBulk\n  - listEnergyAccountBalancesSpecificAccounts\n  - getEnergyAccountInvoices\n  - listEnergyAccountInvoicesBulk\n  - listEnergyInvoicesForSpecificAccounts\n  - getBillingForEnergyAccount\n  - listEnergyAccountBillingBulk\n  - listEnergyAccountBillingForSpecificAccounts\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:electricity.servicepoints.basic:read\n  description: >\n    Basic standing data for the customer's electricity service points, including the\n    National Meter Identifier (NMI). Excludes location and meter attributes.\n  flows: [authorizationCode]\n  operations: [listElectricityServicePoints]\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:electricity.servicepoints.detail:read\n  description: >\n    Detailed\
  \ service point connection information including meter information. Additional\n    authorisation on top of the basic service point scope. Excludes meter usage data.\n  flows: [authorizationCode]\n  operations: [getElectricityServicePointDetail]\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:electricity.usage:read\n  description: >\n    Electricity usage data for the customer's service points, including basic and\n    interval meter reads.\n  flows: [authorizationCode]\n  operations:\n  - getElectricityServicePointUsage\n  - listElectricityUsageBulk\n  - listElectricityUsageForServicePoints\n  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: energy:electricity.der:read\n  description: >\n    Distributed energy resource data for the customer's service points, as available in\n    AEMO's DER Register.\n  flows: [authorizationCode]\n  operations:\n  - getElectricityDERForServicePoint\n  - listElectricityDERBulk\n  - listElectricityDERForSpecificServicePoints\n\
  \  sources: [openapi/alinta-energy-cds-energy-api-openapi.yml]\n- scope: common:customer.basic:read\n  description: Basic information about the authorised customer (name or organisation, customer type).\n  flows: [authorizationCode]\n  operations: [getCustomer]\n  sources: [openapi/alinta-energy-cds-common-api-openapi.yml]\n- scope: common:customer.detail:read\n  description: >\n    Detailed customer information including contact details (phone numbers, email\n    addresses, physical addresses).\n  flows: [authorizationCode]\n  operations: [getCustomerDetail]\n  sources: [openapi/alinta-energy-cds-common-api-openapi.yml]\noidc_scopes:\n- scope: openid\n  description: Required OpenID Connect scope for the CDR authorisation flow.\n- scope: profile\n  description: Basic profile information of the authenticated end-user (CDR Profile Scope).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/scopes/alinta-energy-scopes.yml
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
- Open Energy Data
- Smart Metering
- Renewables
- Generation
token_urls: []
---
