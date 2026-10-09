---
api_specs:
- filename: centrapay-payment-requests-api-openapi.yml
  format: yaml
  label: Centrapay Payment Requests API
  slug: centrapay-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/openapi/centrapay-payment-requests-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.centrapay.com/api/auth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Centrapay Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 scheme. These are the OIDC scopes_supported published by the Centrapay authorization server (HTTP 200). API authorization is role/permission based (e.g. payment-requests:pay), documented on the Auth page, not OAuth scope based.
overview: 'Centrapay publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Centrapay API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Centrapay
provider_slug: centrapay
schemes: []
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: profile
slug: centrapay-scopes
source_filename: centrapay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: 'generated: ''2026-10-09''

  method: probed

  source: https://auth.centrapay.com/.well-known/openid-configuration

  docs: https://docs.centrapay.com/api/auth

  note: The OpenAPI declares no oauth2 scheme. These are the OIDC scopes_supported published by the Centrapay authorization server (HTTP 200). API authorization is role/permission based (e.g. payment-requests:pay), documented on the Auth page, not OAuth scope based.

  scopes:

  - name: openid

  - name: email

  - name: phone

  - name: profile

  '
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrapay/refs/heads/main/scopes/centrapay-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Payments
- Digital Wallets
- Open Banking
- QR Code Payments
- Loyalty
- Gift Cards
- Fintech
token_bound: false
token_urls: []
---
