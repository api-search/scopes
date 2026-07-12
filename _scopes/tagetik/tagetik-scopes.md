---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tagetik Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CCH Tagetik publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CCH Tagetik API on a user''s behalf.


  Tokens are issued from https://{environment}/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CCH Tagetik
provider_slug: tagetik
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{environment}/oauth2/token
  name: OAuth2ClientCredentials
  source: openapi/cch-tagetik-odata-openapi.yml
scope_count: 1
scope_names:
- read
scopes:
- description: Read access to financial and analytical data
  flows:
  - clientCredentials
  scope: read
slug: tagetik-scopes
source_filename: tagetik-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cch-tagetik-odata-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/cch-tagetik-odata-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}/oauth2/token\nscopes:\n- scope: read\n  description: Read access to financial and analytical data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cch-tagetik-odata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tagetik/refs/heads/main/scopes/tagetik-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Analytics
- Budgeting
- Corporate Performance Management
- ESG
- Financial Close
- Financial Consolidation
- Financial Planning
- OData
- Reporting
token_urls:
- https://{environment}/oauth2/token
---
