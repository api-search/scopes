---
authorization_urls:
- https://patient.samedi.de/oauth/authorize
description: ''
docs: https://wiki.samedi.de/display/doc/Booking+API
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Samedi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'samedi publishes 10 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the samedi API on a user''s behalf.


  Tokens are issued from https://patient.samedi.de/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: samedi
provider_slug: samedi
schemes:
- flows:
  - authorizationUrl: https://patient.samedi.de/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://patient.samedi.de/oauth/token
  - flow: clientCredentials
    tokenUrl: https://patient.samedi.de/oauth/token
  name: OAuth2
  source: https://patient.samedi.de/.well-known/openid-configuration
scope_count: 10
scope_names:
- openid
- basic
- profile:read
- profile_read
- appointments:read
- appointments:book
- appointment_read
- appointment_write
- appointment_guest_lookup
- appointment_guest_write
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Basic access to the authorized user context.
  flows: []
  scope: basic
- description: Read the patient/user profile.
  flows: []
  scope: profile:read
- description: Read the patient/user profile (underscore variant).
  flows: []
  scope: profile_read
- description: Read the user's appointments.
  flows: []
  scope: appointments:read
- description: Book appointments on behalf of the user.
  flows: []
  scope: appointments:book
- description: Read appointments (underscore variant).
  flows: []
  scope: appointment_read
- description: Create or modify appointments (underscore variant).
  flows: []
  scope: appointment_write
- description: Look up appointments for a guest (non-registered) booking.
  flows: []
  scope: appointment_guest_lookup
- description: Create or modify appointments for a guest (non-registered) booking.
  flows: []
  scope: appointment_guest_write
slug: samedi-scopes
source_filename: samedi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://patient.samedi.de/.well-known/openid-configuration\ndocs: https://wiki.samedi.de/display/doc/Booking+API\nschemes:\n- name: OAuth2\n  source: https://patient.samedi.de/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient.samedi.de/oauth/authorize\n    tokenUrl: https://patient.samedi.de/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://patient.samedi.de/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: basic\n  description: Basic access to the authorized user context.\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: profile:read\n  description: Read the patient/user profile.\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: profile_read\n  description: Read the patient/user profile\
  \ (underscore variant).\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: appointments:read\n  description: Read the user's appointments.\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: appointments:book\n  description: Book appointments on behalf of the user.\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: appointment_read\n  description: Read appointments (underscore variant).\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: appointment_write\n  description: Create or modify appointments (underscore variant).\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: appointment_guest_lookup\n  description: Look up appointments for a guest (non-registered) booking.\n  sources: ['well-known/samedi-openid-configuration.json']\n- scope: appointment_guest_write\n  description: Create or modify appointments for a guest (non-registered) booking.\n  sources: ['well-known/samedi-openid-configuration.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samedi/refs/heads/main/scopes/samedi-scopes.yml
summary_line: 10 scopes · authorizationCode/clientCredentials
tags:
- Company
- Healthcare
- Scheduling
- Appointments
- Booking
- Patient Engagement
- OAuth
- FHIR
- Telemedicine
- Germany
token_urls:
- https://patient.samedi.de/oauth/token
---
