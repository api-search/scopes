---
authorization_urls:
- https://community.spiceworks.com/oauth/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Spiceworks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spiceworks publishes 3 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spiceworks API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spiceworks
provider_slug: spiceworks
schemes:
- description: OAuth 2.0 authentication via the Spiceworks Cloud Apps platform. Applications receive an implicit grant token through the JS SDK postMessage bridge when running inside the Spiceworks UI.
  flows:
  - authorizationUrl: https://community.spiceworks.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/spiceworks-cloud-apps-openapi.yml
scope_count: 3
scope_names:
- helpdesk
- inventory
- users
scopes:
- description: Access Help Desk tickets and comments
  flows:
  - implicit
  scope: helpdesk
- description: Access device inventory data
  flows:
  - implicit
  scope: inventory
- description: Access user profile data
  flows:
  - implicit
  scope: users
slug: spiceworks-scopes
source_filename: spiceworks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spiceworks-cloud-apps-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/spiceworks-cloud-apps-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://community.spiceworks.com/oauth/authorize\n  description: OAuth 2.0 authentication via the Spiceworks Cloud Apps platform. Applications\n    receive an implicit grant token through the JS SDK postMessage bridge when running inside\n    the Spiceworks UI.\nscopes:\n- scope: helpdesk\n  description: Access Help Desk tickets and comments\n  flows:\n  - implicit\n  sources:\n  - openapi/spiceworks-cloud-apps-openapi.yml\n- scope: inventory\n  description: Access device inventory data\n  flows:\n  - implicit\n  sources:\n  - openapi/spiceworks-cloud-apps-openapi.yml\n- scope: users\n  description: Access user profile data\n  flows:\n  - implicit\n  sources:\n  - openapi/spiceworks-cloud-apps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiceworks/refs/heads/main/scopes/spiceworks-scopes.yml
summary_line: 3 scopes · implicit
tags:
- Community
- Enterprise IT
- IT Management
token_urls: []
---
