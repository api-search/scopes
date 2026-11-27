---
api_specs:
- filename: multilocale-com-phrases-api-openapi.yml
  format: yaml
  label: MultiLocale Phrases API
  slug: multilocale-com-phrases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-phrases-api-openapi.yml
- filename: multilocale-com-projects-api-openapi.yml
  format: yaml
  label: MultiLocale Projects API
  slug: multilocale-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-projects-api-openapi.yml
- filename: multilocale-com-sandbox-api-openapi.yml
  format: yaml
  label: MultiLocale Sandbox API
  slug: multilocale-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/multilocale-com/openapi/multilocale-com-sandbox-api-openapi.yml
authorization_urls:
- https://app.multilocale.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: MultiLocale Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MultiLocale publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MultiLocale API on a user''s behalf.


  Tokens are issued from https://api.authrice.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MultiLocale
provider_slug: multilocale-com
schemes:
- description: Authrice authorization-code flow with PKCE for delegated access.
  flows:
  - authorizationUrl: https://app.multilocale.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.authrice.com/api/oauth/token
  name: oauth2
  source: openapi/multilocale-com-openapi.json
scope_count: 5
scope_names:
- phrases:read
- phrases:write
- projects:read
- projects:write
- translations:write
scopes:
- description: Read phrases and translations.
  flows:
  - authorizationCode
  scope: phrases:read
- description: Create, update, and delete phrases.
  flows:
  - authorizationCode
  scope: phrases:write
- description: Read projects and their locales.
  flows:
  - authorizationCode
  scope: projects:read
- description: Create, rename, and delete projects.
  flows:
  - authorizationCode
  scope: projects:write
- description: Machine-translate phrases using organization credits.
  flows:
  - authorizationCode
  scope: translations:write
slug: multilocale-com-scopes
source_filename: multilocale-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/multilocale-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/multilocale-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.multilocale.com/oauth/authorize\n    tokenUrl: https://api.authrice.com/api/oauth/token\n  description: Authrice authorization-code flow with PKCE for delegated access.\nscopes:\n- scope: phrases:read\n  description: Read phrases and translations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/multilocale-com-openapi.json\n- scope: phrases:write\n  description: Create, update, and delete phrases.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/multilocale-com-openapi.json\n- scope: projects:read\n  description: Read projects and their locales.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/multilocale-com-openapi.json\n- scope: projects:write\n  description: Create, rename, and delete projects.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/multilocale-com-openapi.json\n- scope: translations:write\n  description: Machine-translate phrases using organization credits.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/multilocale-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/multilocale-com/scopes/multilocale-com-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Localization
- Translation
- Developer Tools
- Software-as-a-Service
token_bound: false
token_urls:
- https://api.authrice.com/api/oauth/token
---
