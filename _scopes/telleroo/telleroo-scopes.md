---
authorization_urls:
- https://admin.telleroo.com/oauth
description: ''
docs: https://partner-docs.telleroo.com/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Telleroo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Telleroo publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Telleroo API on a user''s behalf.


  Tokens are issued from https://api.telleroo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Telleroo
provider_slug: telleroo
schemes:
- api: Telleroo Partner API
  flows:
  - authorizationUrl: https://admin.telleroo.com/oauth
    flow: authorizationCode
    tokenUrl: https://api.telleroo.com/oauth/token
  name: PartnerOAuth2
scope_count: 1
scope_names:
- create
scopes:
- description: Permission to create pay runs on behalf of an authorizing client company. This is the only scope Telleroo's Partner (Embedded Payments) API currently documents; it is requested in the authorize URL as scope=create and echoed back in the token response.
  flows:
  - authorizationCode
  scope: create
slug: telleroo-scopes
source_filename: telleroo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://partner-docs.telleroo.com/#authentication\ndocs: https://partner-docs.telleroo.com/\nschemes:\n- name: PartnerOAuth2\n  api: Telleroo Partner API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://admin.telleroo.com/oauth\n    tokenUrl: https://api.telleroo.com/oauth/token\nscopes:\n- scope: create\n  description: >-\n    Permission to create pay runs on behalf of an authorizing client company.\n    This is the only scope Telleroo's Partner (Embedded Payments) API\n    currently documents; it is requested in the authorize URL as scope=create\n    and echoed back in the token response.\n  flows: [authorizationCode]\n  sources: [https://partner-docs.telleroo.com/]\nnotes: >-\n  The Business API (v1) does not use OAuth scopes; it authenticates with a\n  static Authorization token whose capability is set by token class\n  (Full Access vs Recipient Access), captured in\n  authentication/telleroo-authentication.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telleroo/refs/heads/main/scopes/telleroo-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Payments
- Bulk Payments
- Payroll
- Faster Payments
- E-Money
- Fintech
- Banking
- International Payments
- Embedded Finance
token_urls:
- https://api.telleroo.com/oauth/token
---
