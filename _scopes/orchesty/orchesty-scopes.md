---
api_specs:
- filename: orchesty-2.0-openapi-generated.yml
  format: yaml
  label: Orchesty.io 2.0 API
  slug: 2.0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orchesty/refs/heads/main/openapi/_ae-authored/orchesty-2.0-openapi-generated.yml
- filename: orchesty-3.0-openapi-generated.yml
  format: yaml
  label: Orchesty.io 3.0 API
  slug: 3.0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orchesty/refs/heads/main/openapi/_ae-authored/orchesty-3.0-openapi-generated.yml
authorization_urls:
- https://auth.wflow.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Orchesty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Orchesty.io publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Orchesty.io API on a user''s behalf.


  Tokens are issued from https://auth.wflow.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Orchesty.io
provider_slug: orchesty
schemes:
- flows:
  - authorizationUrl: https://auth.wflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.wflow.com/oauth/token
  name: OAuth2
  source: openapi/orchesty-2.0-openapi-generated.yml
- flows:
  - authorizationUrl: https://auth.wflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.wflow.com/oauth/token
  name: OAuth2
  source: openapi/orchesty-3.0-openapi-generated.yml
- flows:
  - authorizationUrl: https://auth.wflow.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.wflow.com/oauth/token
  name: OAuth2
  source: openapi/orchesty-openapi-generated.yml
scope_count: 2
scope_names:
- read_invoices
- write_invoices
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: read_invoices
- description: ''
  flows:
  - authorizationCode
  scope: write_invoices
slug: orchesty-scopes
source_filename: orchesty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/orchesty-2.0-openapi-generated.yml, openapi/orchesty-3.0-openapi-generated.yml,\n  openapi/orchesty-openapi-generated.yml\nschemes:\n- name: OAuth2\n  source: openapi/orchesty-2.0-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wflow.com/oauth/authorize\n    tokenUrl: https://auth.wflow.com/oauth/token\n- name: OAuth2\n  source: openapi/orchesty-3.0-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wflow.com/oauth/authorize\n    tokenUrl: https://auth.wflow.com/oauth/token\n- name: OAuth2\n  source: openapi/orchesty-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wflow.com/oauth/authorize\n    tokenUrl: https://auth.wflow.com/oauth/token\nscopes:\n- scope: read_invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orchesty-2.0-openapi-generated.yml\n  - openapi/orchesty-3.0-openapi-generated.yml\n\
  \  - openapi/orchesty-openapi-generated.yml\n- scope: write_invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orchesty-2.0-openapi-generated.yml\n  - openapi/orchesty-3.0-openapi-generated.yml\n  - openapi/orchesty-openapi-generated.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orchesty/refs/heads/main/scopes/orchesty-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Integration
- Platform
- Automation
- Artificial Intelligence
- Open Source
token_bound: false
token_urls:
- https://auth.wflow.com/oauth/token
---
