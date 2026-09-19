---
api_specs:
- filename: agendapro-available-slots-api-openapi.yml
  format: yaml
  label: AgendaPro Available Slots API
  slug: agendapro-available-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-available-slots-api-openapi.yml
- filename: agendapro-bookings-api-openapi.yml
  format: yaml
  label: AgendaPro Bookings API
  slug: agendapro-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-bookings-api-openapi.yml
- filename: agendapro-carts-api-openapi.yml
  format: yaml
  label: AgendaPro Carts API
  slug: agendapro-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-carts-api-openapi.yml
- filename: agendapro-clients-api-openapi.yml
  format: yaml
  label: AgendaPro Clients API
  slug: agendapro-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-clients-api-openapi.yml
- filename: agendapro-custom-attributes-api-openapi.yml
  format: yaml
  label: AgendaPro Custom Attributes API
  slug: agendapro-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-custom-attributes-api-openapi.yml
- filename: agendapro-locations-api-openapi.yml
  format: yaml
  label: AgendaPro Locations API
  slug: agendapro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-locations-api-openapi.yml
- filename: agendapro-payment-requests-api-openapi.yml
  format: yaml
  label: AgendaPro Payment Requests API
  slug: agendapro-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-payment-requests-api-openapi.yml
- filename: agendapro-providers-api-openapi.yml
  format: yaml
  label: AgendaPro Providers API
  slug: agendapro-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-providers-api-openapi.yml
- filename: agendapro-sales-api-openapi.yml
  format: yaml
  label: AgendaPro Sales API
  slug: agendapro-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-sales-api-openapi.yml
- filename: agendapro-services-api-openapi.yml
  format: yaml
  label: AgendaPro Services API
  slug: agendapro-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/openapi/agendapro-services-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.agendapro.com/reference/getting-started-v3
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Agendapro Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AgendaPro uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AgendaPro
provider_slug: agendapro
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agendapro-scopes
source_filename: agendapro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://developers.agendapro.com/reference/getting-started-v3\ndocs: https://developers.agendapro.com/reference/getting-started-v3\nscheme:\n  kind: api-key-scopes\n  oauth2: false\n  note: AgendaPro publishes a real {resource}:{action} scope catalogue, but it is attached to a static per-company\n    API key rather than to OAuth 2.0 tokens. There is no authorization endpoint, no consent screen, and no token\n    exchange. The OAuthScopes pointer is used because it is the canonical type for a published scope reference;\n    the authorization framework is NOT OAuth.\n  pattern: '{resource}:{action}'\n  empty_scopes_means_full_access: true\n  granted_at: API key creation, in Configuraciones > Integraciones\n  denial: 403 forbidden / scope_denied\nscope_count: 11\nscopes:\n- name: bookings:read\n  description: List and show bookings\n  operations:\n  - listBookings\n  - getBooking\n  - listAvailableSlots\n- name: bookings:write\n\
  \  description: Create, update, and cancel bookings\n  operations:\n  - createBooking\n  - updateBooking\n  - cancelBooking\n- name: clients:read\n  description: List and show clients\n  operations:\n  - listClients\n  - getClient\n  - quickSearchClients\n  - listClientCustomAttributes\n- name: clients:write\n  description: Create and update clients\n  operations:\n  - createClient\n  - updateClient\n  - deactivateClient\n- name: locations:read\n  description: List and show locations\n  operations:\n  - listLocations\n  - getLocation\n- name: services:read\n  description: List and show services\n  operations:\n  - listServices\n  - getService\n  - listCategories\n- name: providers:read\n  description: List and show providers\n  operations:\n  - listProviders\n  - getProvider\n- name: custom_attributes:read\n  description: List custom attribute templates\n  operations:\n  - listCustomAttributeTemplates\n- name: sales:read\n  description: List and show sales\n  operations:\n  - listSales\n\
  \  - getSale\n- name: carts:write\n  description: Create and update carts and create payment requests\n  operations:\n  - createCart\n  - updateCart\n  - getCart\n  - createPaymentRequest\n- name: payment_requests:write\n  description: Cancel a pending payment request\n  operations:\n  - cancelPaymentRequest\nnotes:\n- Nine scopes are enumerated in the OpenAPI info.description scope table. carts:write and payment_requests:write\n  are NOT in that table but are named as required scopes in the per-operation error dictionaries for the cart and\n  payment-request endpoints; both are recorded here with that provenance so the catalogue matches the enforced surface.\n- No write scope exists for locations, services, categories, providers or sales — those resources are read-only\n  through the public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agendapro/refs/heads/main/scopes/agendapro-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Appointment Scheduling
- Booking
- Salon Software
- Spa and Wellness
- Point-of-Sale
- Clinic Management
- CRM
- Payments
- Webhook
- Vertical SaaS
- Latin America
- SMB Software
token_urls: []
---
