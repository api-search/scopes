---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Majesco Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'majesco publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the majesco API on a user''s behalf.


  Tokens are issued from https://auth.majesco.example.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: majesco
provider_slug: majesco
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.majesco.example.com/oauth2/token
  name: OAuth2
  source: openapi/majesco-policy-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to policies, claims, and billing
  flows:
  - clientCredentials
  scope: read
- description: Write access for policy and claim operations
  flows:
  - clientCredentials
  scope: write
slug: majesco-scopes
source_filename: majesco-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/majesco-policy-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/majesco-policy-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.majesco.example.com/oauth2/token\nscopes:\n- scope: read\n  description: Read access to policies, claims, and billing\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/majesco-policy-openapi.yml\n- scope: write\n  description: Write access for policy and claim operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/majesco-policy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/majesco/refs/heads/main/scopes/majesco-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- https://auth.majesco.example.com/oauth2/token
---
