---
authorization_urls:
- https://api.cib.bnpparibas.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Connexis Cash Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Connexis Cash publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Connexis Cash API on a user''s behalf.


  Tokens are issued from https://api.cib.bnpparibas.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Connexis Cash
provider_slug: connexis-cash
schemes:
- flows:
  - authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  - flow: clientCredentials
    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token
  name: oauth2
  source: openapi/connexis-cash-openapi.yml
scope_count: 1
scope_names:
- aisp
scopes:
- description: Account Information Service
  flows:
  - authorizationCode
  - clientCredentials
  scope: aisp
slug: connexis-cash-scopes
source_filename: connexis-cash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/connexis-cash-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/connexis-cash-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cib.bnpparibas.com/oauth2/v1/authorize\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://api.cib.bnpparibas.com/oauth2/v1/token\nscopes:\n- scope: aisp\n  description: Account Information Service\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/connexis-cash-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connexis-cash/refs/heads/main/scopes/connexis-cash-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Account Information
- BNP Paribas
- Cash Management
- Corporate Banking
- Digital Banking
- Liquidity Management
- Open Banking
- Payments
- PSD2
- SCA
- STET
token_urls:
- https://api.cib.bnpparibas.com/oauth2/v1/token
---
