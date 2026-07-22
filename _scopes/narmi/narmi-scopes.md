---
api_specs:
- filename: narmi-public-openapi-original.yml
  format: yaml
  label: Narmi Public API
  slug: narmi-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/narmi/refs/heads/main/openapi/narmi-public-openapi-original.yml
authorization_urls:
- /v2/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Narmi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Narmi publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Narmi API on a user''s behalf.


  Tokens are issued from /v2/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Narmi
provider_slug: narmi
schemes:
- flows:
  - authorizationUrl: /v2/oauth/authorize/
    flow: authorizationCode
    tokenUrl: /v2/oauth/token/
  name: oauth2
  source: openapi/narmi-public-openapi-original.yml
scope_count: 11
scope_names:
- banking:accounts:read
- banking:accounts:write
- banking:documents:read
- banking:products:read
- banking:scheduled_transfers:read
- banking:scheduled_transfers:write
- banking:transactions:read
- banking:transactions:write
- banking:users:read
- read
- write
scopes:
- description: Can read account information.
  flows:
  - authorizationCode
  scope: banking:accounts:read
- description: Can update account information.
  flows:
  - authorizationCode
  scope: banking:accounts:write
- description: Can read user statements and documents.
  flows:
  - authorizationCode
  scope: banking:documents:read
- description: Can read product information.
  flows:
  - authorizationCode
  scope: banking:products:read
- description: Can read scheduled transfer information.
  flows:
  - authorizationCode
  scope: banking:scheduled_transfers:read
- description: Can create and update scheduled transfers.
  flows:
  - authorizationCode
  scope: banking:scheduled_transfers:write
- description: Can read transaction information.
  flows:
  - authorizationCode
  scope: banking:transactions:read
- description: Can update transaction information.
  flows:
  - authorizationCode
  scope: banking:transactions:write
- description: Can read user profile information.
  flows:
  - authorizationCode
  scope: banking:users:read
- description: ''
  flows: []
  scope: read
- description: ''
  flows: []
  scope: write
slug: narmi-scopes
source_filename: narmi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/narmi-public-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/narmi-public-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v2/oauth/authorize/\n    tokenUrl: /v2/oauth/token/\nscopes:\n- scope: banking:accounts:read\n  description: Can read account information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:accounts:write\n  description: Can update account information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:documents:read\n  description: Can read user statements and documents.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:products:read\n  description: Can read product information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n\
  - scope: banking:scheduled_transfers:read\n  description: Can read scheduled transfer information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:scheduled_transfers:write\n  description: Can create and update scheduled transfers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:transactions:read\n  description: Can read transaction information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:transactions:write\n  description: Can update transaction information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: banking:users:read\n  description: Can read user profile information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope: read\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n- scope:\
  \ write\n  sources:\n  - openapi/narmi-public-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/narmi/refs/heads/main/scopes/narmi-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Company
- Fintech
- Digital Banking
- Banking
- Payments
- ACH
- Wires
- FedNow
- Cards
- Financial Services
token_urls:
- /v2/oauth/token/
---
