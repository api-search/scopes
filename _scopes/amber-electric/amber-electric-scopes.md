---
api_specs:
- filename: amber-electric-sites-api-openapi.yml
  format: yaml
  label: Amber Electric Sites API
  slug: amber-electric-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/openapi/amber-electric-sites-api-openapi.yml
- filename: amber-electric-state-api-openapi.yml
  format: yaml
  label: Amber Electric State API
  slug: amber-electric-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/openapi/amber-electric-state-api-openapi.yml
authorization_urls:
- https://public.cdr.amber.com.au/connect/authorize
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#end-points
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Amber Electric Scopes
name_suffix: OAuth Scopes
note: Amber's own product API has no OAuth surface at all — it uses an unscoped bearer token minted in the customer app, so there are no scopes to record for it. Every scope below belongs to Amber's regulated Consumer Data Right energy data-holder surface and was read verbatim from the anonymously-served OpenID Connect discovery document at the CDR public base URI. The scope names and their meanings are defined by the Australian Data Standards Body; the descriptions here summarise the CDS energy and common data clusters those scopes unlock. Access requires ACCC accreditation as a data recipient — no general developer can obtain any of these.
overview: 'Amber Electric publishes 16 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Amber Electric API on a user''s behalf.


  Tokens are issued from https://secure.cdr.amber.com.au/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Amber Electric
provider_slug: amber-electric
schemes:
- flows:
  - authorizationUrl: https://public.cdr.amber.com.au/connect/authorize
    client_authentication: private_key_jwt
    flow: authorizationCode
    par_required: true
    pkce: S256
    pushedAuthorizationRequestUrl: https://secure.cdr.amber.com.au/connect/par
    tokenUrl: https://secure.cdr.amber.com.au/connect/token
  - flow: clientCredentials
    note: Used for the admin/metadata-update endpoints between the register and the data holder.
    tokenUrl: https://secure.cdr.amber.com.au/connect/token
  issuer: https://public.cdr.amber.com.au
  name: CDR OpenID Connect
  source: authentication/amber-electric-cdr-openid-configuration.json
scope_count: 16
scope_names:
- openid
- profile
- common:customer.basic:read
- common:customer.detail:read
- cdr:registration
- admin:metrics.basic:read
- admin:metadata:update
- energy:electricity.servicepoints.basic:read
- energy:electricity.servicepoints.detail:read
- energy:electricity.usage:read
- energy:electricity.der:read
- energy:accounts.basic:read
- energy:accounts.detail:read
- energy:accounts.paymentschedule:read
- energy:accounts.concessions:read
- energy:billing:read
scopes:
- description: OpenID Connect authentication — issue an ID token for the consenting consumer.
  flows:
  - authorizationCode
  scope: openid
- description: Consumer profile claims (name, given_name, family_name).
  flows:
  - authorizationCode
  scope: profile
- description: Basic customer identity — name or organisation name and customer type.
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Detailed customer record including contact details and addresses.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
- description: Dynamic client registration management for an accredited data recipient's software product.
  flows:
  - clientCredentials
  scope: cdr:registration
- description: Data-holder administration — read the CDR performance/availability metrics the standards require.
  flows:
  - clientCredentials
  scope: admin:metrics.basic:read
- description: Data-holder administration — accept a metadata-update notification from the CDR Register.
  flows:
  - clientCredentials
  scope: admin:metadata:update
- description: Basic electricity service point (NMI) records held for the consumer.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.basic:read
- description: Detailed service point records, including registered metering and network details.
  flows:
  - authorizationCode
  scope: energy:electricity.servicepoints.detail:read
- description: Interval-level electricity usage data for the consumer's service points.
  flows:
  - authorizationCode
  scope: energy:electricity.usage:read
- description: Distributed energy resource records — solar, battery and inverter installation details.
  flows:
  - authorizationCode
  scope: energy:electricity.der:read
- description: Basic energy account records held with the retailer.
  flows:
  - authorizationCode
  scope: energy:accounts.basic:read
- description: Detailed energy account records including plan and tariff detail.
  flows:
  - authorizationCode
  scope: energy:accounts.detail:read
- description: Payment schedules configured on the consumer's energy accounts.
  flows:
  - authorizationCode
  scope: energy:accounts.paymentschedule:read
- description: Concessions and rebates applied to the consumer's energy accounts.
  flows:
  - authorizationCode
  scope: energy:accounts.concessions:read
- description: Billing and invoice history for the consumer's energy accounts.
  flows:
  - authorizationCode
  scope: energy:billing:read
slug: amber-electric-scopes
source_filename: amber-electric-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://public.cdr.amber.com.au/.well-known/openid-configuration\nlocal_source: authentication/amber-electric-cdr-openid-configuration.json\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#end-points\nfetched: '2026-07-27'\nhttp_status: 200\nanonymous: true\nnote: >-\n  Amber's own product API has no OAuth surface at all — it uses an unscoped\n  bearer token minted in the customer app, so there are no scopes to record for\n  it. Every scope below belongs to Amber's regulated Consumer Data Right energy\n  data-holder surface and was read verbatim from the anonymously-served OpenID\n  Connect discovery document at the CDR public base URI. The scope names and\n  their meanings are defined by the Australian Data Standards Body; the\n  descriptions here summarise the CDS energy and common data clusters those\n  scopes unlock. Access requires ACCC accreditation as a data recipient — no\n  general developer can obtain\
  \ any of these.\nsurface: cdr\nschemes:\n- name: CDR OpenID Connect\n  issuer: https://public.cdr.amber.com.au\n  source: authentication/amber-electric-cdr-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://public.cdr.amber.com.au/connect/authorize\n    tokenUrl: https://secure.cdr.amber.com.au/connect/token\n    pushedAuthorizationRequestUrl: https://secure.cdr.amber.com.au/connect/par\n    par_required: true\n    client_authentication: private_key_jwt\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://secure.cdr.amber.com.au/connect/token\n    note: Used for the admin/metadata-update endpoints between the register and the data holder.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication — issue an ID token for the consenting consumer.\n  flows: [authorizationCode]\n- scope: profile\n  description: Consumer profile claims (name, given_name, family_name).\n  flows: [authorizationCode]\n- scope: common:customer.basic:read\n\
  \  description: Basic customer identity — name or organisation name and customer type.\n  flows: [authorizationCode]\n- scope: common:customer.detail:read\n  description: Detailed customer record including contact details and addresses.\n  flows: [authorizationCode]\n- scope: cdr:registration\n  description: Dynamic client registration management for an accredited data recipient's software product.\n  flows: [clientCredentials]\n- scope: admin:metrics.basic:read\n  description: Data-holder administration — read the CDR performance/availability metrics the standards require.\n  flows: [clientCredentials]\n- scope: admin:metadata:update\n  description: Data-holder administration — accept a metadata-update notification from the CDR Register.\n  flows: [clientCredentials]\n- scope: energy:electricity.servicepoints.basic:read\n  description: Basic electricity service point (NMI) records held for the consumer.\n  flows: [authorizationCode]\n- scope: energy:electricity.servicepoints.detail:read\n\
  \  description: Detailed service point records, including registered metering and network details.\n  flows: [authorizationCode]\n- scope: energy:electricity.usage:read\n  description: Interval-level electricity usage data for the consumer's service points.\n  flows: [authorizationCode]\n- scope: energy:electricity.der:read\n  description: Distributed energy resource records — solar, battery and inverter installation details.\n  flows: [authorizationCode]\n- scope: energy:accounts.basic:read\n  description: Basic energy account records held with the retailer.\n  flows: [authorizationCode]\n- scope: energy:accounts.detail:read\n  description: Detailed energy account records including plan and tariff detail.\n  flows: [authorizationCode]\n- scope: energy:accounts.paymentschedule:read\n  description: Payment schedules configured on the consumer's energy accounts.\n  flows: [authorizationCode]\n- scope: energy:accounts.concessions:read\n  description: Concessions and rebates applied to the\
  \ consumer's energy accounts.\n  flows: [authorizationCode]\n- scope: energy:billing:read\n  description: Billing and invoice history for the consumer's energy accounts.\n  flows: [authorizationCode]\nsummary:\n  scope_count: 16\n  energy_scopes: 9\n  common_scopes: 2\n  admin_scopes: 2\n  registration_scopes: 1\n  identity_scopes: 2\n  access_gate: accredited-only\n  note: >-\n    The presence of the complete energy cluster — service points, usage, DER,\n    accounts, payment schedule, concessions and billing — is the signature of a\n    full Consumer Data Standards energy build rather than a partial one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amber-electric/refs/heads/main/scopes/amber-electric-scopes.yml
summary_line: 16 scopes · authorizationCode/clientCredentials
tags:
- Energy
- Australia
- Electricity
- Utilities
- Consumer Data Right
- Energy Markets
- Renewables
- Solar
- Batteries
- DER
- Smart Metering
- Wholesale Pricing
token_urls:
- https://secure.cdr.amber.com.au/connect/token
---
