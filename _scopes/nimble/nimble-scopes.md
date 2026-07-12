---
authorization_urls:
- https://app.nimble.com/oauth/authorize
description: ''
docs: https://www.nimble.com/developers/docs/#tag/Authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nimble Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nimble publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nimble API on a user''s behalf.


  Tokens are issued from https://app.nimble.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nimble
provider_slug: nimble
schemes:
- description: 'OAuth 2.0 bearer token. Provide the token via either the

    `Authorization: Bearer <token>` header or the

    `access_token=<token>` query parameter.'
  flows:
  - authorizationUrl: https://app.nimble.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.nimble.com/oauth/token
  name: bearerAuth
  source: openapi/nimble-openapi.yml
scope_count: 3
scope_names:
- basic
- contacts
- deals
scopes:
- description: Access to user and company info.
  flows: []
  scope: basic
- description: Access to contacts.
  flows: []
  scope: contacts
- description: Access to deals.
  flows: []
  scope: deals
slug: nimble-scopes
source_filename: nimble-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/nimble-openapi.yml\ndocs: https://www.nimble.com/developers/docs/#tag/Authentication\nschemes:\n- name: bearerAuth\n  source: openapi/nimble-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.nimble.com/oauth/authorize\n    tokenUrl: https://app.nimble.com/oauth/token\n  description: |-\n    OAuth 2.0 bearer token. Provide the token via either the\n    `Authorization: Bearer <token>` header or the\n    `access_token=<token>` query parameter.\nscopes:\n- scope: basic\n  description: Access to user and company info.\n  sources:\n  - https://www.nimble.com/developers/docs/#tag/Authentication\n- scope: contacts\n  description: Access to contacts.\n  sources:\n  - https://www.nimble.com/developers/docs/#tag/Authentication\n- scope: deals\n  description: Access to deals.\n  sources:\n  - https://www.nimble.com/developers/docs/#tag/Authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/scopes/nimble-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- CRM
- Sales
- Contact Management
- Relationship Management
- Marketing Automation
- Pipeline Management
token_urls:
- https://app.nimble.com/oauth/token
---
