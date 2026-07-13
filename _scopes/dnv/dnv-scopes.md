---
api_specs:
- filename: dnv-class-status-openapi.yml
  format: yaml
  label: DNV Class Status API
  slug: dnv-class-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/openapi/dnv-class-status-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Dnv Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DNV publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DNV API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DNV
provider_slug: dnv
schemes:
- description: OAuth 2.0 via Azure AD B2C. Tokens obtained from https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token using client credentials grant with resource ID c916a223-f3d4-4d43-b709-cfcd77ff4a05.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token
  name: oauth2
  source: openapi/dnv-class-status-openapi.yml
scope_count: 1
scope_names:
- class_status:read
scopes:
- description: Read vessel classification status
  flows:
  - clientCredentials
  scope: class_status:read
slug: dnv-scopes
source_filename: dnv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dnv-class-status-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/dnv-class-status-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token\n  description: OAuth 2.0 via Azure AD B2C. Tokens obtained from https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token\n    using client credentials grant with resource ID c916a223-f3d4-4d43-b709-cfcd77ff4a05.\nscopes:\n- scope: class_status:read\n  description: Read vessel classification status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dnv-class-status-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnv/refs/heads/main/scopes/dnv-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Maritime
- Energy
- Classification
- Vessel
- Data Platform
token_urls:
- https://login.microsoftonline.com/dnvglb2cprod.onmicrosoft.com/oauth2/token
---
