---
api_specs:
- filename: energy-queensland-data-holder-customers-api-openapi.yml
  format: yaml
  label: Energy Queensland Data Holder Customers API
  slug: energy-queensland-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-data-holder-customers-api-openapi.yml
- filename: energy-queensland-data-holder-operations-api-openapi.yml
  format: yaml
  label: Energy Queensland Data Holder Operations API
  slug: energy-queensland-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-data-holder-operations-api-openapi.yml
- filename: energy-queensland-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: Energy Queensland Distributed Energy Resources API
  slug: energy-queensland-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-distributed-energy-resources-api-openapi.yml
- filename: energy-queensland-electricity-service-points-api-openapi.yml
  format: yaml
  label: Energy Queensland Electricity Service Points API
  slug: energy-queensland-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-electricity-service-points-api-openapi.yml
- filename: energy-queensland-electricity-usage-api-openapi.yml
  format: yaml
  label: Energy Queensland Electricity Usage API
  slug: energy-queensland-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-electricity-usage-api-openapi.yml
- filename: energy-queensland-energy-account-balances-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Account Balances API
  slug: energy-queensland-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-account-balances-api-openapi.yml
- filename: energy-queensland-energy-account-billing-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Account Billing API
  slug: energy-queensland-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-account-billing-api-openapi.yml
- filename: energy-queensland-energy-accounts-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Accounts API
  slug: energy-queensland-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-accounts-api-openapi.yml
- filename: energy-queensland-energy-plans-api-openapi.yml
  format: yaml
  label: Energy Queensland Energy Plans API
  slug: energy-queensland-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/openapi/energy-queensland-energy-plans-api-openapi.yml
authorization_urls:
- not publicly discoverable (authenticated CDR Register only)
description: 'The OAuth2 authorisation scopes that govern Ergon Energy Retail''s Consumer Data Right energy surface. These scopes are NOT defined by Energy Queensland - they are set centrally by the Treasury Data Standards Body and are identical for all 84 registered Australian energy data holder brands. No scope can be requested by a caller who is not an ACCC-accredited data recipient, and every scope is consented to by the individual customer through the data holder''s authorisation flow. The two anonymously callable surfaces recorded in apis.yml (Get Generic Plans / Get Generic Plan Detail on the AER host, Get Status / Get Outages on Ergon''s public base URI) carry NO x-scopes at all and require no token; that absence is itself recorded below. No OAuth2 securityScheme is declared in the harvested OpenAPI documents - the DSB publishes the security model in the Security Profile section of the standard rather than in the swagger - so these scopes were read from the per-operation x-scopes
  extension, not from a flows map. Anonymous discovery of the token/authorisation endpoints was attempted and failed by design: GET https://public.cdr.ergonretail.com.au/.well-known/openid-configuration and /.well-known/oauth-authorization-server both returned HTTP 404 on 2026-07-27, because a CDR data holder publishes its infosec base URI through the authenticated portion of the CDR Register, not publicly.'
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Energy Queensland Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Energy Queensland publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Energy Queensland API on a user''s behalf.


  Tokens are issued from not publicly discoverable (authenticated CDR Register only).


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Energy Queensland
provider_slug: energy-queensland
schemes:
- flows:
  - authorizationUrl: not publicly discoverable (authenticated CDR Register only)
    flow: authorizationCode
    notes: Authorization code flow with PKCE and Pushed Authorization Requests, OIDC id_token, private_key_jwt client authentication, and mutual TLS sender-constrained tokens. Client registration is dynamic (CDR DCR) using a software statement assertion issued by the CDR Register.
    tokenUrl: not publicly discoverable (authenticated CDR Register only)
  name: CDR OAuth2 (FAPI 1.0 Advanced profile)
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
- description: Mandatory OIDC scope for the CDR authorisation flow. Required on every consent request under the Security Profile.
  flows:
  - authorizationCode
  scope: openid
- description: OIDC profile scope. Supported in the CDR authorisation flow alongside the CDR data scopes.
  flows:
  - authorizationCode
  scope: profile
- description: Name and occupation for an individual, or organisation name and industry for a business.
  flows: []
  scope: common:customer.basic:read
- description: Phone, email, mail address and residential address of the customer.
  flows: []
  scope: common:customer.detail:read
- description: Account name, type, creation date and plan overview for the customer's energy accounts.
  flows: []
  scope: energy:accounts.basic:read
- description: Full account detail including the plan the account is on, authorised contacts, tariff and contract detail.
  flows: []
  scope: energy:accounts.detail:read
- description: Concessions and rebates applied to the customer's energy account.
  flows: []
  scope: energy:accounts.concessions:read
- description: The agreed payment schedule on the account (direct debit, card debit, digital wallet or manual).
  flows: []
  scope: energy:accounts.paymentschedule:read
- description: Account balances, invoices and billing transactions - the largest single scope on the energy surface, covering seven operations.
  flows: []
  scope: energy:billing:read
- description: Basic electricity service point data - national metering identifier, jurisdiction, classification and status.
  flows: []
  scope: energy:electricity.servicepoints.basic:read
- description: Detailed service point data - meters, registers, distribution loss factor, location and related market participants.
  flows: []
  scope: energy:electricity.servicepoints.detail:read
- description: Interval and basic metering reads for a service point. Sourced from AEMO as the CDR secondary data holder under the Shared Responsibility model.
  flows: []
  scope: energy:electricity.usage:read
- description: Distributed energy resource records for a service point - solar/battery AC connections, approved capacity, phases, protection mode and islandable installation flags. Sourced from the AEMO DER Register.
  flows: []
  scope: energy:electricity.der:read
slug: energy-queensland-scopes
source_filename: energy-queensland-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  x-scopes vendor extension on every operation in\n  openapi/energy-queensland-cds-energy-openapi.yml and\n  openapi/energy-queensland-cds-common-openapi.yml (DSB Consumer Data Standards\n  v1.36.0), cross-checked against the Authorisation Scopes section of the\n  published standard.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\ndescription: >-\n  The OAuth2 authorisation scopes that govern Ergon Energy Retail's Consumer\n  Data Right energy surface. These scopes are NOT defined by Energy Queensland -\n  they are set centrally by the Treasury Data Standards Body and are identical\n  for all 84 registered Australian energy data holder brands. No scope can be\n  requested by a caller who is not an ACCC-accredited data recipient, and every\n  scope is consented to by the individual customer through the data holder's\n  authorisation flow. The two anonymously callable surfaces recorded\
  \ in apis.yml\n  (Get Generic Plans / Get Generic Plan Detail on the AER host, Get Status /\n  Get Outages on Ergon's public base URI) carry NO x-scopes at all and require\n  no token; that absence is itself recorded below.\n  No OAuth2 securityScheme is declared in the harvested OpenAPI documents - the\n  DSB publishes the security model in the Security Profile section of the\n  standard rather than in the swagger - so these scopes were read from the\n  per-operation x-scopes extension, not from a flows map.\n  Anonymous discovery of the token/authorisation endpoints was attempted and\n  failed by design: GET https://public.cdr.ergonretail.com.au/.well-known/openid-configuration\n  and /.well-known/oauth-authorization-server both returned HTTP 404 on\n  2026-07-27, because a CDR data holder publishes its infosec base URI through\n  the authenticated portion of the CDR Register, not publicly.\nschemes:\n  - name: CDR OAuth2 (FAPI 1.0 Advanced profile)\n    source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: not publicly discoverable (authenticated CDR Register only)\n        tokenUrl: not publicly discoverable (authenticated CDR Register only)\n        notes: >-\n          Authorization code flow with PKCE and Pushed Authorization Requests,\n          OIDC id_token, private_key_jwt client authentication, and mutual TLS\n          sender-constrained tokens. Client registration is dynamic (CDR DCR)\n          using a software statement assertion issued by the CDR Register.\nscopes:\n  - scope: openid\n    description: >-\n      Mandatory OIDC scope for the CDR authorisation flow. Required on every\n      consent request under the Security Profile.\n    flows: [authorizationCode]\n    sources: [https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes]\n  - scope: profile\n    description: >-\n      OIDC profile scope. Supported in the CDR authorisation flow alongside the\n      CDR data scopes.\n\
  \    flows: [authorizationCode]\n    sources: [https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes]\n  - scope: common:customer.basic:read\n    description: Name and occupation for an individual, or organisation name and industry for a business.\n    operations: [getCustomer]\n    sources: [openapi/energy-queensland-cds-common-openapi.yml]\n  - scope: common:customer.detail:read\n    description: Phone, email, mail address and residential address of the customer.\n    operations: [getCustomerDetail]\n    sources: [openapi/energy-queensland-cds-common-openapi.yml]\n  - scope: energy:accounts.basic:read\n    description: Account name, type, creation date and plan overview for the customer's energy accounts.\n    operations: [listEnergyAccounts]\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:accounts.detail:read\n    description: >-\n      Full account detail including the plan the account is on, authorised\n      contacts,\
  \ tariff and contract detail.\n    operations: [getEnergyAccountDetail]\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:accounts.concessions:read\n    description: Concessions and rebates applied to the customer's energy account.\n    operations: [getEnergyAccountConcessions]\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:accounts.paymentschedule:read\n    description: The agreed payment schedule on the account (direct debit, card debit, digital wallet or manual).\n    operations: [getEnergyAccountPaymentSchedule]\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:billing:read\n    description: >-\n      Account balances, invoices and billing transactions - the largest single\n      scope on the energy surface, covering seven operations.\n    operations:\n      - listEnergyAccountBalancesBulk\n      - listEnergyAccountBalancesSpecificAccounts\n      - getEnergyAccountBalance\n    \
  \  - listEnergyAccountBillingBulk\n      - listEnergyAccountBillingForSpecificAccounts\n      - getBillingForEnergyAccount\n      - listEnergyAccountInvoicesBulk\n      - listEnergyInvoicesForSpecificAccounts\n      - getEnergyAccountInvoices\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:electricity.servicepoints.basic:read\n    description: >-\n      Basic electricity service point data - national metering identifier,\n      jurisdiction, classification and status.\n    operations: [listElectricityServicePoints]\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:electricity.servicepoints.detail:read\n    description: >-\n      Detailed service point data - meters, registers, distribution loss factor,\n      location and related market participants.\n    operations: [getElectricityServicePointDetail]\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:electricity.usage:read\n    description:\
  \ >-\n      Interval and basic metering reads for a service point. Sourced from AEMO\n      as the CDR secondary data holder under the Shared Responsibility model.\n    operations:\n      - listElectricityUsageBulk\n      - listElectricityUsageForServicePoints\n      - getElectricityServicePointUsage\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\n  - scope: energy:electricity.der:read\n    description: >-\n      Distributed energy resource records for a service point - solar/battery AC\n      connections, approved capacity, phases, protection mode and islandable\n      installation flags. Sourced from the AEMO DER Register.\n    operations:\n      - listElectricityDERBulk\n      - listElectricityDERForSpecificServicePoints\n      - getElectricityDERForServicePoint\n    sources: [openapi/energy-queensland-cds-energy-openapi.yml]\nunscoped_operations:\n  note: >-\n    These operations declare no x-scopes and are callable with no token at all.\n    Both were confirmed live\
  \ and anonymous on 2026-07-27.\n  operations:\n    - operationId: listEnergyPlans\n      surface: https://cdr.energymadeeasy.gov.au/ergon/cds-au/v1/energy/plans\n      auth: none (x-v header only)\n    - operationId: getEnergyPlanDetail\n      surface: https://cdr.energymadeeasy.gov.au/ergon/cds-au/v1/energy/plans/{planId}\n      auth: none (x-v header only, minimum version 3)\n    - operationId: getStatus\n      surface: https://public.cdr.ergonretail.com.au/cds-au/v1/discovery/status\n      auth: none (x-v header only)\n    - operationId: getOutages\n      surface: https://public.cdr.ergonretail.com.au/cds-au/v1/discovery/outages\n      auth: none (x-v header only)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-queensland/refs/heads/main/scopes/energy-queensland-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Energy Retail
- Consumer Data Right
- CDR
- Product Reference Data
- Queensland
- Smart Metering
- Solar
- DER
- Open Data
token_urls:
- not publicly discoverable (authenticated CDR Register only)
---
