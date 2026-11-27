---
api_specs:
- filename: clousd-com-account-api-openapi.yml
  format: yaml
  label: Clousd Account API
  slug: clousd-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-account-api-openapi.yml
- filename: clousd-com-adb-api-openapi.yml
  format: yaml
  label: Clousd ADB API
  slug: clousd-com-adb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-adb-api-openapi.yml
- filename: clousd-com-ai-agents-api-openapi.yml
  format: yaml
  label: Clousd AI agents API
  slug: clousd-com-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-ai-agents-api-openapi.yml
- filename: clousd-com-apps-api-openapi.yml
  format: yaml
  label: Clousd Apps API
  slug: clousd-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-apps-api-openapi.yml
- filename: clousd-com-devices-api-openapi.yml
  format: yaml
  label: Clousd Devices API
  slug: clousd-com-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-devices-api-openapi.yml
- filename: clousd-com-files-and-media-api-openapi.yml
  format: yaml
  label: Clousd Files and media API
  slug: clousd-com-files-and-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-files-and-media-api-openapi.yml
- filename: clousd-com-network-api-openapi.yml
  format: yaml
  label: Clousd Network API
  slug: clousd-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-network-api-openapi.yml
- filename: clousd-com-screen-and-input-api-openapi.yml
  format: yaml
  label: Clousd Screen and input API
  slug: clousd-com-screen-and-input-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-screen-and-input-api-openapi.yml
- filename: clousd-com-tasks-api-openapi.yml
  format: yaml
  label: Clousd Tasks API
  slug: clousd-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-tasks-api-openapi.yml
- filename: clousd-com-webhooks-api-openapi.yml
  format: yaml
  label: Clousd Webhooks API
  slug: clousd-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://clousd.com/docs/api-keys/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clousd Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares only http bearer; scopes are documented for API keys, and the MCP OAuth consent offers the matching choice ("See and control" or "Only see").
overview: 'Clousd publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clousd API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clousd
provider_slug: clousd-com
schemes: []
scope_count: 2
scope_names:
- read
- control
scopes:
- description: List devices, take screenshots, observe the screen, read jobs. Any call that changes something answers 403.
  flows: []
  scope: read
- description: Everything above, plus start, stop, install apps, act on the screen and run tasks.
  flows: []
  scope: control
slug: clousd-com-scopes
source_filename: clousd-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clousd.com/docs/api-keys/, https://clousd.com/docs/mcp/\ndocs: https://clousd.com/docs/api-keys/\nnote: The OpenAPI declares only http bearer; scopes are documented for API keys, and the MCP OAuth consent offers the matching\n  choice (\"See and control\" or \"Only see\").\nscopes:\n- name: read\n  description: List devices, take screenshots, observe the screen, read jobs. Any call that changes something answers 403.\n  oauth_consent_label: Only see\n- name: control\n  description: Everything above, plus start, stop, install apps, act on the screen and run tasks.\n  oauth_consent_label: See and control\n"
source_yaml_url: https://artifacts.apis.io/clousd-com/scopes/clousd-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Android
- Cloud Phones
- AI Agents
- MCP
- Mobile Testing
- QA
- Emulators
token_bound: false
token_urls: []
---
