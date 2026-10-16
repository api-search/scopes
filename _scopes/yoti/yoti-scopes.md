---
api_specs:
- filename: yoti-openapi-generated.yml
  format: yaml
  label: Yoti API
  slug: yoti-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/_ae-authored/yoti-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Yoti Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Yoti publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Yoti API on a user''s behalf.


  Tokens are issued from https://auth.api.yoti.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yoti
provider_slug: yoti
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.api.yoti.com/v1/oauth/token
  name: OAuth2_Client_Credentials
  source: openapi/yoti-openapi-generated.yml
scope_count: 2
scope_names:
- did:match
- poa:verify
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: did:match
- description: ''
  flows:
  - clientCredentials
  scope: poa:verify
slug: yoti-scopes
source_filename: yoti-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/yoti-openapi-generated.yml\nschemes:\n- name: OAuth2_Client_Credentials\n  source: openapi/yoti-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.api.yoti.com/v1/oauth/token\nscopes:\n- scope: did:match\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/yoti-openapi-generated.yml\n- scope: poa:verify\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/yoti-openapi-generated.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/scopes/yoti-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Identity
- Verification
- DigitalID
- SDK
token_bound: false
token_urls:
- https://auth.api.yoti.com/v1/oauth/token
---
