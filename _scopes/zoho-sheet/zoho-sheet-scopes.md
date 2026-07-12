---
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Sheet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Sheet publishes 2 OAuth 2.0 scopes via the authorizationCode, implicit, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Sheet API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Sheet
provider_slug: zoho-sheet
schemes:
- description: Zoho OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://accounts.zoho.com/oauth/v3/device/token
  name: oauthToken
  source: openapi/openapi.yml
scope_count: 2
scope_names:
- ZohoSheet.dataAPI.READ
- ZohoSheet.dataAPI.UPDATE
scopes:
- description: Read spreadsheet data
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: ZohoSheet.dataAPI.READ
- description: Write and update spreadsheet data
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  scope: ZohoSheet.dataAPI.UPDATE
slug: zoho-sheet-scopes
source_filename: zoho-sheet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: oauthToken\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n  - flow: implicit\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n  - flow: clientCredentials\n    tokenUrl: https://accounts.zoho.com/oauth/v3/device/token\n  description: Zoho OAuth 2.0 authentication\nscopes:\n- scope: ZohoSheet.dataAPI.READ\n  description: Read spreadsheet data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/openapi.yml\n- scope: ZohoSheet.dataAPI.UPDATE\n  description: Write and update spreadsheet data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-sheet/refs/heads/main/scopes/zoho-sheet-scopes.yml
summary_line: 2 scopes · authorizationCode/implicit/clientCredentials
tags:
- Spreadsheets
- Productivity
- Collaboration
- Data
- Office
- Zoho
token_urls:
- https://accounts.zoho.com/oauth/v2/token
- https://accounts.zoho.com/oauth/v3/device/token
---
