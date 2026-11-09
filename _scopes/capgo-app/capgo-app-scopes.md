---
api_specs:
- filename: capgo-app-api-keys-api-openapi.yml
  format: yaml
  label: Capgo API Keys API
  slug: capgo-app-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-api-keys-api-openapi.yml
- filename: capgo-app-apps-api-openapi.yml
  format: yaml
  label: Capgo Apps API
  slug: capgo-app-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-apps-api-openapi.yml
- filename: capgo-app-bundles-api-openapi.yml
  format: yaml
  label: Capgo Bundles API
  slug: capgo-app-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-bundles-api-openapi.yml
- filename: capgo-app-channels-api-openapi.yml
  format: yaml
  label: Capgo Channels API
  slug: capgo-app-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-channels-api-openapi.yml
- filename: capgo-app-devices-api-openapi.yml
  format: yaml
  label: Capgo Devices API
  slug: capgo-app-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-devices-api-openapi.yml
- filename: capgo-app-members-api-openapi.yml
  format: yaml
  label: Capgo Members API
  slug: capgo-app-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-members-api-openapi.yml
- filename: capgo-app-organizations-api-openapi.yml
  format: yaml
  label: Capgo Organizations API
  slug: capgo-app-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-organizations-api-openapi.yml
- filename: capgo-app-statistics-api-openapi.yml
  format: yaml
  label: Capgo Statistics API
  slug: capgo-app-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capgo-app/openapi/capgo-app-statistics-api-openapi.yml
authorization_urls:
- https://api.capgo.app/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Capgo App Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Capgo publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Capgo API on a user''s behalf.


  Tokens are issued from https://api.capgo.app/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Capgo
provider_slug: capgo-app
schemes:
- description: 'OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration (https://api.capgo.app/mcp/oauth/register). Issuer: https://capgo.app. The access token is a Capgo API key limited to the organizations the user selects on the consent screen; send it as a Bearer token.'
  flows:
  - authorizationUrl: https://api.capgo.app/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.capgo.app/mcp/oauth/token
  name: CapgoOAuth
  source: openapi/capgo-app-openapi.json
scope_count: 1
scope_names:
- capgo
scopes:
- description: Act on the organizations the user selects on the consent screen, with the user's role in each of them.
  flows:
  - authorizationCode
  scope: capgo
slug: capgo-app-scopes
source_filename: capgo-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/capgo-app-openapi.json\nschemes:\n- name: CapgoOAuth\n  source: openapi/capgo-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.capgo.app/mcp/oauth/authorize\n    tokenUrl: https://api.capgo.app/mcp/oauth/token\n  description: 'OAuth 2.0 authorization code flow with PKCE (S256) and dynamic client registration\n    (https://api.capgo.app/mcp/oauth/register). Issuer: https://capgo.app. The access token\n    is a Capgo API key limited to the organizations the user selects on the consent screen;\n    send it as a Bearer token.'\nscopes:\n- scope: capgo\n  description: Act on the organizations the user selects on the consent screen, with the user's\n    role in each of them.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/capgo-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/capgo-app/scopes/capgo-app-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Mobile
- Development
- Capacitor
token_bound: false
token_urls:
- https://api.capgo.app/mcp/oauth/token
---
