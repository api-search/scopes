---
api_specs:
- filename: ptc-thingworx-websocket-asyncapi.yml
  format: yaml
  label: PTC ThingWorx WebSocket/AlwaysOn API
  slug: thingworx-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/asyncapi/ptc-thingworx-websocket-asyncapi.yml
- filename: ptc-thingworx-datashapes-api-openapi.yml
  format: yaml
  label: ptc-thingworx DataShapes API
  slug: ptc-thingworx-datashapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-datashapes-api-openapi.yml
- filename: ptc-thingworx-events-api-openapi.yml
  format: yaml
  label: ptc-thingworx Events API
  slug: ptc-thingworx-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-events-api-openapi.yml
- filename: ptc-thingworx-properties-api-openapi.yml
  format: yaml
  label: ptc-thingworx Properties API
  slug: ptc-thingworx-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-properties-api-openapi.yml
- filename: ptc-thingworx-things-api-openapi.yml
  format: yaml
  label: ptc-thingworx Things API
  slug: ptc-thingworx-things-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-things-api-openapi.yml
- filename: ptc-thingworx-thingtemplates-api-openapi.yml
  format: yaml
  label: ptc-thingworx ThingTemplates API
  slug: ptc-thingworx-thingtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-thingtemplates-api-openapi.yml
- filename: ptc-thingworx-valuestreams-api-openapi.yml
  format: yaml
  label: ptc-thingworx ValueStreams API
  slug: ptc-thingworx-valuestreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/openapi/ptc-thingworx-valuestreams-api-openapi.yml
authorization_urls:
- https://thingworx.example.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ptc Thingworx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PTC ThingWorx publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PTC ThingWorx API on a user''s behalf.


  Tokens are issued from https://thingworx.example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PTC ThingWorx
provider_slug: ptc-thingworx
schemes:
- flows:
  - authorizationUrl: https://thingworx.example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://thingworx.example.com/oauth/token
  name: oauth2
  source: openapi/ptc-thingworx-rest-openapi.yml
scope_count: 1
scope_names:
- THINGWORX
scopes:
- description: Access ThingWorx REST API
  flows:
  - authorizationCode
  scope: THINGWORX
slug: ptc-thingworx-scopes
source_filename: ptc-thingworx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ptc-thingworx-rest-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/ptc-thingworx-rest-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thingworx.example.com/oauth/authorize\n    tokenUrl: https://thingworx.example.com/oauth/token\nscopes:\n- scope: THINGWORX\n  description: Access ThingWorx REST API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ptc-thingworx-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ptc-thingworx/refs/heads/main/scopes/ptc-thingworx-scopes.yml
summary_line: 1 scope · authorizationCode
tags: []
token_urls:
- https://thingworx.example.com/oauth/token
---
