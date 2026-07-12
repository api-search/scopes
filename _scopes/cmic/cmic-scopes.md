---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cmic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CMiC publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CMiC API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CMiC
provider_slug: cmic
schemes:
- description: OAuth 2.0 client credentials for CMiC API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/cmic-construction-erp-openapi.yml
scope_count: 1
scope_names:
- api://cmic/.default
scopes:
- description: Full CMiC API access
  flows:
  - clientCredentials
  scope: api://cmic/.default
slug: cmic-scopes
source_filename: cmic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cmic-construction-erp-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cmic-construction-erp-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: OAuth 2.0 client credentials for CMiC API access\nscopes:\n- scope: api://cmic/.default\n  description: Full CMiC API access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cmic-construction-erp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cmic/refs/heads/main/scopes/cmic-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Construction
- ERP
- Finance
- Project Management
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
