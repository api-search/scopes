---
authorization_urls: []
description: ''
docs: https://developer.equifax.com/documentation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Equifax Scopes
name_suffix: OAuth Scopes
note: 'Equifax documents that a `scope` parameter is REQUIRED in the OAuth 2.0 client_credentials token request ("you obtain the Access Token by providing only the client_id, client_secret, and the scope"), but publishes no scope reference. Scope values are per-API-product and are rendered only on the signed-in application page in the Equifax Developer Portal — the public quick-start guide instructs integrators to "Expand each API to confirm the appropriate endpoint ''Scope'' to use in test mode" (https://assets.equifax.com/marketing/US/assets/developer-quick-start-guide.PDF). scope_count is an honest zero: zero scope values are published, not zero scopes exist. Recovering the real list requires an authenticated portal session, which this pipeline does not create.'
overview: 'Equifax uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Equifax
provider_slug: equifax
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: equifax-scopes
source_filename: equifax-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developer.equifax.com/documentation\ndocs: https://developer.equifax.com/documentation\nprovider: Equifax\nproviderId: equifax\nflow: clientCredentials\ntoken_endpoint: https://api.equifax.com/v2/oauth/token\nscope_count: 0\nscopes: []\nnote: >-\n  Equifax documents that a `scope` parameter is REQUIRED in the OAuth 2.0\n  client_credentials token request (\"you obtain the Access Token by providing only the\n  client_id, client_secret, and the scope\"), but publishes no scope reference. Scope\n  values are per-API-product and are rendered only on the signed-in application page in\n  the Equifax Developer Portal — the public quick-start guide instructs integrators to\n  \"Expand each API to confirm the appropriate endpoint 'Scope' to use in test mode\"\n  (https://assets.equifax.com/marketing/US/assets/developer-quick-start-guide.PDF).\n  scope_count is an honest zero: zero scope values are published, not zero scopes\
  \ exist.\n  Recovering the real list requires an authenticated portal session, which this pipeline\n  does not create.\ngated: true\ngate: Equifax Developer Portal sign-in (https://developer.equifax.com/user/login)\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equifax/refs/heads/main/scopes/equifax-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Credit
- Credit History
- Credit Reporting
- Identity
- Fraud Detection
- Fortune 1000
token_urls: []
---
