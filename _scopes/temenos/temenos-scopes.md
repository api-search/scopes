---
authorization_urls:
- https://journey.temenos.com/oauth2/authorize
- https://auth.temenos.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Temenos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Temenos publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Temenos API on a user''s behalf.


  Tokens are issued from https://journey.temenos.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Temenos
provider_slug: temenos
schemes:
- flows:
  - authorizationUrl: https://journey.temenos.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://journey.temenos.com/oauth2/token
  name: oauth2
  source: openapi/temenos-journey-manager-openapi.yml
- description: OAuth 2.0 authentication for API access
  flows:
  - authorizationUrl: https://auth.temenos.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.temenos.com/oauth2/token
  name: oauth2
  source: openapi/temenos-transact-openapi.yml
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Administrative access
  flows:
  - authorizationCode
  scope: admin
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: temenos-scopes
source_filename: temenos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/temenos-journey-manager-openapi.yml, openapi/temenos-transact-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/temenos-journey-manager-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://journey.temenos.com/oauth2/authorize\n    tokenUrl: https://journey.temenos.com/oauth2/token\n- name: oauth2\n  source: openapi/temenos-transact-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.temenos.com/oauth2/authorize\n    tokenUrl: https://auth.temenos.com/oauth2/token\n  description: OAuth 2.0 authentication for API access\nscopes:\n- scope: admin\n  description: Administrative access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temenos-transact-openapi.yml\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temenos-journey-manager-openapi.yml\n  - openapi/temenos-transact-openapi.yml\n- scope:\
  \ write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/temenos-journey-manager-openapi.yml\n  - openapi/temenos-transact-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/scopes/temenos-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
token_urls:
- https://journey.temenos.com/oauth2/token
- https://auth.temenos.com/oauth2/token
---
