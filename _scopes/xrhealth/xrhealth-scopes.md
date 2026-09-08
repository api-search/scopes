---
api_specs:
- filename: xrhealth-platform-openapi.yml
  format: yaml
  label: XRHealth Platform API
  slug: xrhealth-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xrhealth/refs/heads/main/openapi/xrhealth-platform-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Xrhealth Scopes
name_suffix: OAuth Scopes
note: 'These two scope names are read from the provider''s own published EXAMPLE value ("patient:login patient:read") and are the only scope strings XRHealth publishes anywhere. They are recorded with confidence medium and complete: false: an example is evidence that the patient:<verb> namespace is real, not evidence that these are the only two scopes, and no scope descriptions are published. A scopes/permissions reference page would live behind the invitation-only developer portal at https://developer.xr.health/, where every documentation path probed on 2026-09-04 returned 404 to an unauthenticated client. Nothing here is invented.'
overview: 'XRHealth publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the XRHealth API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: XRHealth
provider_slug: xrhealth
schemes: []
scope_count: 2
scope_names:
- patient:login
- patient:read
scopes:
- description: ''
  flows: []
  scope: patient:login
- description: ''
  flows: []
  scope: patient:read
slug: xrhealth-scopes
source_filename: xrhealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/xrhealth-platform-openapi.yml\ndocs: null\ncomplete: false\nschemes: []\nschemes_note: >-\n  No oauth2 securityScheme is declared in the document, so 0-working/derive-oauth-scopes.py finds\n  nothing and writes nothing. This file records the scope evidence the contract carries anyway,\n  because the API is OAuth-shaped in every respect except its securityScheme declaration:\n  /auth/public/token accepts grant_type authorization_code and refresh_token, PKCE S256 is required,\n  and both TokenResponse and MeResponse carry scopes.\nscope_carriers:\n- schema: TokenResponse\n  field: scope\n  form: space-delimited string\n  required: true\n- schema: MeResponse\n  field: scopes\n  form: array of string\n  required: true\nscopes:\n- scope: 'patient:login'\n  description: null\n  source: 'openapi/xrhealth-platform-openapi.yml -> components.schemas.TokenResponse.properties.scope.example'\n  confidence: medium\n- scope: 'patient:read'\n\
  \  description: null\n  source: 'openapi/xrhealth-platform-openapi.yml -> components.schemas.TokenResponse.properties.scope.example'\n  confidence: medium\nnote: >-\n  These two scope names are read from the provider's own published EXAMPLE value\n  (\"patient:login patient:read\") and are the only scope strings XRHealth publishes anywhere. They\n  are recorded with confidence medium and complete: false: an example is evidence that the\n  patient:<verb> namespace is real, not evidence that these are the only two scopes, and no scope\n  descriptions are published. A scopes/permissions reference page would live behind the\n  invitation-only developer portal at https://developer.xr.health/, where every documentation path\n  probed on 2026-09-04 returned 404 to an unauthenticated client. Nothing here is invented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xrhealth/refs/heads/main/scopes/xrhealth-scopes.yml
summary_line: 2 scopes
tags:
- Health
- Digital Health
- Telehealth
- Virtual Reality
- Extended Reality
- Medical Devices
- Rehabilitation
- Mental Health
- Patient Authentication
- Healthcare
token_urls: []
---
