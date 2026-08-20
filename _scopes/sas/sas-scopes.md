---
api_specs:
- filename: sas-businessrules-api-openapi.yml
  format: yaml
  label: SAS Institute BusinessRules API
  slug: sas-businessrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-businessrules-api-openapi.yml
- filename: sas-cas-api-openapi.yml
  format: yaml
  label: SAS Institute CAS API
  slug: sas-cas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-cas-api-openapi.yml
- filename: sas-decisions-api-openapi.yml
  format: yaml
  label: SAS Institute Decisions API
  slug: sas-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-decisions-api-openapi.yml
- filename: sas-files-api-openapi.yml
  format: yaml
  label: SAS Institute Files API
  slug: sas-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-files-api-openapi.yml
- filename: sas-folders-api-openapi.yml
  format: yaml
  label: SAS Institute Folders API
  slug: sas-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-folders-api-openapi.yml
- filename: sas-identities-api-openapi.yml
  format: yaml
  label: SAS Institute Identities API
  slug: sas-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-identities-api-openapi.yml
- filename: sas-jobs-api-openapi.yml
  format: yaml
  label: SAS Institute Jobs API
  slug: sas-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-jobs-api-openapi.yml
- filename: sas-logon-api-openapi.yml
  format: yaml
  label: SAS Institute Logon API
  slug: sas-logon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-logon-api-openapi.yml
- filename: sas-models-api-openapi.yml
  format: yaml
  label: SAS Institute Models API
  slug: sas-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-models-api-openapi.yml
- filename: sas-reports-api-openapi.yml
  format: yaml
  label: SAS Institute Reports API
  slug: sas-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/openapi/sas-reports-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Sas Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAS Institute publishes 1 OAuth 2.0 scope via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAS Institute API on a user''s behalf.


  Tokens are issued from /SASLogon/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAS Institute
provider_slug: sas
schemes:
- flows:
  - flow: password
    tokenUrl: /SASLogon/oauth/token
  name: oauth2
  source: openapi/sas-viya-rest-api-openapi.yml
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect scope
  flows:
  - password
  scope: openid
slug: sas-scopes
source_filename: sas-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sas-viya-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sas-viya-rest-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /SASLogon/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect scope\n  flows:\n  - password\n  sources:\n  - openapi/sas-viya-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sas/refs/heads/main/scopes/sas-scopes.yml
summary_line: 1 scope · password
tags:
- Analytics
- Data Management
- Artificial Intelligence
- Machine-Learning
- Software
token_urls:
- /SASLogon/oauth/token
---
