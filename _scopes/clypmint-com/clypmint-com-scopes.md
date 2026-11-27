---
api_specs:
- filename: clypmint-com-assets-api-openapi.yml
  format: yaml
  label: Clypmint Assets API
  slug: clypmint-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-assets-api-openapi.yml
- filename: clypmint-com-content-plans-api-openapi.yml
  format: yaml
  label: Clypmint Content Plans API
  slug: clypmint-com-content-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-content-plans-api-openapi.yml
- filename: clypmint-com-me-api-openapi.yml
  format: yaml
  label: Clypmint Me API
  slug: clypmint-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-me-api-openapi.yml
- filename: clypmint-com-memory-api-openapi.yml
  format: yaml
  label: Clypmint Memory API
  slug: clypmint-com-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-memory-api-openapi.yml
- filename: clypmint-com-openapi-json-api-openapi.yml
  format: yaml
  label: Clypmint Openapi.json API
  slug: clypmint-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-openapi-json-api-openapi.yml
- filename: clypmint-com-schedule-api-openapi.yml
  format: yaml
  label: Clypmint Schedule API
  slug: clypmint-com-schedule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-schedule-api-openapi.yml
- filename: clypmint-com-styles-api-openapi.yml
  format: yaml
  label: Clypmint Styles API
  slug: clypmint-com-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-styles-api-openapi.yml
- filename: clypmint-com-videos-api-openapi.yml
  format: yaml
  label: Clypmint Videos API
  slug: clypmint-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clypmint-com/openapi/clypmint-com-videos-api-openapi.yml
authorization_urls: []
description: ''
docs: https://clypmint.com/developers
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clypmint Scopes
name_suffix: OAuth Scopes
note: scopes_supported read from the OAuth protected-resource metadata (HTTP 200, GET). The OpenAPI declares only http bearer; its 403 response names the publish scope.
overview: 'Clypmint publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clypmint API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clypmint
provider_slug: clypmint-com
schemes: []
scope_count: 2
scope_names:
- clypmint
- clypmint.publish
scopes:
- description: Base scope listed in scopes_supported for the MCP resource; no further description is published.
  flows: []
  scope: clypmint
- description: Publishing permission. The OpenAPI 403 reads "This needs publishing permission (scope clypmint.publish)"; scheduling with schedule_plan approve true requires it.
  flows: []
  scope: clypmint.publish
slug: clypmint-com-scopes
source_filename: clypmint-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clypmint.com/.well-known/oauth-protected-resource\ndocs: https://clypmint.com/developers\nnote: scopes_supported read from the OAuth protected-resource metadata (HTTP 200, GET). The OpenAPI declares only http bearer; its 403 response names the publish scope.\nscopes:\n- name: clypmint\n  description: Base scope listed in scopes_supported for the MCP resource; no further description is published.\n- name: clypmint.publish\n  description: Publishing permission. The OpenAPI 403 reads \"This needs publishing permission (scope clypmint.publish)\"; scheduling with schedule_plan approve true requires it.\n"
source_yaml_url: https://artifacts.apis.io/clypmint-com/scopes/clypmint-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- AI Video Editing
- Video
- Generative AI
- Content Creation
- MCP
- Creator Tools
- Short-Form Video
token_bound: false
token_urls: []
---
