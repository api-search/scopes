---
api_specs:
- filename: guestready-rentalready-openapi.yml
  format: yaml
  label: RentalReady API
  slug: rentalready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guestready/refs/heads/main/openapi/guestready-rentalready-openapi.yml
authorization_urls:
- /o/authorize/
description: ''
docs: https://pms.rentalready.io/api/v3/schema/swagger-ui/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Guestready Scopes
name_suffix: OAuth Scopes
note: RentalReady publishes no standalone scopes or permissions reference page. The authoritative scope list is the OAuth 2.0 securityScheme inside the specification the provider serves anonymously at https://pms.rentalready.io/api/v3/schema/, rendered for humans at its Swagger UI. The provider's own client-examples repository publishes a working SCOPES string in python/.env.example naming 24 of these scopes, which corroborates the spec but is a strict subset of it — the spec is the superset and is what is recorded here. Descriptions below are the provider's own verbatim scope labels. Two scopes carry a deprecation marker in their own label (hosts:read, hosts:write, both "(deprecated)"); see lifecycle/guestready-lifecycle.yml.
overview: 'GuestReady publishes 54 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GuestReady API on a user''s behalf.


  Tokens are issued from /o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GuestReady
provider_slug: guestready
schemes:
- flows:
  - authorizationUrl: /o/authorize/
    flow: authorizationCode
    tokenUrl: /o/token/
  name: oauth2
  source: openapi/guestready-rentalready-openapi.yml
scope_count: 54
scope_names:
- accounting_invoice:read
- accounting_invoice:write
- agents:read
- amenities:read
- amenities:write
- blacklist:read
- calendar:read
- calendar:write
- city_tax_rules:read
- conversations:read
- conversations:write
- custom_fields:read
- custom_fields:write
- guest_registration:read
- hosts:read
- hosts:write
- incidents:read
- incidents:write
- inquiries:read
- issues:read
- issues:write
- listing_requests:read
- messages:read
- messages:write
- missions:read
- missions:write
- neighbourhoods:read
- offices:read
- onboarding_requests:read
- owners:read
- owners:write
- payment_acceptance_transactions:read
- payment_acceptance_transactions:write
- payment_links:read
- payout_adjustments:read
- payout_adjustments:write
- photos:write
- pricing:read
- pricing:write
- property_managers:read
- read
- rentals:read
- rentals:write
- reservation_platform:read
- reservations:read
- reservations:write
- reviews:read
- reviews:write
- smart_schedulers:read
- smart_schedulers:write
- swikly_deposits:read
- users:read
- vouchers:read
- write
scopes:
- description: Read accounting invoices
  flows:
  - authorizationCode
  scope: accounting_invoice:read
- description: Write accounting invoices
  flows:
  - authorizationCode
  scope: accounting_invoice:write
- description: Read agents
  flows:
  - authorizationCode
  scope: agents:read
- description: Read amenities
  flows:
  - authorizationCode
  scope: amenities:read
- description: Create, update and delete amenities
  flows:
  - authorizationCode
  scope: amenities:write
- description: ''
  flows: []
  scope: blacklist:read
- description: Read calendar
  flows:
  - authorizationCode
  scope: calendar:read
- description: Write calendar
  flows:
  - authorizationCode
  scope: calendar:write
- description: Read city tax rules
  flows:
  - authorizationCode
  scope: city_tax_rules:read
- description: Read conversations
  flows:
  - authorizationCode
  scope: conversations:read
- description: Write conversations
  flows:
  - authorizationCode
  scope: conversations:write
- description: Read custom fields
  flows:
  - authorizationCode
  scope: custom_fields:read
- description: Write custom fields
  flows:
  - authorizationCode
  scope: custom_fields:write
- description: Read guest registration data
  flows:
  - authorizationCode
  scope: guest_registration:read
- description: Read hosts (deprecated)
  flows:
  - authorizationCode
  scope: hosts:read
- description: Write hosts (deprecated)
  flows:
  - authorizationCode
  scope: hosts:write
- description: Read incidents
  flows:
  - authorizationCode
  scope: incidents:read
- description: Write incidents
  flows:
  - authorizationCode
  scope: incidents:write
- description: Read inquiries
  flows:
  - authorizationCode
  scope: inquiries:read
- description: Read issues
  flows:
  - authorizationCode
  scope: issues:read
- description: Write issues
  flows:
  - authorizationCode
  scope: issues:write
- description: Read listing requests
  flows:
  - authorizationCode
  scope: listing_requests:read
- description: Read messages
  flows:
  - authorizationCode
  scope: messages:read
- description: Write messages
  flows:
  - authorizationCode
  scope: messages:write
- description: Read missions
  flows:
  - authorizationCode
  scope: missions:read
- description: Write missions
  flows:
  - authorizationCode
  scope: missions:write
- description: Read neighbourhoods
  flows:
  - authorizationCode
  scope: neighbourhoods:read
- description: Read offices
  flows:
  - authorizationCode
  scope: offices:read
- description: Read onboarding requests
  flows:
  - authorizationCode
  scope: onboarding_requests:read
- description: Read owners
  flows:
  - authorizationCode
  scope: owners:read
- description: Write owners
  flows:
  - authorizationCode
  scope: owners:write
- description: Read payment acceptance transactions
  flows:
  - authorizationCode
  scope: payment_acceptance_transactions:read
- description: Write payment acceptance transactions
  flows:
  - authorizationCode
  scope: payment_acceptance_transactions:write
- description: Read payment links
  flows:
  - authorizationCode
  scope: payment_links:read
- description: Read payout adjustments
  flows:
  - authorizationCode
  scope: payout_adjustments:read
- description: Write payout adjustments
  flows:
  - authorizationCode
  scope: payout_adjustments:write
- description: Create, update and delete photos
  flows:
  - authorizationCode
  scope: photos:write
- description: Read pricing
  flows:
  - authorizationCode
  scope: pricing:read
- description: Create, update and delete pricing
  flows:
  - authorizationCode
  scope: pricing:write
- description: Read property managers
  flows:
  - authorizationCode
  scope: property_managers:read
- description: Read scope
  flows:
  - authorizationCode
  scope: read
- description: Read rentals
  flows:
  - authorizationCode
  scope: rentals:read
- description: Create, update and delete rentals
  flows:
  - authorizationCode
  scope: rentals:write
- description: Read reservation platform
  flows:
  - authorizationCode
  scope: reservation_platform:read
- description: Read reservations
  flows:
  - authorizationCode
  scope: reservations:read
- description: Create, update and cancel reservations
  flows:
  - authorizationCode
  scope: reservations:write
- description: Read reviews
  flows:
  - authorizationCode
  scope: reviews:read
- description: Write reviews
  flows:
  - authorizationCode
  scope: reviews:write
- description: Read smart schedulers
  flows:
  - authorizationCode
  scope: smart_schedulers:read
- description: Write smart schedulers
  flows:
  - authorizationCode
  scope: smart_schedulers:write
- description: Read swikly deposits
  flows:
  - authorizationCode
  scope: swikly_deposits:read
- description: Read user data
  flows:
  - authorizationCode
  scope: users:read
- description: ''
  flows: []
  scope: vouchers:read
- description: Write scope
  flows:
  - authorizationCode
  scope: write
slug: guestready-scopes
source_filename: guestready-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://pms.rentalready.io/api/v3/schema/\ndocs: https://pms.rentalready.io/api/v3/schema/swagger-ui/\nalso:\n- https://github.com/guestready/rentalready-api-client-examples/blob/main/python/.env.example\nnote: >-\n  RentalReady publishes no standalone scopes or permissions reference page. The authoritative scope list is\n  the OAuth 2.0 securityScheme inside the specification the provider serves anonymously at\n  https://pms.rentalready.io/api/v3/schema/, rendered for humans at its Swagger UI. The provider's own\n  client-examples repository publishes a working SCOPES string in python/.env.example naming 24 of these\n  scopes, which corroborates the spec but is a strict subset of it — the spec is the superset and is what\n  is recorded here. Descriptions below are the provider's own verbatim scope labels. Two scopes carry a\n  deprecation marker in their own label (hosts:read, hosts:write, both \"(deprecated)\"); see\n  lifecycle/guestready-lifecycle.yml.\n\
  authorization_url: https://pms.rentalready.io/o/authorize/\ntoken_url: https://pms.rentalready.io/o/token/\ngrant: authorization_code\nauthorization_code_ttl_seconds: 60\nschemes:\n- name: oauth2\n  source: openapi/guestready-rentalready-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /o/authorize/\n    tokenUrl: /o/token/\nscopes:\n- scope: accounting_invoice:read\n  description: Read accounting invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: accounting_invoice:write\n  description: Write accounting invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: agents:read\n  description: Read agents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: amenities:read\n  description: Read amenities\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope:\
  \ amenities:write\n  description: Create, update and delete amenities\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: blacklist:read\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: calendar:read\n  description: Read calendar\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: calendar:write\n  description: Write calendar\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: city_tax_rules:read\n  description: Read city tax rules\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: conversations:read\n  description: Read conversations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: conversations:write\n  description: Write conversations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n\
  - scope: custom_fields:read\n  description: Read custom fields\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: custom_fields:write\n  description: Write custom fields\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: guest_registration:read\n  description: Read guest registration data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: hosts:read\n  description: Read hosts (deprecated)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: hosts:write\n  description: Write hosts (deprecated)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: incidents:read\n  description: Read incidents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: incidents:write\n  description: Write incidents\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: inquiries:read\n  description: Read inquiries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: issues:read\n  description: Read issues\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: issues:write\n  description: Write issues\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: listing_requests:read\n  description: Read listing requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: messages:read\n  description: Read messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: messages:write\n  description: Write messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: missions:read\n\
  \  description: Read missions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: missions:write\n  description: Write missions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: neighbourhoods:read\n  description: Read neighbourhoods\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: offices:read\n  description: Read offices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: onboarding_requests:read\n  description: Read onboarding requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: owners:read\n  description: Read owners\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: owners:write\n  description: Write owners\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n\
  - scope: payment_acceptance_transactions:read\n  description: Read payment acceptance transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: payment_acceptance_transactions:write\n  description: Write payment acceptance transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: payment_links:read\n  description: Read payment links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: payout_adjustments:read\n  description: Read payout adjustments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: payout_adjustments:write\n  description: Write payout adjustments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: photos:write\n  description: Create, update and delete photos\n  flows:\n  - authorizationCode\n  sources:\n \
  \ - openapi/guestready-rentalready-openapi.yml\n- scope: pricing:read\n  description: Read pricing\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: pricing:write\n  description: Create, update and delete pricing\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: property_managers:read\n  description: Read property managers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: read\n  description: Read scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: rentals:read\n  description: Read rentals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: rentals:write\n  description: Create, update and delete rentals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: reservation_platform:read\n\
  \  description: Read reservation platform\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: reservations:read\n  description: Read reservations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: reservations:write\n  description: Create, update and cancel reservations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: reviews:read\n  description: Read reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: reviews:write\n  description: Write reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: smart_schedulers:read\n  description: Read smart schedulers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: smart_schedulers:write\n  description: Write smart schedulers\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: swikly_deposits:read\n  description: Read swikly deposits\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: users:read\n  description: Read user data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: vouchers:read\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n- scope: write\n  description: Write scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/guestready-rentalready-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guestready/refs/heads/main/scopes/guestready-scopes.yml
summary_line: 54 scopes · authorizationCode
tags:
- Property Management
- Short Term Rentals
- Vacation Rentals
- Hospitality
- Travel
- Real Estate
- Channel Management
- Reservations
- Revenue Management
- PMS
- MCP
- OAuth
token_urls:
- /o/token/
---
