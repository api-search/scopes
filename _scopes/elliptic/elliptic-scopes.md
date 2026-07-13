---
api_specs:
- filename: aml-api-oauth.json
  format: json
  label: Elliptic AML API
  slug: elliptic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/aml-api-oauth.json
- filename: ia-api.json
  format: json
  label: Elliptic AI API
  slug: elliptic-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/ia-api.json
- filename: sanctions-api.json
  format: json
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/sanctions-api.json
- filename: data-fabric.yaml
  format: yaml
  label: Elliptic Data Fabric API
  slug: elliptic-data-fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/data-fabric.yaml
authorization_urls:
- https://login.elliptic.co/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Elliptic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elliptic publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elliptic API on a user''s behalf.


  Tokens are issued from https://login.elliptic.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elliptic
provider_slug: elliptic
schemes:
- flows:
  - authorizationUrl: https://login.elliptic.co/authorize
    flow: authorizationCode
    tokenUrl: https://login.elliptic.co/oauth/token
  name: oauth2
  source: openapi/aml-api-oauth.json
scope_count: 2
scope_names:
- openid
- profile
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: profile
slug: elliptic-scopes
source_filename: elliptic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aml-api-oauth.json\nschemes:\n- name: oauth2\n  source: openapi/aml-api-oauth.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.elliptic.co/authorize\n    tokenUrl: https://login.elliptic.co/oauth/token\nscopes:\n- scope: openid\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aml-api-oauth.json\n- scope: profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aml-api-oauth.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/scopes/elliptic-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Blockchain
- Crypto
- Compliance
- AML
- Transaction Screening
- Wallet Screening
- Risk Scoring
- Analytics
token_urls:
- https://login.elliptic.co/oauth/token
---
