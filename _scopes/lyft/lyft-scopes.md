---
api_specs:
- filename: lyft-concierge-rides-api-openapi.yml
  format: yaml
  label: lyft Concierge Rides API
  slug: lyft-concierge-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-concierge-rides-api-openapi.yml
- filename: lyft-cost-estimates-api-openapi.yml
  format: yaml
  label: lyft Cost Estimates API
  slug: lyft-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-cost-estimates-api-openapi.yml
- filename: lyft-drivers-api-openapi.yml
  format: yaml
  label: lyft Drivers API
  slug: lyft-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-drivers-api-openapi.yml
- filename: lyft-eta-api-openapi.yml
  format: yaml
  label: lyft ETA API
  slug: lyft-eta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-eta-api-openapi.yml
- filename: lyft-profile-api-openapi.yml
  format: yaml
  label: lyft Profile API
  slug: lyft-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-profile-api-openapi.yml
- filename: lyft-ride-types-api-openapi.yml
  format: yaml
  label: lyft Ride Types API
  slug: lyft-ride-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-ride-types-api-openapi.yml
- filename: lyft-rides-api-openapi.yml
  format: yaml
  label: lyft Rides API
  slug: lyft-rides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/openapi/lyft-rides-api-openapi.yml
authorization_urls: []
description: 'The complete OAuth 2.0 scope vocabulary Lyft publishes for api.lyft.com, read verbatim from the provider''s own RFC 8414 authorization-server metadata. Lyft''s developer portal is login-gated, so this anonymous discovery document is the only public source for the scope vocabulary; no scope reference page is publicly readable and Lyft publishes no human-readable description for any individual scope, so none is recorded here. The family: grouping is our own, derived from the scope prefix.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Lyft Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lyft publishes 47 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lyft API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lyft
provider_slug: lyft
schemes: []
scope_count: 47
scope_names:
- autonomouspartners.set
- driver.details.address
- driver.details.basic
- driver.details.license
- drivers.tracking.read
- enterprise.support_tickets.create
- external_supply_integrator
- lb.ride_costs.get
- lb.ride_receipts.get
- lb.rides.cancel
- lb.rides.dispatch
- lb.rides.update
- loyalty_tier
- lus_partnership.account_management
- lyft_enterprise.admin_access
- lyft_rewards.usage
- lyft_rider_mcp.read
- memberships.updates_subscribe
- offline
- openid
- privileged.admin
- privileged.b2b_payouts.boomi_partner_records
- privileged.driver.tax.summary
- privileged.enterprise.dell_boomi
- privileged.enterprise.invoices
- privileged.enterprise.ride_program
- privileged.mobility.rides
- privileged.price.upfront
- privileged.rides.additional_fields.drivers_license
- privileged.rides.dispatch
- privileged.wav_dispatch
- profile
- profile.email
- profile.phone
- public
- rides.active_ride
- rides.read
- rides.request
- rides.subscribe_all
- rides.subscribe_ride_receipt
- rides.subscribe_ride_request
- routes.read
- scopedurl
- tapi.atms.webhook
- transportation_api.trip_insights
- transportation_api.trips
- users.create
scopes:
- description: ''
  flows: []
  scope: autonomouspartners.set
- description: ''
  flows: []
  scope: driver.details.address
- description: ''
  flows: []
  scope: driver.details.basic
- description: ''
  flows: []
  scope: driver.details.license
- description: ''
  flows: []
  scope: drivers.tracking.read
- description: ''
  flows: []
  scope: enterprise.support_tickets.create
- description: ''
  flows: []
  scope: external_supply_integrator
- description: ''
  flows: []
  scope: lb.ride_costs.get
- description: ''
  flows: []
  scope: lb.ride_receipts.get
- description: ''
  flows: []
  scope: lb.rides.cancel
- description: ''
  flows: []
  scope: lb.rides.dispatch
- description: ''
  flows: []
  scope: lb.rides.update
- description: ''
  flows: []
  scope: loyalty_tier
- description: ''
  flows: []
  scope: lus_partnership.account_management
- description: ''
  flows: []
  scope: lyft_enterprise.admin_access
- description: ''
  flows: []
  scope: lyft_rewards.usage
- description: ''
  flows: []
  scope: lyft_rider_mcp.read
- description: ''
  flows: []
  scope: memberships.updates_subscribe
- description: ''
  flows: []
  scope: offline
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: privileged.admin
- description: ''
  flows: []
  scope: privileged.b2b_payouts.boomi_partner_records
- description: ''
  flows: []
  scope: privileged.driver.tax.summary
- description: ''
  flows: []
  scope: privileged.enterprise.dell_boomi
- description: ''
  flows: []
  scope: privileged.enterprise.invoices
- description: ''
  flows: []
  scope: privileged.enterprise.ride_program
- description: ''
  flows: []
  scope: privileged.mobility.rides
- description: ''
  flows: []
  scope: privileged.price.upfront
- description: ''
  flows: []
  scope: privileged.rides.additional_fields.drivers_license
- description: ''
  flows: []
  scope: privileged.rides.dispatch
- description: ''
  flows: []
  scope: privileged.wav_dispatch
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: profile.email
- description: ''
  flows: []
  scope: profile.phone
- description: ''
  flows: []
  scope: public
- description: ''
  flows: []
  scope: rides.active_ride
- description: ''
  flows: []
  scope: rides.read
- description: ''
  flows: []
  scope: rides.request
- description: ''
  flows: []
  scope: rides.subscribe_all
- description: ''
  flows: []
  scope: rides.subscribe_ride_receipt
- description: ''
  flows: []
  scope: rides.subscribe_ride_request
- description: ''
  flows: []
  scope: routes.read
- description: ''
  flows: []
  scope: scopedurl
- description: ''
  flows: []
  scope: tapi.atms.webhook
- description: ''
  flows: []
  scope: transportation_api.trip_insights
- description: ''
  flows: []
  scope: transportation_api.trips
- description: ''
  flows: []
  scope: users.create
slug: lyft-scopes
source_filename: lyft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: lyft\nproviderId: lyft\ngenerated: '2026-09-17'\nmethod: probed\nsource: https://api.lyft.com/.well-known/oauth-authorization-server\ndescription: 'The complete OAuth 2.0 scope vocabulary Lyft publishes for api.lyft.com, read verbatim from\n  the provider''s own RFC 8414 authorization-server metadata. Lyft''s developer portal is login-gated,\n  so this anonymous discovery document is the only public source for the scope vocabulary; no scope reference\n  page is publicly readable and Lyft publishes no human-readable description for any individual scope,\n  so none is recorded here. The family: grouping is our own, derived from the scope prefix.'\ndocs: null\ndocs_note: 'No publicly readable scope/permission reference page: https://www.lyft.com/developers 302s\n  to https://account.lyft.com/auth/email.'\nissuer: https://api.lyft.com\nauthorization_endpoint: https://api.lyft.com/oauth/authorize\ntoken_endpoint:\
  \ https://api.lyft.com/oauth/token\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\ncode_challenge_methods_supported:\n- S256\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- none\nscope_count: 47\nscopes:\n- scope: autonomouspartners.set\n  family: other\n- scope: driver.details.address\n  family: driver\n- scope: driver.details.basic\n  family: driver\n- scope: driver.details.license\n  family: driver\n- scope: drivers.tracking.read\n  family: driver\n- scope: enterprise.support_tickets.create\n  family: enterprise\n- scope: external_supply_integrator\n  family: other\n- scope: lb.ride_costs.get\n  family: lyft-business\n- scope: lb.ride_receipts.get\n  family: lyft-business\n- scope: lb.rides.cancel\n  family: lyft-business\n- scope: lb.rides.dispatch\n  family: lyft-business\n- scope: lb.rides.update\n  family: lyft-business\n- scope: loyalty_tier\n  family: openid-connect-and-core\n- scope: lus_partnership.account_management\n\
  \  family: other\n- scope: lyft_enterprise.admin_access\n  family: enterprise\n- scope: lyft_rewards.usage\n  family: memberships-and-rewards\n- scope: lyft_rider_mcp.read\n  family: agent/mcp\n- scope: memberships.updates_subscribe\n  family: memberships-and-rewards\n- scope: offline\n  family: openid-connect-and-core\n- scope: openid\n  family: openid-connect-and-core\n- scope: privileged.admin\n  family: privileged (partner-restricted)\n- scope: privileged.b2b_payouts.boomi_partner_records\n  family: privileged (partner-restricted)\n- scope: privileged.driver.tax.summary\n  family: privileged (partner-restricted)\n- scope: privileged.enterprise.dell_boomi\n  family: privileged (partner-restricted)\n- scope: privileged.enterprise.invoices\n  family: privileged (partner-restricted)\n- scope: privileged.enterprise.ride_program\n  family: privileged (partner-restricted)\n- scope: privileged.mobility.rides\n  family: privileged (partner-restricted)\n- scope: privileged.price.upfront\n  family:\
  \ privileged (partner-restricted)\n- scope: privileged.rides.additional_fields.drivers_license\n  family: privileged (partner-restricted)\n- scope: privileged.rides.dispatch\n  family: privileged (partner-restricted)\n- scope: privileged.wav_dispatch\n  family: privileged (partner-restricted)\n- scope: profile\n  family: openid-connect-and-core\n- scope: profile.email\n  family: profile\n- scope: profile.phone\n  family: profile\n- scope: public\n  family: openid-connect-and-core\n- scope: rides.active_ride\n  family: rider-rides\n- scope: rides.read\n  family: rider-rides\n- scope: rides.request\n  family: rider-rides\n- scope: rides.subscribe_all\n  family: rider-rides\n- scope: rides.subscribe_ride_receipt\n  family: rider-rides\n- scope: rides.subscribe_ride_request\n  family: rider-rides\n- scope: routes.read\n  family: rider-rides\n- scope: scopedurl\n  family: openid-connect-and-core\n- scope: tapi.atms.webhook\n  family: transportation-api\n- scope: transportation_api.trip_insights\n\
  \  family: transportation-api\n- scope: transportation_api.trips\n  family: transportation-api\n- scope: users.create\n  family: other\nnotes:\n- openid + profile + offline are present, but api.lyft.com serves no /.well-known/openid-configuration\n  (404), so the OIDC discovery document is absent even though OIDC scopes are advertised.\n- lyft_rider_mcp.read is an MCP-specific scope in the published vocabulary — first-party evidence that\n  an MCP surface exists behind authentication. No anonymously reachable MCP endpoint was found (see mcp/lyft-mcp.yml).\n- rides.subscribe_all, rides.subscribe_ride_request, rides.subscribe_ride_receipt, memberships.updates_subscribe\n  and tapi.atms.webhook are subscription/webhook scopes (see asyncapi/lyft-webhooks.yml).\n- The 18 operations in openapi/ are covered by a small part of this vocabulary; most scopes belong to\n  Lyft Business, enterprise, driver and privileged partner surfaces that publish no public contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lyft/refs/heads/main/scopes/lyft-scopes.yml
summary_line: 47 scopes
tags:
- Transportation
- Mobility
- Ride Hailing
- Micromobility
- Bike Share
- Scooters
- GBFS
- Logistics
- Travel
token_urls: []
---
