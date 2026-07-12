---
authorization_urls: []
description: ''
docs: https://developer.prove.com/tutorial/access-api-keys
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Prove Scopes
name_suffix: OAuth Scopes
note: Prove's API uses an OAuth 2.0 client_credentials flow with no published scopes - access is governed by the client_id/client_secret credentials themselves, and Prove's official server SDKs request tokens with an empty scope list (see https://developer.prove.com/tutorial/access-api-keys and https://github.com/prove-identity/prove-sdk-server-go).
overview: 'Prove uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.prove.com/v3/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Prove
provider_slug: prove
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.prove.com/v3/token
  name: oauth2
  source: openapi/prove-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: prove-scopes
source_filename: prove-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prove-openapi.yml\ndocs: https://developer.prove.com/tutorial/access-api-keys\nnote: Prove's API uses an OAuth 2.0 client_credentials flow with no published scopes\n  - access is governed by the client_id/client_secret credentials themselves, and\n  Prove's official server SDKs request tokens with an empty scope list (see\n  https://developer.prove.com/tutorial/access-api-keys and\n  https://github.com/prove-identity/prove-sdk-server-go).\nschemes:\n- name: oauth2\n  source: openapi/prove-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.prove.com/v3/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prove/refs/heads/main/scopes/prove-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Identity Verification
- Authentication
- Phone Intelligence
- KYC
- Fraud Prevention
token_urls:
- https://api.prove.com/v3/token
---
