---
api_specs:
- filename: enphase-monitoring-api-openapi.json
  format: json
  label: Enphase Monitoring API
  slug: enphase-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/openapi/enphase-monitoring-api-openapi.json
- filename: enphase-commissioning-api-openapi.json
  format: json
  label: Enphase Commissioning API
  slug: enphase-commissioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/openapi/enphase-commissioning-api-openapi.json
- filename: enphase-vpp-api-openapi.json
  format: json
  label: Enphase VPP API
  slug: enphase-vpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/openapi/enphase-vpp-api-openapi.json
authorization_urls: []
description: ''
docs: https://developer-v4.enphase.com/developer-plans
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Enphase Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Enphase Energy uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Enphase Energy
provider_slug: enphase
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: enphase-scopes
source_filename: enphase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://developer-v4.enphase.com/docs/quickstart.html\ndocs: https://developer-v4.enphase.com/developer-plans\nnotes: >-\n  Enphase runs OAuth 2.0 but does not publish a scope reference page, and no published spec\n  declares an oauth2 securityScheme, so derive-oauth-scopes.py finds nothing. Two real\n  authorization surfaces exist and both are captured here. The OAuth token itself carries only\n  the coarse pair \"read write\" - visible in every token sample response in the quick start guide.\n  The fine-grained surface is the portal's Access Controls: an application is created against a\n  plan, the developer ticks the access-control groups that plan allows, and that tick list\n  becomes the application's effective scope, shown to the homeowner on the consent screen. Access\n  controls are selected at application-registration time, not requested per authorization\n  request, so they never appear as an OAuth scope parameter.\n\
  oauth_scopes:\n- scope: read\n  description: Read the system data the system owner has approved for this application.\n  flows:\n  - authorizationCode\n  - password\n  - clientCredentials\n  evidence: 'token sample response: \"scope\": \"read write\"'\n- scope: write\n  description: Write system configuration and control operations the system owner has approved.\n  flows:\n  - authorizationCode\n  - password\n  evidence: 'token sample response: \"scope\": \"read write\"'\naccess_controls:\n  model: plan-gated application permissions, selected at registration and shown on the consent screen\n  docs: https://developer-v4.enphase.com/developer-plans\n  groups:\n  - name: System Details\n    plans: [Watt, Kilowatt, Megawatt, Partner]\n    covers: System listing, search, summary, devices, events, alarms, event types\n  - name: Site Level Production Monitoring\n    plans: [Watt, Kilowatt, Megawatt, Partner]\n    covers: Production meter readings, energy lifetime, production meter telemetry,\
  \ RGM stats\n  - name: Site Level Consumption Monitoring\n    plans: [Watt, Kilowatt, Megawatt, Partner]\n    covers: Consumption meter readings and telemetry, consumption lifetime, import/export lifetime\n  - name: EV Charger Monitoring\n    plans: [Watt, Kilowatt, Megawatt, Partner]\n    covers: IQ EV charger devices, events, sessions, schedules, lifetime and telemetry\n  - name: Device Level Monitoring\n    plans: [Kilowatt, Megawatt, Partner]\n    covers: Per-microinverter and per-IQ-Battery telemetry, EVSE and heat-pump device telemetry\n  - name: Streaming API\n    plans: [Kilowatt, Megawatt, Partner]\n    covers: The live-status text/event-stream endpoint (getLiveData), billed at $0.10 per hit\n  - name: System Configurations\n    plans: [Megawatt, Partner]\n    covers: Battery settings, storm guard, grid status, load control read and write\n  - name: Commissioning API\n    plans: [Partner]\n    covers: Activations, companies, users, meters, grid profiles, tariff, estimate, PV catalog\n\
  \  - name: EV Charger Control\n    plans: [Partner]\n    covers: start_charging and stop_charging on an IQ EV charger\nvpp_authorization:\n  model: contract-scoped, no user-selectable scopes\n  notes: >-\n    The VPP API is sold to utilities, aggregators, DERMS providers and third-party owners\n    registered as Enphase Grid Services partners. Its client_credentials token carries no scope\n    field; entitlement is bound to the partner account and the VPP/program records it owns.\n  docs: https://developer-v4.enphase.com/vpp-plans\ngaps:\n- No published scope reference page and no scopes map in any spec.\n- Access controls cannot be stepped up per authorization request; changing them means creating a\n  new application and re-obtaining homeowner consent.\nrelated:\n- authentication/enphase-authentication.yml\n- plans/enphase-plans.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enphase/refs/heads/main/scopes/enphase-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- United States
- Solar
- DER
- Renewables
- Battery Storage
- EV Charging
- Demand Response
- Virtual Power Plant
- Grid Services
- Microinverters
- Home Energy Management
- Smart Metering
- Telemetry
token_urls: []
---
