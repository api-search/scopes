---
api_specs:
- filename: qubiqle-openapi-original.json
  format: json
  label: Ottimate API V1
  slug: ottimate-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/openapi/qubiqle-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.ottimate.com/auth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Qubiqle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Qubiqle publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Qubiqle API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qubiqle
provider_slug: qubiqle
schemes:
- flow: clientCredentials
  name: OAuth2
  token_urls:
    production: https://auth.ottimate.com/oauth/token
    sandbox: https://sandbox-auth.ottimate.com/oauth/token
scope_count: 1
scope_names:
- accounts.can_access_dashboard
scopes:
- description: The only scope currently supported. Requested at token exchange (scope=accounts.can_access_dashboard) and echoed back on the token response.
  flows:
  - clientCredentials
  scope: accounts.can_access_dashboard
slug: qubiqle-scopes
source_filename: qubiqle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/qubiqle-openapi-original.json\ndocs: https://docs.ottimate.com/auth\nschemes:\n- name: OAuth2\n  flow: clientCredentials\n  token_urls:\n    sandbox: https://sandbox-auth.ottimate.com/oauth/token\n    production: https://auth.ottimate.com/oauth/token\nscopes:\n- scope: accounts.can_access_dashboard\n  description: >-\n    The only scope currently supported. Requested at token exchange\n    (scope=accounts.can_access_dashboard) and echoed back on the token response.\n  flows: [clientCredentials]\nnotes: >-\n  Ottimate documents a single OAuth scope today. The OpenAPI securityScheme is\n  declared as http/bearer rather than a typed oauth2 flow, so this scope list is\n  captured from the documented client_credentials exchange at\n  https://docs.ottimate.com/auth, not derived from the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qubiqle/refs/heads/main/scopes/qubiqle-scopes.yml
summary_line: 1 scope
tags:
- Company
- Accounts Payable
- Invoicing
- Payments
- Accounting
- FinTech
- Automation
- Artificial Intelligence
- ERP Integration
- Procurement
token_urls: []
---
