---
authorization_urls: []
description: ''
docs: ''
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Encompass Developer Connect Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Encompass Developer Connect publishes 2 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Encompass Developer Connect API on a user''s behalf.


  Tokens are issued from https://api.elliemae.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Encompass Developer Connect
provider_slug: encompass-developer-connect
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.elliemae.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.elliemae.com/oauth2/v1/token
  name: oauth2
  source: openapi/encompass-developer-connect-openapi.yml
scope_count: 2
scope_names:
- lor
- lp
scopes:
- description: Loan origination access
  flows:
  - clientCredentials
  - password
  scope: lor
- description: Loan pipeline access
  flows:
  - clientCredentials
  - password
  scope: lp
slug: encompass-developer-connect-scopes
source_filename: encompass-developer-connect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/encompass-developer-connect-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/encompass-developer-connect-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.elliemae.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.elliemae.com/oauth2/v1/token\nscopes:\n- scope: lor\n  description: Loan origination access\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/encompass-developer-connect-openapi.yml\n- scope: lp\n  description: Loan pipeline access\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/encompass-developer-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass-developer-connect/refs/heads/main/scopes/encompass-developer-connect-scopes.yml
summary_line: 2 scopes · password/clientCredentials
tags:
- Encompass
- ICE Mortgage Technology
- Loan Origination
- Lending
- Mortgage
- REST API
token_urls:
- https://api.elliemae.com/oauth2/v1/token
---
