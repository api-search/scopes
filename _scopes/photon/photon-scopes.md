---
api_specs:
- filename: photon-website-api-openapi.json
  format: json
  label: Photon Website API
  slug: photon-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-website-api-openapi.json
authorization_urls: []
description: ''
docs: https://docs.photon.health/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Photon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Photon publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Photon API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Photon
provider_slug: photon
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  token_url: https://auth.photon.health/oauth/token
scope_count: 6
scope_names:
- read:patient
- write:patient
- read:prescription
- write:prescription
- read:order
- write:order
scopes:
- description: Read access to patient records.
  flows:
  - clientCredentials
  scope: read:patient
- description: Create and update patient records (e.g. createPatient).
  flows:
  - clientCredentials
  scope: write:patient
- description: Read access to prescriptions.
  flows:
  - clientCredentials
  scope: read:prescription
- description: Create/modify prescriptions. Restricted - granted only to authorized providers via user access tokens; not available to M2M tokens.
  flows:
  - clientCredentials
  scope: write:prescription
- description: Read access to orders and fulfillment.
  flows:
  - clientCredentials
  scope: read:order
- description: Create and modify orders (routing, reroute, resend).
  flows:
  - clientCredentials
  scope: write:order
slug: photon-scopes
source_filename: photon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://docs.photon.health/docs/authentication\ndocs: https://docs.photon.health/docs/authentication\nprovider: Auth0\naudience:\n  production: https://api.photon.health\n  sandbox: https://api.neutron.health\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  token_url: https://auth.photon.health/oauth/token\nscopes:\n- scope: read:patient\n  description: Read access to patient records.\n  flows: [clientCredentials]\n- scope: write:patient\n  description: Create and update patient records (e.g. createPatient).\n  flows: [clientCredentials]\n- scope: read:prescription\n  description: Read access to prescriptions.\n  flows: [clientCredentials]\n- scope: write:prescription\n  description: Create/modify prescriptions. Restricted - granted only to authorized providers via user access tokens; not available to M2M tokens.\n  flows: [clientCredentials]\n  restricted: true\n- scope: read:order\n  description: Read\
  \ access to orders and fulfillment.\n  flows: [clientCredentials]\n- scope: write:order\n  description: Create and modify orders (routing, reroute, resend).\n  flows: [clientCredentials]\nnotes: >-\n  Scopes above are the Photon API application scopes documented on the auth page.\n  The Auth0 authorization server additionally advertises standard OIDC scopes\n  (openid, profile, offline_access, email) in its openid-configuration; those are\n  identity scopes, not API-resource scopes. write:prescription is the only\n  restricted resource scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/scopes/photon-scopes.yml
summary_line: 6 scopes
tags:
- Healthcare
- United States
- e-Prescribing
- Pharmacy
- Prescription Routing
- GraphQL
- Clinical API
- Digital Health
- Benefit Check
- Authentication
token_urls: []
---
