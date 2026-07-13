---
api_specs:
- filename: schlage-home-openapi.yml
  format: yaml
  label: Schlage Home API
  slug: schlage-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/openapi/schlage-home-openapi.yml
- filename: engage-credentialing-openapi.yml
  format: yaml
  label: ENGAGE Cloud Credentialing API
  slug: engage-credentialing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/openapi/engage-credentialing-openapi.yml
authorization_urls:
- https://account.schlage.com/OAuth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Allegion Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allegion publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allegion API on a user''s behalf.


  Tokens are issued from https://account.schlage.com/OAuth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allegion
provider_slug: allegion
schemes:
- flows:
  - authorizationUrl: https://account.schlage.com/OAuth2/authorize
    flow: authorizationCode
    tokenUrl: https://account.schlage.com/OAuth2/token
  name: OAuth2
  source: openapi/schlage-home-openapi.yml
scope_count: 5
scope_names:
- access_codes.read
- access_codes.write
- devices.read
- devices.write
- webhooks.manage
scopes:
- description: Read access codes stored on devices
  flows:
  - authorizationCode
  scope: access_codes.read
- description: Create, update, and delete access codes
  flows:
  - authorizationCode
  scope: access_codes.write
- description: Read device state, battery, connectivity, and firmware
  flows:
  - authorizationCode
  scope: devices.read
- description: Issue lock, unlock, and configuration commands
  flows:
  - authorizationCode
  scope: devices.write
- description: Create, list, and delete webhook subscriptions
  flows:
  - authorizationCode
  scope: webhooks.manage
slug: allegion-scopes
source_filename: allegion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/schlage-home-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/schlage-home-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.schlage.com/OAuth2/authorize\n    tokenUrl: https://account.schlage.com/OAuth2/token\nscopes:\n- scope: access_codes.read\n  description: Read access codes stored on devices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/schlage-home-openapi.yml\n- scope: access_codes.write\n  description: Create, update, and delete access codes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/schlage-home-openapi.yml\n- scope: devices.read\n  description: Read device state, battery, connectivity, and firmware\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/schlage-home-openapi.yml\n- scope: devices.write\n  description: Issue lock, unlock, and configuration commands\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/schlage-home-openapi.yml\n\
  - scope: webhooks.manage\n  description: Create, list, and delete webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/schlage-home-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allegion/refs/heads/main/scopes/allegion-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Access Control
- Smart Lock
- Smart Home
- Mobile Credentials
- Bluetooth
- BLE
- IoT
- Security
- Webhooks
- OAuth
- Schlage
- Von Duprin
- ENGAGE
token_urls:
- https://account.schlage.com/OAuth2/token
---
