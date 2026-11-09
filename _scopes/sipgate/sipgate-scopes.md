---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Sipgate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'sipgate publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the sipgate API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: sipgate
provider_slug: sipgate
schemes: []
scope_count: 5
scope_names:
- all
- contacts:read
- devices:localprefix:read
- devices:sim:read
- devices:tariffannouncement:write
scopes:
- description: Full access
  flows: []
  scope: all
- description: Read contact information
  flows: []
  scope: contacts:read
- description: Read your device settings for localprefix
  flows: []
  scope: devices:localprefix:read
- description: Read your sim device settings
  flows: []
  scope: devices:sim:read
- description: Modify your device settings for tariff
  flows: []
  scope: devices:tariffannouncement:write
slug: sipgate-scopes
source_filename: sipgate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: searched\nsource: https://en.sipgate.io/rest-api/oauth2-scopes\nscopes:\n- name: all\n  description: Full access\n- name: contacts:read\n  description: Read contact information\n- name: devices:localprefix:read\n  description: Read your device settings for localprefix\n- name: devices:sim:read\n  description: Read your sim device settings\n- name: devices:tariffannouncement:write\n  description: Modify your device settings for tariff\n"
source_yaml_url: https://artifacts.apis.io/sipgate/scopes/sipgate-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Telephony
- Cloud
- Communications
token_bound: false
token_urls: []
---
