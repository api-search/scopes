---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cvent Hospitality Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cvent Hospitality Cloud publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cvent Hospitality Cloud API on a user''s behalf.


  Tokens are issued from https://api-platform.cvent.com/reglink/v1/authentication/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cvent Hospitality Cloud
provider_slug: cvent-hospitality-cloud
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/reglink/v1/authentication/token
  name: OAuth2ClientCredentials
  source: openapi/cvent-hospitality-cloud-openapi.yml
scope_count: 2
scope_names:
- passkey:read
- passkey:write
scopes:
- description: Read Passkey events, hotels, room types, reservations
  flows:
  - clientCredentials
  scope: passkey:read
- description: Create and modify reservation requests
  flows:
  - clientCredentials
  scope: passkey:write
slug: cvent-hospitality-cloud-scopes
source_filename: cvent-hospitality-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-hospitality-cloud-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/cvent-hospitality-cloud-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/reglink/v1/authentication/token\nscopes:\n- scope: passkey:read\n  description: Read Passkey events, hotels, room types, reservations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-openapi.yml\n- scope: passkey:write\n  description: Create and modify reservation requests\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-hospitality-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-hospitality-cloud/refs/heads/main/scopes/cvent-hospitality-cloud-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Catering
- Group Bookings
- Hospitality
- Hospitality Cloud
- Hotels
- Housing
- OAuth 2.0
- Passkey
- Reservations
- RFP
- Room Blocks
- Sales
- Sourcing
- Supplier Network
- Venues
token_urls:
- https://api-platform.cvent.com/reglink/v1/authentication/token
---
