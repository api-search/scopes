---
api_specs:
- filename: v4.json
  format: json
  label: Kit API
  slug: kit-api
  spec_type: OpenAPI
  url: https://developers.kit.com/api-reference/v4.json
authorization_urls:
- https://api.kit.com/v4/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Convertkit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kit publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kit API on a user''s behalf.


  Tokens are issued from https://api.kit.com/v4/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kit
provider_slug: convertkit
schemes:
- description: Authenticate API requests via an OAuth token
  flows:
  - authorizationUrl: https://api.kit.com/v4/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kit.com/v4/oauth/token
  name: OAuth2
  source: openapi/openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Kit API v4
  flows:
  - authorizationCode
  scope: read
- description: Write access to Kit API v4
  flows:
  - authorizationCode
  scope: write
slug: convertkit-scopes
source_filename: convertkit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kit.com/v4/oauth/authorize\n    tokenUrl: https://api.kit.com/v4/oauth/token\n  description: Authenticate API requests via an OAuth token\nscopes:\n- scope: read\n  description: Read access to Kit API v4\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: write\n  description: Write access to Kit API v4\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/scopes/convertkit-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
token_urls:
- https://api.kit.com/v4/oauth/token
---
