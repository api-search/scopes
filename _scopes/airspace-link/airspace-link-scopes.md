---
authorization_urls: []
description: ''
docs: https://developers.airspacelink.com/doc-2002712
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Airspace Link Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Airspace Link publishes 15 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Airspace Link API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Airspace Link
provider_slug: airspace-link
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  tokenUrl: https://airhub-api-sandbox.airspacelink.com/v1/oauth/token
scope_count: 15
scope_names:
- advisory:read
- aviation:read
- hazard:read
- briefing:area:read
- briefing:location:read
- operation:read
- operation:create
- operation:update
- operation:delete
- laanc:read
- laanc:create
- laanc:update
- laanc:delete
- surface:create
- route:create
scopes:
- description: Read airspace advisories.
  flows:
  - clientCredentials
  scope: advisory:read
- description: Read aviation airspace data.
  flows:
  - clientCredentials
  scope: aviation:read
- description: Read operational hazard data (documented as "hazar:read" in the auth overview).
  flows:
  - clientCredentials
  scope: hazard:read
- description: Read B4UFLY airspace briefings for an area geometry.
  flows:
  - clientCredentials
  scope: briefing:area:read
- description: Read B4UFLY airspace briefings for a point location.
  flows:
  - clientCredentials
  scope: briefing:location:read
- description: Read ASL and ephemeral operations.
  flows:
  - clientCredentials
  scope: operation:read
- description: Create ASL and ephemeral operations.
  flows:
  - clientCredentials
  scope: operation:create
- description: Update ASL operations.
  flows:
  - clientCredentials
  scope: operation:update
- description: Delete ASL and ephemeral operations.
  flows:
  - clientCredentials
  scope: operation:delete
- description: Read LAANC SDSP operations and authorizations.
  flows:
  - clientCredentials
  scope: laanc:read
- description: Create LAANC operations and submit LAANC authorizations.
  flows:
  - clientCredentials
  scope: laanc:create
- description: Update, cancel, close, and acknowledge LAANC operations and authorizations.
  flows:
  - clientCredentials
  scope: laanc:update
- description: Delete LAANC operations.
  flows:
  - clientCredentials
  scope: laanc:delete
- description: Request surface-layer access, classify risk, and generate surface hexbins.
  flows:
  - clientCredentials
  scope: surface:create
- description: Generate risk-aware drone routes.
  flows:
  - clientCredentials
  scope: route:create
slug: airspace-link-scopes
source_filename: airspace-link-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.airspacelink.com/doc-2002712\ndocs: https://developers.airspacelink.com/doc-2002712\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  tokenUrl: https://airhub-api-sandbox.airspacelink.com/v1/oauth/token\nscopes:\n- scope: advisory:read\n  description: Read airspace advisories.\n  flows: [clientCredentials]\n- scope: aviation:read\n  description: Read aviation airspace data.\n  flows: [clientCredentials]\n- scope: hazard:read\n  description: Read operational hazard data (documented as \"hazar:read\" in the auth overview).\n  flows: [clientCredentials]\n- scope: briefing:area:read\n  description: Read B4UFLY airspace briefings for an area geometry.\n  flows: [clientCredentials]\n- scope: briefing:location:read\n  description: Read B4UFLY airspace briefings for a point location.\n  flows: [clientCredentials]\n- scope: operation:read\n  description: Read ASL and ephemeral operations.\n\
  \  flows: [clientCredentials]\n- scope: operation:create\n  description: Create ASL and ephemeral operations.\n  flows: [clientCredentials]\n- scope: operation:update\n  description: Update ASL operations.\n  flows: [clientCredentials]\n- scope: operation:delete\n  description: Delete ASL and ephemeral operations.\n  flows: [clientCredentials]\n- scope: laanc:read\n  description: Read LAANC SDSP operations and authorizations.\n  flows: [clientCredentials]\n- scope: laanc:create\n  description: Create LAANC operations and submit LAANC authorizations.\n  flows: [clientCredentials]\n- scope: laanc:update\n  description: Update, cancel, close, and acknowledge LAANC operations and authorizations.\n  flows: [clientCredentials]\n- scope: laanc:delete\n  description: Delete LAANC operations.\n  flows: [clientCredentials]\n- scope: surface:create\n  description: Request surface-layer access, classify risk, and generate surface hexbins.\n  flows: [clientCredentials]\n- scope: route:create\n  description:\
  \ Generate risk-aware drone routes.\n  flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airspace-link/refs/heads/main/scopes/airspace-link-scopes.yml
summary_line: 15 scopes
tags:
- Company
- Drones
- UAS
- Airspace
- Aviation
- LAANC
- UTM
- Geospatial
- Public Safety
- Logistics
token_urls: []
---
