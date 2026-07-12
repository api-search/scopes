---
authorization_urls:
- https://accounts.infusionsoft.com/app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Keap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Keap publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Keap API on a user''s behalf.


  Tokens are issued from https://api.infusionsoft.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Keap
provider_slug: keap
schemes:
- description: Keap uses OAuth 2.0 for authentication. See https://developer.infusionsoft.com/getting-started-oauth-keys/
  flows:
  - authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.infusionsoft.com/token
  name: oauth2
  source: openapi/keap-openapi.yml
scope_count: 1
scope_names:
- full
scopes:
- description: Full access to the Keap CRM REST API.
  flows:
  - authorizationCode
  scope: full
slug: keap-scopes
source_filename: keap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keap-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/keap-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize\n    tokenUrl: https://api.infusionsoft.com/token\n  description: Keap uses OAuth 2.0 for authentication. See https://developer.infusionsoft.com/getting-started-oauth-keys/\nscopes:\n- scope: full\n  description: Full access to the Keap CRM REST API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/keap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/scopes/keap-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- CRM
- Sales
- Marketing Automation
- Small Business
- E-Commerce
- Contacts
token_urls:
- https://api.infusionsoft.com/token
---
