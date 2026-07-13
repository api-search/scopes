---
api_specs:
- filename: verizon-thingspace-connectivity-openapi.yml
  format: yaml
  label: Verizon ThingSpace
  slug: thingspace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-thingspace-connectivity-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Verizon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Verizon publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Verizon API on a user''s behalf.


  Tokens are issued from https://thingspace.verizon.com/api/m2m/v2/session/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Verizon
provider_slug: verizon
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://thingspace.verizon.com/api/m2m/v2/session/token
  name: OAuth2ClientCredentials
  source: openapi/verizon-thingspace-connectivity-openapi.yml
scope_count: 3
scope_names:
- DISCOVERYREAD
- EVENTSREAD
- SERVICEPROFILEREAD
scopes:
- description: Read discovery information
  flows:
  - clientCredentials
  scope: DISCOVERYREAD
- description: Read device events
  flows:
  - clientCredentials
  scope: EVENTSREAD
- description: Read service profiles
  flows:
  - clientCredentials
  scope: SERVICEPROFILEREAD
slug: verizon-scopes
source_filename: verizon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/verizon-thingspace-connectivity-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/verizon-thingspace-connectivity-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://thingspace.verizon.com/api/m2m/v2/session/token\nscopes:\n- scope: DISCOVERYREAD\n  description: Read discovery information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/verizon-thingspace-connectivity-openapi.yml\n- scope: EVENTSREAD\n  description: Read device events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/verizon-thingspace-connectivity-openapi.yml\n- scope: SERVICEPROFILEREAD\n  description: Read service profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/verizon-thingspace-connectivity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/scopes/verizon-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Wireless
- Telecommunications
- IoT
- 5G
- Enterprise
- Network APIs
- Fortune 100
token_urls:
- https://thingspace.verizon.com/api/m2m/v2/session/token
---
