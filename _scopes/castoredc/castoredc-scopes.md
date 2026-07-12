---
authorization_urls: []
description: ''
docs: https://data.castoredc.com/api
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Castoredc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Castor publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Castor API on a user''s behalf.


  Tokens are issued from https://data.castoredc.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Castor
provider_slug: castoredc
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://data.castoredc.com/api/oauth/token
  name: oauth2ClientCredentials
  source: openapi/castoredc-openapi.yml
scope_count: 3
scope_names:
- default
- study_statistics
- record
scopes:
- description: Grants access to everything (allows access to all endpoints).
  flows: []
  scope: default
- description: Grants access to a study's statistics.
  flows: []
  scope: study_statistics
- description: Grants access to the data for a single participant; intended for use by study subjects.
  flows: []
  scope: record
slug: castoredc-scopes
source_filename: castoredc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/castoredc-openapi.yml\ndocs: https://data.castoredc.com/api\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/castoredc-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://data.castoredc.com/api/oauth/token\nscopes:\n- scope: default\n  description: Grants access to everything (allows access to all endpoints).\n  sources:\n  - https://data.castoredc.com/api\n  - https://data.castoredc.com/api/swagger?format=json\n- scope: study_statistics\n  description: Grants access to a study's statistics.\n  sources:\n  - https://data.castoredc.com/api\n  - https://data.castoredc.com/api/swagger?format=json\n- scope: record\n  description: Grants access to the data for a single participant; intended for use\n    by study subjects.\n  sources:\n  - https://data.castoredc.com/api\n  - https://data.castoredc.com/api/swagger?format=json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/scopes/castoredc-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- Healthcare
- Life Sciences
- Research
token_urls:
- https://data.castoredc.com/api/oauth/token
---
