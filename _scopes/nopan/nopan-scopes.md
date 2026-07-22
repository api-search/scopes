---
api_specs:
- filename: nopan-openapi-original.yml
  format: yaml
  label: Nopan API
  slug: nopan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nopan/refs/heads/main/openapi/nopan-openapi-original.yml
authorization_urls: []
description: OAuth2 client_credentials scopes for the Nopan API. Scopes are requested as a space-delimited `scope` form parameter on POST /auth/token; the default is payments:read. Captured from the /auth/token operation in the OpenAPI definition.
docs: https://docs.nopan.com/guides/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Nopan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nopan publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nopan API on a user''s behalf.


  Tokens are issued from https://api.nopan.io/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nopan
provider_slug: nopan
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.nopan.io/auth/token
  name: OAuth2ClientCredentials
  source: openapi/nopan-openapi-original.yml
scope_count: 2
scope_names:
- payments:read
- payments:process
scopes:
- description: Read access to payments (default scope).
  flows:
  - clientCredentials
  scope: payments:read
- description: Process/mutate payments (initiate, finalize, charge, capture, cancel, refund).
  flows:
  - clientCredentials
  scope: payments:process
slug: nopan-scopes
source_filename: nopan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nopan-openapi-original.yml\ndocs: https://docs.nopan.com/guides/authentication\ndescription: >-\n  OAuth2 client_credentials scopes for the Nopan API. Scopes are requested as a\n  space-delimited `scope` form parameter on POST /auth/token; the default is\n  payments:read. Captured from the /auth/token operation in the OpenAPI definition.\nschemes:\n  - name: OAuth2ClientCredentials\n    source: openapi/nopan-openapi-original.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.nopan.io/auth/token\nscopes:\n  - scope: payments:read\n    description: Read access to payments (default scope).\n    flows: [clientCredentials]\n    sources: [openapi/nopan-openapi-original.yml]\n  - scope: payments:process\n    description: Process/mutate payments (initiate, finalize, charge, capture, cancel, refund).\n    flows: [clientCredentials]\n    sources: [openapi/nopan-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nopan/refs/heads/main/scopes/nopan-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Payments
- Payment Service Provider
- Account to Account
- Wallet Payments
- Open Banking
- PSD2
- Fintech
- Europe
- Tokenization
- Recurring Payments
token_urls:
- https://api.nopan.io/auth/token
---
