---
api_specs:
- filename: salv-aml-openapi-original.yml
  format: yaml
  label: Salv AML API
  slug: salv-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-aml-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Salv Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salv publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salv API on a user''s behalf.


  Tokens are issued from https://app.salv.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salv
provider_slug: salv
schemes:
- description: 'In order to use the API, you need to generate client credentials using [Salv UI](https://demo.salv.com/credentials).

    Never share your secret keys. Keep them guarded and secure.


    We use OAuth2 client credentials flow to issue our API tokens.

    By default our API tokens have expiration time of 50 years, so effectively they never expire.

    Please do not make any assumptions about the content of the access_token.

    At the moment we use a JWT token, but it can change to any other string with the future updates.


    An API token can be invalidated using Salv UI by deleting the client credentials that were used to generate the token.


    Please make sure you only request it once per reasonable amount of time,

    as `oauth/token` endpoint has a rate limit of **10 requests per minute** per IP address.


    | Environment | Token URL |

    |-------------|-----------|

    | Production | `https://app.salv.com/oauth/token` |

    | Sandbox | `https://demo.salv.com/oauth/token` |


    Use the token URL matching your selected server environment.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://app.salv.com/oauth/token
  name: OAuth2
  source: openapi/salv-aml-openapi-original.yml
scope_count: 1
scope_names:
- aml
scopes:
- description: Can use AML API
  flows:
  - clientCredentials
  scope: aml
slug: salv-scopes
source_filename: salv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/salv-aml-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/salv-aml-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.salv.com/oauth/token\n  description: |-\n    In order to use the API, you need to generate client credentials using [Salv UI](https://demo.salv.com/credentials).\n    Never share your secret keys. Keep them guarded and secure.\n\n    We use OAuth2 client credentials flow to issue our API tokens.\n    By default our API tokens have expiration time of 50 years, so effectively they never expire.\n    Please do not make any assumptions about the content of the access_token.\n    At the moment we use a JWT token, but it can change to any other string with the future updates.\n\n    An API token can be invalidated using Salv UI by deleting the client credentials that were used to generate the token.\n\n    Please make sure you only request it once per reasonable\
  \ amount of time,\n    as `oauth/token` endpoint has a rate limit of **10 requests per minute** per IP address.\n\n    | Environment | Token URL |\n    |-------------|-----------|\n    | Production | `https://app.salv.com/oauth/token` |\n    | Sandbox | `https://demo.salv.com/oauth/token` |\n\n    Use the token URL matching your selected server environment.\nscopes:\n- scope: aml\n  description: Can use AML API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/salv-aml-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/scopes/salv-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Anti-Money Laundering
- Financial Crime
- Compliance
- RegTech
- Sanctions Screening
- Transaction Monitoring
- Fraud Prevention
token_urls:
- https://app.salv.com/oauth/token
---
