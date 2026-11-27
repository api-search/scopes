---
authorization_urls:
- https://japanstartupresources.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Japan Startup Resources Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Japan Startup Resources publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Japan Startup Resources API on a user''s behalf.


  Tokens are issued from https://japanstartupresources.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Japan Startup Resources
provider_slug: japanstartupresources-com
schemes:
- flows:
  - authorizationUrl: https://japanstartupresources.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://japanstartupresources.com/oauth/token
  name: subscriberOAuth
  source: openapi/japanstartupresources-com-openapi.json
scope_count: 1
scope_names:
- mcp:v0
scopes:
- description: Read curated weekly events and news
  flows:
  - authorizationCode
  scope: mcp:v0
slug: japanstartupresources-com-scopes
source_filename: japanstartupresources-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/japanstartupresources-com-openapi.json\nschemes:\n- name: subscriberOAuth\n  source: openapi/japanstartupresources-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://japanstartupresources.com/oauth/authorize\n    tokenUrl: https://japanstartupresources.com/oauth/token\nscopes:\n- scope: mcp:v0\n  description: Read curated weekly events and news\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/japanstartupresources-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/japanstartupresources-com/scopes/japanstartupresources-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Startups
- Japan
- Entrepreneurship
- Directory
- Newsletters
token_bound: false
token_urls:
- https://japanstartupresources.com/oauth/token
---
