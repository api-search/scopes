---
authorization_urls: []
description: ''
docs: https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: 75F Scopes
name_suffix: OAuth Scopes
note: 75F publishes no public OpenAPI, so this was read from the provider's own documentation rather than derived by 0-working/derive-oauth-scopes.py (which requires openapi/ files). The only named OAuth scopes 75F documents are on the v2 Special Schedules API; the Project Haystack surface is authorized by Facilisight site membership (Secondary Manager role) rather than by scope strings.
overview: '75F publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 75F API on a user''s behalf.


  Tokens are issued from https://api.75f.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 75F
provider_slug: 75f
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.75f.io/oauth/token
  name: OAuth2ClientCredentials
  source: https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API
scope_count: 2
scope_names:
- schedules:read
- schedules:write
scopes:
- description: Read special (exception-based) schedules for authorized zones and buildings.
  flows:
  - clientCredentials
  scope: schedules:read
- description: Create, update and delete special schedules for authorized zones and buildings.
  flows:
  - clientCredentials
  scope: schedules:write
slug: 75f-scopes
source_filename: 75f-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://support.75f.io/hc/en-us/articles/45325600917651-Special-Schedules-Via-API\ndocs: https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API\nnote: >-\n  75F publishes no public OpenAPI, so this was read from the provider's own documentation rather than\n  derived by 0-working/derive-oauth-scopes.py (which requires openapi/ files). The only named OAuth\n  scopes 75F documents are on the v2 Special Schedules API; the Project Haystack surface is authorized\n  by Facilisight site membership (Secondary Manager role) rather than by scope strings.\nschemes:\n- name: OAuth2ClientCredentials\n  source: https://support.75f.io/hc/en-us/articles/5459701361427-Oauth-API\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.75f.io/oauth/token\nscopes:\n- scope: schedules:read\n  description: Read special (exception-based) schedules for authorized zones and buildings.\n  flows: [clientCredentials]\n  apis: [75F Special\
  \ Schedules API]\n  sources: [https://support.75f.io/hc/en-us/articles/45325600917651-Special-Schedules-Via-API]\n- scope: schedules:write\n  description: Create, update and delete special schedules for authorized zones and buildings.\n  flows: [clientCredentials]\n  apis: [75F Special Schedules API]\n  sources: [https://support.75f.io/hc/en-us/articles/45325600917651-Special-Schedules-Via-API]\nunscoped_surfaces:\n- api: 75F Haystack API\n  authorization: >-\n    No documented scope strings. Read/write separation is expressed as separate Azure APIM products\n    (Read API, Write API, Special Schedule API), each with its own subscription key, combined with the\n    caller's Facilisight site permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/75f/refs/heads/main/scopes/75f-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Building Automation
- Smart Buildings
- HVAC
- Internet of Things
- Energy Management
- Project Haystack
- Facilities Management
- Sensors
- Building Management System
token_urls:
- https://api.75f.io/oauth/token
---
