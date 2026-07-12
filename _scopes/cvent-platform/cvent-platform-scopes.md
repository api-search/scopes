---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cvent Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cvent Platform publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cvent Platform API on a user''s behalf.


  Tokens are issued from https://api-platform.cvent.com/ea/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cvent Platform
provider_slug: cvent-platform
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/cvent-platform-openapi.yml
scope_count: 9
scope_names:
- event/attendees:read
- event/attendees:write
- event/contacts:read
- event/contacts:write
- event/custom-fields:read
- event/events:read
- event/events:write
- event/registration-types:read
- event/sessions:read
scopes:
- description: Read attendees
  flows:
  - clientCredentials
  scope: event/attendees:read
- description: Write attendees
  flows:
  - clientCredentials
  scope: event/attendees:write
- description: Read contacts
  flows:
  - clientCredentials
  scope: event/contacts:read
- description: Write contacts
  flows:
  - clientCredentials
  scope: event/contacts:write
- description: Read custom fields
  flows:
  - clientCredentials
  scope: event/custom-fields:read
- description: Read events
  flows:
  - clientCredentials
  scope: event/events:read
- description: Write events
  flows:
  - clientCredentials
  scope: event/events:write
- description: Read registration types
  flows:
  - clientCredentials
  scope: event/registration-types:read
- description: Read sessions
  flows:
  - clientCredentials
  scope: event/sessions:read
slug: cvent-platform-scopes
source_filename: cvent-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-platform-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/cvent-platform-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\nscopes:\n- scope: event/attendees:read\n  description: Read attendees\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/attendees:write\n  description: Write attendees\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/contacts:read\n  description: Read contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/contacts:write\n  description: Write contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/custom-fields:read\n  description: Read custom fields\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/cvent-platform-openapi.yml\n- scope: event/events:read\n  description: Read events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/events:write\n  description: Write events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/registration-types:read\n  description: Read registration types\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- scope: event/sessions:read\n  description: Read sessions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cvent-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-platform/refs/heads/main/scopes/cvent-platform-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Attendee Hub
- Conferences
- Event Management
- Event Marketing
- Events
- Hospitality
- Hospitality Cloud
- Hybrid Events
- Meetings
- OAuth 2.0
- Passkey
- Registration
- REST API
- Supplier Network
- Surveys
- Venue Management
- Virtual Events
token_urls:
- https://api-platform.cvent.com/ea/oauth2/token
---
