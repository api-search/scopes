---
api_specs:
- filename: razorpay-openapi.yml
  format: yaml
  label: Razorpay Core REST API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/openapi/razorpay-openapi.yml
- filename: razorpay-webhooks-asyncapi.yml
  format: yaml
  label: Razorpay Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/asyncapi/razorpay-webhooks-asyncapi.yml
authorization_urls: []
description: Razorpay's OAuth 2.0 scopes. The core Razorpay API authenticates with HTTP Basic key_id/key_secret, not OAuth, so the OpenAPI securitySchemes carry no oauth2 scopes. OAuth is used by Razorpay Partners (technology partners / aggregators) to obtain access tokens acting on onboarded merchant accounts, and by the Razorpay MCP server. This is the searched fill capturing the partner OAuth scope surface. Multiple scopes are requested with array notation (scope[]=read_only&scope[]=rx_read_write).
docs: https://razorpay.com/docs/partners/technology-partners/onboard-businesses/integrate-oauth/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Razorpay Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Razorpay publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Razorpay API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Razorpay
provider_slug: razorpay
schemes:
- authorizationUrl: https://auth.razorpay.com/authorize
  docs: https://razorpay.com/docs/partners/technology-partners/onboard-businesses/integrate-oauth/integration-steps/
  grant_types:
  - authorization_code
  - refresh_token
  name: Razorpay Partner OAuth
  response_type: code
  tokenUrl: https://auth.razorpay.com/token
  type: oauth2
scope_count: 5
scope_names:
- read_only
- read_write
- rx_read_only
- rx_read_write
- rx_partner_read_write
scopes:
- description: Read access to all resources (all GET API requests) — view payments, refunds, etc.
  flows: []
  scope: read_only
- description: Read and write access to all resources — view and create payments, refunds, etc.
  flows: []
  scope: read_write
- description: Read access to all RazorpayX resources (all GET requests) — view payouts, contacts, etc.
  flows: []
  scope: rx_read_only
- description: Read and write access to all RazorpayX resources — view and create payouts, contacts, etc.
  flows: []
  scope: rx_read_write
- description: Fetch payouts, contacts, fund accounts, transactions, and approve or reject a payout.
  flows: []
  scope: rx_partner_read_write
slug: razorpay-scopes
source_filename: razorpay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nsource: https://razorpay.com/docs/partners/technology-partners/onboard-businesses/integrate-oauth/integration-steps/\ndocs: https://razorpay.com/docs/partners/technology-partners/onboard-businesses/integrate-oauth/\ndescription: >-\n  Razorpay's OAuth 2.0 scopes. The core Razorpay API authenticates with HTTP\n  Basic key_id/key_secret, not OAuth, so the OpenAPI securitySchemes carry no\n  oauth2 scopes. OAuth is used by Razorpay Partners (technology partners /\n  aggregators) to obtain access tokens acting on onboarded merchant accounts,\n  and by the Razorpay MCP server. This is the searched fill capturing the\n  partner OAuth scope surface. Multiple scopes are requested with array notation\n  (scope[]=read_only&scope[]=rx_read_write).\nschemes:\n  - name: Razorpay Partner OAuth\n    type: oauth2\n    grant_types: [authorization_code, refresh_token]\n    response_type: code\n    authorizationUrl: https://auth.razorpay.com/authorize\n\
  \    tokenUrl: https://auth.razorpay.com/token\n    docs: https://razorpay.com/docs/partners/technology-partners/onboard-businesses/integrate-oauth/integration-steps/\nscopes:\n  - scope: read_only\n    description: Read access to all resources (all GET API requests) — view payments, refunds, etc.\n    schemes: [Razorpay Partner OAuth]\n  - scope: read_write\n    description: Read and write access to all resources — view and create payments, refunds, etc.\n    schemes: [Razorpay Partner OAuth]\n  - scope: rx_read_only\n    description: Read access to all RazorpayX resources (all GET requests) — view payouts, contacts, etc.\n    schemes: [Razorpay Partner OAuth]\n  - scope: rx_read_write\n    description: Read and write access to all RazorpayX resources — view and create payouts, contacts, etc.\n    schemes: [Razorpay Partner OAuth]\n  - scope: rx_partner_read_write\n    description: Fetch payouts, contacts, fund accounts, transactions, and approve or reject a payout.\n    schemes: [Razorpay\
  \ Partner OAuth]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/razorpay/refs/heads/main/scopes/razorpay-scopes.yml
summary_line: 5 scopes
tags:
- Payments
- Payment Gateway
- Fintech
- India
- UPI
- Subscriptions
- Payouts
- Checkout
token_urls: []
---
