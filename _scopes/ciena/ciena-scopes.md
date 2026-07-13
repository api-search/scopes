---
api_specs:
- filename: ciena-blue-planet-openapi.yml
  format: yaml
  label: Ciena Blue Planet Open API
  slug: blue-planet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/openapi/ciena-blue-planet-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ciena Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ciena publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ciena API on a user''s behalf.


  Tokens are issued from https://api.blueplanet.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ciena
provider_slug: ciena
schemes:
- description: OAuth 2.0 authentication for Blue Planet API
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.blueplanet.com/oauth/token
  name: oauth2
  source: openapi/ciena-blue-planet-openapi.yml
scope_count: 5
scope_names:
- alarms:read
- performance:read
- services:read
- services:write
- topology:read
scopes:
- description: Read network alarms
  flows:
  - clientCredentials
  scope: alarms:read
- description: Read performance metrics
  flows:
  - clientCredentials
  scope: performance:read
- description: Read network services
  flows:
  - clientCredentials
  scope: services:read
- description: Create and modify network services
  flows:
  - clientCredentials
  scope: services:write
- description: Read network topology
  flows:
  - clientCredentials
  scope: topology:read
slug: ciena-scopes
source_filename: ciena-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ciena-blue-planet-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/ciena-blue-planet-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.blueplanet.com/oauth/token\n  description: OAuth 2.0 authentication for Blue Planet API\nscopes:\n- scope: alarms:read\n  description: Read network alarms\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ciena-blue-planet-openapi.yml\n- scope: performance:read\n  description: Read performance metrics\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ciena-blue-planet-openapi.yml\n- scope: services:read\n  description: Read network services\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ciena-blue-planet-openapi.yml\n- scope: services:write\n  description: Create and modify network services\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ciena-blue-planet-openapi.yml\n- scope: topology:read\n  description: Read network\
  \ topology\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ciena-blue-planet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/scopes/ciena-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- MEF
- NETCONF
- Network Automation
- Network Management
- Optical
- RESTCONF
- SDN
- Telecom
- TM Forum
- Fortune 1000
token_urls:
- https://api.blueplanet.com/oauth/token
---
