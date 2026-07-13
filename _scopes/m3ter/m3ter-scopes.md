---
api_specs:
- filename: m3ter-openapi.yml
  format: yaml
  label: M3ter API
  slug: m3ter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/m3ter/refs/heads/main/openapi/m3ter-openapi.yml
authorization_urls:
- https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: M3Ter Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'M3ter publishes 6 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the M3ter API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: M3ter
provider_slug: m3ter
schemes:
- description: 'm3ter supports machine to machine authentication using the `clientCredentials` OAuth2 flow.


    The `authorizationCode` flow controls access for human users via the m3ter Console application.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  - authorizationUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/token
  name: OAuth2
  source: openapi/m3ter-openapi.yml
scope_count: 6
scope_names:
- email
- m3ter-resources/m3ter-scope
- measurements:fileUpload
- measurements:retrieve
- measurements:upload
- openid
scopes:
- description: email
  flows:
  - authorizationCode
  scope: email
- description: m3ter resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: m3ter-resources/m3ter-scope
- description: Upload file
  flows:
  - authorizationCode
  - clientCredentials
  scope: measurements:fileUpload
- description: Retrieve measurements
  flows:
  - authorizationCode
  - clientCredentials
  scope: measurements:retrieve
- description: Upload measurements
  flows:
  - authorizationCode
  - clientCredentials
  scope: measurements:upload
- description: OpenID
  flows:
  - authorizationCode
  scope: openid
slug: m3ter-scopes
source_filename: m3ter-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/m3ter-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/m3ter-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/token\n  description: |-\n    m3ter supports machine to machine authentication using the `clientCredentials` OAuth2 flow.\n\n    The `authorizationCode` flow controls access for human users via the m3ter Console application.\nscopes:\n- scope: email\n  description: email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/m3ter-openapi.yml\n- scope: m3ter-resources/m3ter-scope\n  description: m3ter resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/m3ter-openapi.yml\n- scope: measurements:fileUpload\n  description: Upload file\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/m3ter-openapi.yml\n- scope: measurements:retrieve\n  description: Retrieve measurements\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/m3ter-openapi.yml\n- scope: measurements:upload\n  description: Upload measurements\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/m3ter-openapi.yml\n- scope: openid\n  description: OpenID\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/m3ter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m3ter/refs/heads/main/scopes/m3ter-scopes.yml
summary_line: 6 scopes · clientCredentials/authorizationCode
tags:
- FinOps
- Usage-Based Billing
- Metering
- Billing
- Pricing
- SaaS
token_urls:
- /oauth/token
- https://m3ter.auth.us-east-1.amazoncognito.com/oauth2/token
---
