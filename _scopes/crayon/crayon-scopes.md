---
authorization_urls: []
description: ''
docs: https://apidocs.crayon.com/scenarios/token-get.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Crayon Scopes
name_suffix: OAuth Scopes
note: Crayon's API (Cloud-iQ) documents a single OAuth2 scope, CustomerApi, used when requesting a token from the connect/token endpoint; no finer-grained scopes are published (https://apidocs.crayon.com/getting-started/authentication.html).
overview: 'Crayon publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Crayon API on a user''s behalf.


  Tokens are issued from https://api.crayon.com/api/v1/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Crayon
provider_slug: crayon
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.crayon.com/api/v1/connect/token
  name: OAuth2
  source: openapi/crayon-openapi.yml
scope_count: 1
scope_names:
- CustomerApi
scopes:
- description: Grants access to the Crayon customer API (Cloud-iQ); the single scope value passed when requesting an OAuth2 token.
  flows: []
  scope: CustomerApi
slug: crayon-scopes
source_filename: crayon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/crayon-openapi.yml\ndocs: https://apidocs.crayon.com/scenarios/token-get.html\nnote: >-\n  Crayon's API (Cloud-iQ) documents a single OAuth2 scope, CustomerApi, used\n  when requesting a token from the connect/token endpoint; no finer-grained\n  scopes are published (https://apidocs.crayon.com/getting-started/authentication.html).\nschemes:\n- name: OAuth2\n  source: openapi/crayon-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.crayon.com/api/v1/connect/token\nscopes:\n- scope: CustomerApi\n  description: >-\n    Grants access to the Crayon customer API (Cloud-iQ); the single scope\n    value passed when requesting an OAuth2 token.\n  sources:\n  - https://apidocs.crayon.com/scenarios/token-get.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crayon/refs/heads/main/scopes/crayon-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Competitive Intelligence
- Market Intelligence
- Sales Enablement
- Battlecards
- Win-Loss Analysis
- AI
- MCP
token_urls:
- https://api.crayon.com/api/v1/connect/token
---
