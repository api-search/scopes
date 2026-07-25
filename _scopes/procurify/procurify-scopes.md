---
api_specs:
- filename: procurify-account-codes-api-openapi.yml
  format: yaml
  label: Procurify account-codes API
  slug: procurify-account-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-account-codes-api-openapi.yml
- filename: procurify-accounts-api-openapi.yml
  format: yaml
  label: Procurify accounts API
  slug: procurify-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-accounts-api-openapi.yml
- filename: procurify-ap-api-openapi.yml
  format: yaml
  label: Procurify ap API
  slug: procurify-ap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-ap-api-openapi.yml
- filename: procurify-catalog-api-openapi.yml
  format: yaml
  label: Procurify catalog API
  slug: procurify-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-catalog-api-openapi.yml
- filename: procurify-currencies-api-openapi.yml
  format: yaml
  label: Procurify currencies API
  slug: procurify-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-currencies-api-openapi.yml
- filename: procurify-custom-fields-api-openapi.yml
  format: yaml
  label: Procurify custom-fields API
  slug: procurify-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-custom-fields-api-openapi.yml
- filename: procurify-departments-api-openapi.yml
  format: yaml
  label: Procurify departments API
  slug: procurify-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-departments-api-openapi.yml
- filename: procurify-locations-api-openapi.yml
  format: yaml
  label: Procurify locations API
  slug: procurify-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-locations-api-openapi.yml
- filename: procurify-oauth-api-openapi.yml
  format: yaml
  label: Procurify oauth API
  slug: procurify-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-oauth-api-openapi.yml
- filename: procurify-order-items-api-openapi.yml
  format: yaml
  label: Procurify order-items API
  slug: procurify-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-order-items-api-openapi.yml
- filename: procurify-permissions-api-openapi.yml
  format: yaml
  label: Procurify permissions API
  slug: procurify-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-permissions-api-openapi.yml
- filename: procurify-public-api-openapi.yml
  format: yaml
  label: Procurify public API
  slug: procurify-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-public-api-openapi.yml
- filename: procurify-purchase-orders-api-openapi.yml
  format: yaml
  label: Procurify purchase-orders API
  slug: procurify-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-purchase-orders-api-openapi.yml
- filename: procurify-receipt-api-openapi.yml
  format: yaml
  label: Procurify receipt API
  slug: procurify-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-receipt-api-openapi.yml
- filename: procurify-requisitions-api-openapi.yml
  format: yaml
  label: Procurify requisitions API
  slug: procurify-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-requisitions-api-openapi.yml
- filename: procurify-users-api-openapi.yml
  format: yaml
  label: Procurify users API
  slug: procurify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-users-api-openapi.yml
- filename: procurify-vendors-api-openapi.yml
  format: yaml
  label: Procurify vendors API
  slug: procurify-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-vendors-api-openapi.yml
authorization_urls:
- https://<your-domain>.procurify.com/oauth/authorize
description: ''
docs: https://developer.procurify.com/tag/oauth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Procurify Scopes
name_suffix: OAuth Scopes
note: Procurify's API supports only the OAuth 2.0 client_credentials grant and does not offer granular, selectable permission scopes; tokens are automatically scoped to the requesting domain and user email, as shown in the token response documented at https://developer.procurify.com/tag/oauth/.
overview: 'Procurify publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Procurify API on a user''s behalf.


  Tokens are issued from https://<your-domain>.procurify.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Procurify
provider_slug: procurify
schemes:
- flows:
  - authorizationUrl: https://<your-domain>.procurify.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://<your-domain>.procurify.com/oauth/token
  name: RemoteAuthentication
  source: openapi/procurify-procurify-api-openapi.yml
scope_count: 2
scope_names:
- urn:procurify-api:domain:<your_domain>
- urn:procurify-api:email:<your_email>
scopes:
- description: Automatic scope binding the access token to the requesting Procurify domain; returned in the client_credentials token response rather than requested by the client.
  flows: []
  scope: urn:procurify-api:domain:<your_domain>
- description: Automatic scope binding the access token to the email address of the user whose API credentials were used; returned in the client_credentials token response rather than requested by the client.
  flows: []
  scope: urn:procurify-api:email:<your_email>
slug: procurify-scopes
source_filename: procurify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/procurify-procurify-api-openapi.yml\ndocs: https://developer.procurify.com/tag/oauth/\nnote: >-\n  Procurify's API supports only the OAuth 2.0 client_credentials grant and does\n  not offer granular, selectable permission scopes; tokens are automatically\n  scoped to the requesting domain and user email, as shown in the token response\n  documented at https://developer.procurify.com/tag/oauth/.\nschemes:\n- name: RemoteAuthentication\n  source: openapi/procurify-procurify-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://<your-domain>.procurify.com/oauth/authorize\n    tokenUrl: https://<your-domain>.procurify.com/oauth/token\nscopes:\n- scope: urn:procurify-api:domain:<your_domain>\n  description: >-\n    Automatic scope binding the access token to the requesting Procurify\n    domain; returned in the client_credentials token response rather than\n    requested by the client.\n \
  \ sources:\n  - https://developer.procurify.com/tag/oauth/\n- scope: urn:procurify-api:email:<your_email>\n  description: >-\n    Automatic scope binding the access token to the email address of the user\n    whose API credentials were used; returned in the client_credentials token\n    response rather than requested by the client.\n  sources:\n  - https://developer.procurify.com/tag/oauth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/scopes/procurify-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Spend Management
- Procurement
- Purchase Orders
- Accounts Payable
- Vendor Management
- Budget Tracking
- Procure-to-Pay
- ERP Integration
token_urls:
- https://<your-domain>.procurify.com/oauth/token
---
