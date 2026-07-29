---
api_specs:
- filename: openadr-3-1-1-openapi.yaml
  format: yaml
  label: OpenADR 3 API
  slug: openadr-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openadr-alliance/refs/heads/main/openapi/openadr-3-1-1-openapi.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Openadr Alliance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OpenADR Alliance publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OpenADR Alliance API on a user''s behalf.


  Tokens are issued from auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OpenADR Alliance
provider_slug: openadr-alliance
schemes:
- description: Client credential flow.
  flows:
  - flow: clientCredentials
    tokenUrl: auth/token
  name: oAuth2ClientCredentials
  source: openapi/openadr-3-0-0-openapi.yaml
- description: Client credential flow.
  flows:
  - flow: clientCredentials
    tokenUrl: auth/token
  name: oAuth2ClientCredentials
  source: openapi/openadr-3-0-1-openapi.yaml
- description: Client credential flow.
  flows:
  - flow: clientCredentials
    tokenUrl: auth/token
  name: oAuth2ClientCredentials
  source: openapi/openadr-3-1-0-openapi.yaml
- description: Client credential flow.
  flows:
  - flow: clientCredentials
    tokenUrl: auth/token
  name: oAuth2ClientCredentials
  source: openapi/openadr-3-1-1-openapi.yaml
scope_count: 9
scope_names:
- read_all
- read_bl
- read_targets
- read_ven_objects
- write_events
- write_programs
- write_reports
- write_subscriptions
- write_vens
scopes:
- description: VENs and BL can read all resources
  flows:
  - clientCredentials
  scope: read_all
- description: BL can read BL-scoped notifier topic metadata
  flows:
  - clientCredentials
  scope: read_bl
- description: VENs may only read objects with targets by providing matching targets
  flows:
  - clientCredentials
  scope: read_targets
- description: VENs may only read objects whose clientID matches their own
  flows:
  - clientCredentials
  scope: read_ven_objects
- description: Only BL can write to events
  flows:
  - clientCredentials
  scope: write_events
- description: Only BL can write to programs
  flows:
  - clientCredentials
  scope: write_programs
- description: only VENs can write to reports
  flows:
  - clientCredentials
  scope: write_reports
- description: VENs and BL can write to subscriptions
  flows:
  - clientCredentials
  scope: write_subscriptions
- description: VENS and BL can write to vens and resources
  flows:
  - clientCredentials
  scope: write_vens
slug: openadr-alliance-scopes
source_filename: openadr-alliance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/openadr-3-0-0-openapi.yaml, openapi/openadr-3-0-1-openapi.yaml, openapi/openadr-3-1-0-openapi.yaml,\n  openapi/openadr-3-1-1-openapi.yaml\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/openadr-3-0-0-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: auth/token\n  description: Client credential flow.\n- name: oAuth2ClientCredentials\n  source: openapi/openadr-3-0-1-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: auth/token\n  description: Client credential flow.\n- name: oAuth2ClientCredentials\n  source: openapi/openadr-3-1-0-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: auth/token\n  description: Client credential flow.\n- name: oAuth2ClientCredentials\n  source: openapi/openadr-3-1-1-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: auth/token\n  description: Client credential flow.\nscopes:\n- scope: read_all\n  description: VENs\
  \ and BL can read all resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: read_bl\n  description: BL can read BL-scoped notifier topic metadata\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: read_targets\n  description: VENs may only read objects with targets by providing matching targets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: read_ven_objects\n  description: VENs may only read objects whose clientID matches their own\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: write_events\n  description: Only BL can write to events\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: write_programs\n  description: Only BL can write to programs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: write_reports\n  description: only VENs can write to reports\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n- scope: write_subscriptions\n  description: VENs and BL can write to subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n\
  - scope: write_vens\n  description: VENS and BL can write to vens and resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/openadr-3-0-0-openapi.yaml\n  - openapi/openadr-3-0-1-openapi.yaml\n  - openapi/openadr-3-1-0-openapi.yaml\n  - openapi/openadr-3-1-1-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openadr-alliance/refs/heads/main/scopes/openadr-alliance-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Energy
- United States
- Utilities
- Electricity
- Demand Response
- Grid
- DER
- OpenADR
- Standards
- Smart Grid
- EV Charging
- Certification
token_urls:
- auth/token
---
