---
api_specs:
- filename: td-synnex-authentication-api-openapi.yml
  format: yaml
  label: TD SYNNEX Authentication API
  slug: td-synnex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-authentication-api-openapi.yml
- filename: td-synnex-cart-items-api-openapi.yml
  format: yaml
  label: TD SYNNEX Cart Items API
  slug: td-synnex-cart-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-cart-items-api-openapi.yml
- filename: td-synnex-carts-api-openapi.yml
  format: yaml
  label: TD SYNNEX Carts API
  slug: td-synnex-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-carts-api-openapi.yml
- filename: td-synnex-cloud-providers-api-openapi.yml
  format: yaml
  label: TD SYNNEX Cloud Providers API
  slug: td-synnex-cloud-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-cloud-providers-api-openapi.yml
- filename: td-synnex-customers-api-openapi.yml
  format: yaml
  label: TD SYNNEX Customers API
  slug: td-synnex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-customers-api-openapi.yml
- filename: td-synnex-orders-api-openapi.yml
  format: yaml
  label: TD SYNNEX Orders API
  slug: td-synnex-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-orders-api-openapi.yml
- filename: td-synnex-products-api-openapi.yml
  format: yaml
  label: TD SYNNEX Products API
  slug: td-synnex-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-products-api-openapi.yml
- filename: td-synnex-provisioning-api-openapi.yml
  format: yaml
  label: TD SYNNEX Provisioning API
  slug: td-synnex-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-provisioning-api-openapi.yml
- filename: td-synnex-reports-api-openapi.yml
  format: yaml
  label: TD SYNNEX Reports API
  slug: td-synnex-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-reports-api-openapi.yml
- filename: td-synnex-subscriptions-api-openapi.yml
  format: yaml
  label: TD SYNNEX Subscriptions API
  slug: td-synnex-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/openapi/td-synnex-subscriptions-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Td Synnex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TD SYNNEX publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TD SYNNEX API on a user''s behalf.


  Tokens are issued from https://ion.tdsynnex.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TD SYNNEX
provider_slug: td-synnex
schemes:
- description: TD SYNNEX StreamOne Ion uses OAuth 2.0 with refresh token flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://ion.tdsynnex.com/oauth/token
  name: OAuth2
  source: openapi/td-synnex-streamone-ion-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to partner resources
  flows:
  - clientCredentials
  scope: read
- description: Write access to create and update resources
  flows:
  - clientCredentials
  scope: write
slug: td-synnex-scopes
source_filename: td-synnex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-synnex-streamone-ion-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/td-synnex-streamone-ion-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ion.tdsynnex.com/oauth/token\n  description: TD SYNNEX StreamOne Ion uses OAuth 2.0 with refresh token flow\nscopes:\n- scope: read\n  description: Read access to partner resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/td-synnex-streamone-ion-openapi.yml\n- scope: write\n  description: Write access to create and update resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/td-synnex-streamone-ion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-synnex/refs/heads/main/scopes/td-synnex-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Technology Distribution
- IT Distribution
- Cloud
- Reseller
- StreamOne
- Fortune 100
- B2B
token_urls:
- https://ion.tdsynnex.com/oauth/token
---
