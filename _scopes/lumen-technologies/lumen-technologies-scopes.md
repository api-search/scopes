---
api_specs:
- filename: lumen-internet-on-demand-api-openapi.yml
  format: yaml
  label: Lumen Internet On-Demand API
  slug: internet-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/openapi/lumen-internet-on-demand-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lumen Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lumen Technologies publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lumen Technologies API on a user''s behalf.


  Tokens are issued from https://api.lumen.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lumen Technologies
provider_slug: lumen-technologies
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.lumen.com/oauth2/token
  name: oauth2
  source: openapi/lumen-internet-on-demand-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to connections
  flows:
  - clientCredentials
  scope: read
- description: Write access to connections
  flows:
  - clientCredentials
  scope: write
slug: lumen-technologies-scopes
source_filename: lumen-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lumen-internet-on-demand-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/lumen-internet-on-demand-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.lumen.com/oauth2/token\nscopes:\n- scope: read\n  description: Read access to connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lumen-internet-on-demand-api-openapi.yml\n- scope: write\n  description: Write access to connections\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lumen-internet-on-demand-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumen-technologies/refs/heads/main/scopes/lumen-technologies-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Bandwidth
- Edge Cloud
- Fiber
- Infrastructure
- Internet
- Network
- Networking
- Security
- Telecom
token_urls:
- https://api.lumen.com/oauth2/token
---
