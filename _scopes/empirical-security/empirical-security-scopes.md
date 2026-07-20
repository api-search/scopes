---
api_specs:
- filename: empirical-security-openapi.yml
  format: yaml
  label: Empirical Security API
  slug: empirical-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/openapi/empirical-security-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.empiricalsecurity.com/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Empirical Security Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Empirical Security publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Empirical Security API on a user''s behalf.


  Tokens are issued from https://empiricalsecurity.fusionauth.io/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Empirical Security
provider_slug: empirical-security
schemes:
- description: OAuth 2.0 client credentials flow via FusionAuth. Exchange client ID/secret (HTTP Basic) for a one-hour JWT access token, then send it as a Bearer token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://empiricalsecurity.fusionauth.io/oauth2/token
  name: oauth2
  source: openapi/empirical-security-openapi.yml
scope_count: 1
scope_names:
- target-entity:0c6d5dcc-8bf0-4cd1-bd65-066ef0422369
scopes:
- description: Access to the Empirical Security tenant/entity's CVE data.
  flows:
  - clientCredentials
  scope: target-entity:0c6d5dcc-8bf0-4cd1-bd65-066ef0422369
slug: empirical-security-scopes
source_filename: empirical-security-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/empirical-security-openapi.yml\ndocs: https://docs.empiricalsecurity.com/authentication\nschemes:\n- name: oauth2\n  source: openapi/empirical-security-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://empiricalsecurity.fusionauth.io/oauth2/token\n  description: OAuth 2.0 client credentials flow via FusionAuth. Exchange client ID/secret (HTTP\n    Basic) for a one-hour JWT access token, then send it as a Bearer token.\nscopes:\n- scope: target-entity:0c6d5dcc-8bf0-4cd1-bd65-066ef0422369\n  description: Access to the Empirical Security tenant/entity's CVE data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/empirical-security-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empirical-security/refs/heads/main/scopes/empirical-security-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Security
- Cybersecurity
- Vulnerability Management
- Vulnerability Prioritization
- CVE
- EPSS
- Exploit Prediction
- Threat Intelligence
token_urls:
- https://empiricalsecurity.fusionauth.io/oauth2/token
---
