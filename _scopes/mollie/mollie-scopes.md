---
api_specs:
- filename: mollie-openapi-original.yml
  format: yaml
  label: Mollie API
  slug: mollie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/openapi/mollie-openapi-original.yml
authorization_urls:
- https://my.mollie.com/oauth2/authorize
description: ''
docs: https://docs.mollie.com/reference/oauth2
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mollie Scopes
name_suffix: OAuth Scopes
note: 61 scopes. All 42 scopes referenced in the OpenAPI operation security requirements are a subset of the 61 published in Mollie's RFC 8414 authorization-server metadata; the extra 19 cover product areas whose operations are not (yet) in the public OpenAPI — disputes, files, persons, external accounts, pricing rates/segments, shipments, orders and business-account draft transfers.
overview: 'Mollie publishes 61 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mollie API on a user''s behalf.


  Tokens are issued from https://api.mollie.com/oauth2/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mollie
provider_slug: mollie
schemes:
- flows:
  - authorizationUrl: https://my.mollie.com/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.mollie.com/oauth2/tokens
  name: oAuth
  source: openapi/mollie-openapi-original.yml
scope_count: 61
scope_names:
- balance-reports.read
- balance-transfers.read
- balance-transfers.write
- balances.read
- business-account-draft-transfers.read
- business-account-draft-transfers.write
- business-account-payee-verifications.write
- business-account-transfers.read
- business-account-transfers.write
- business-accounts.read
- clients.read
- clients.write
- customers.read
- customers.write
- disputes.read
- disputes.write
- events.read
- external-accounts.read
- external-accounts.write
- files.read
- files.write
- invoices.read
- mandates.read
- mandates.write
- onboarding.read
- onboarding.write
- orders.read
- orders.write
- organizations.read
- organizations.write
- payment-links.read
- payment-links.write
- payments.read
- payments.write
- payouts.read
- payouts.write
- persons.read
- persons.write
- pricing-rates.read
- pricing-rates.write
- pricing-segments.read
- pricing-segments.write
- profiles.read
- profiles.write
- refunds.read
- refunds.write
- sales-invoices.read
- sales-invoices.write
- sessions.read
- sessions.write
- settlements.read
- shipments.read
- shipments.write
- subscriptions.read
- subscriptions.write
- terminals.read
- terminals.write
- unmatched-credit-transfers.read
- unmatched-credit-transfers.write
- webhooks.read
- webhooks.write
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: balance-reports.read
- description: ''
  flows:
  - authorizationCode
  scope: balance-transfers.read
- description: ''
  flows:
  - authorizationCode
  scope: balance-transfers.write
- description: ''
  flows:
  - authorizationCode
  scope: balances.read
- description: ''
  flows:
  - authorizationCode
  scope: business-account-draft-transfers.read
- description: ''
  flows:
  - authorizationCode
  scope: business-account-draft-transfers.write
- description: ''
  flows:
  - authorizationCode
  scope: business-account-payee-verifications.write
- description: ''
  flows:
  - authorizationCode
  scope: business-account-transfers.read
- description: ''
  flows:
  - authorizationCode
  scope: business-account-transfers.write
- description: ''
  flows:
  - authorizationCode
  scope: business-accounts.read
- description: ''
  flows:
  - authorizationCode
  scope: clients.read
- description: ''
  flows:
  - authorizationCode
  scope: clients.write
- description: ''
  flows:
  - authorizationCode
  scope: customers.read
- description: ''
  flows:
  - authorizationCode
  scope: customers.write
- description: ''
  flows:
  - authorizationCode
  scope: disputes.read
- description: ''
  flows:
  - authorizationCode
  scope: disputes.write
- description: ''
  flows:
  - authorizationCode
  scope: events.read
- description: ''
  flows:
  - authorizationCode
  scope: external-accounts.read
- description: ''
  flows:
  - authorizationCode
  scope: external-accounts.write
- description: ''
  flows:
  - authorizationCode
  scope: files.read
- description: ''
  flows:
  - authorizationCode
  scope: files.write
- description: ''
  flows:
  - authorizationCode
  scope: invoices.read
- description: ''
  flows:
  - authorizationCode
  scope: mandates.read
- description: ''
  flows:
  - authorizationCode
  scope: mandates.write
- description: ''
  flows:
  - authorizationCode
  scope: onboarding.read
- description: ''
  flows:
  - authorizationCode
  scope: onboarding.write
- description: ''
  flows:
  - authorizationCode
  scope: orders.read
- description: ''
  flows:
  - authorizationCode
  scope: orders.write
- description: ''
  flows:
  - authorizationCode
  scope: organizations.read
- description: ''
  flows:
  - authorizationCode
  scope: organizations.write
- description: ''
  flows:
  - authorizationCode
  scope: payment-links.read
- description: ''
  flows:
  - authorizationCode
  scope: payment-links.write
- description: ''
  flows:
  - authorizationCode
  scope: payments.read
- description: ''
  flows:
  - authorizationCode
  scope: payments.write
- description: ''
  flows:
  - authorizationCode
  scope: payouts.read
- description: ''
  flows:
  - authorizationCode
  scope: payouts.write
- description: ''
  flows:
  - authorizationCode
  scope: persons.read
- description: ''
  flows:
  - authorizationCode
  scope: persons.write
- description: ''
  flows:
  - authorizationCode
  scope: pricing-rates.read
- description: ''
  flows:
  - authorizationCode
  scope: pricing-rates.write
- description: ''
  flows:
  - authorizationCode
  scope: pricing-segments.read
- description: ''
  flows:
  - authorizationCode
  scope: pricing-segments.write
- description: ''
  flows:
  - authorizationCode
  scope: profiles.read
- description: ''
  flows:
  - authorizationCode
  scope: profiles.write
- description: ''
  flows:
  - authorizationCode
  scope: refunds.read
- description: ''
  flows:
  - authorizationCode
  scope: refunds.write
- description: ''
  flows:
  - authorizationCode
  scope: sales-invoices.read
- description: ''
  flows:
  - authorizationCode
  scope: sales-invoices.write
- description: ''
  flows:
  - authorizationCode
  scope: sessions.read
- description: ''
  flows:
  - authorizationCode
  scope: sessions.write
- description: ''
  flows:
  - authorizationCode
  scope: settlements.read
- description: ''
  flows:
  - authorizationCode
  scope: shipments.read
- description: ''
  flows:
  - authorizationCode
  scope: shipments.write
- description: ''
  flows:
  - authorizationCode
  scope: subscriptions.read
- description: ''
  flows:
  - authorizationCode
  scope: subscriptions.write
- description: ''
  flows:
  - authorizationCode
  scope: terminals.read
- description: ''
  flows:
  - authorizationCode
  scope: terminals.write
- description: ''
  flows:
  - authorizationCode
  scope: unmatched-credit-transfers.read
- description: ''
  flows:
  - authorizationCode
  scope: unmatched-credit-transfers.write
- description: ''
  flows:
  - authorizationCode
  scope: webhooks.read
- description: ''
  flows:
  - authorizationCode
  scope: webhooks.write
slug: mollie-scopes
source_filename: mollie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://my.mollie.com/.well-known/oauth-authorization-server\ndocs: https://docs.mollie.com/reference/oauth2\nalso_derived_from: openapi/mollie-openapi-original.yml\nnote: >-\n  61 scopes. All 42 scopes referenced in the OpenAPI operation security requirements are\n  a subset of the 61 published in Mollie's RFC 8414 authorization-server metadata; the\n  extra 19 cover product areas whose operations are not (yet) in the public OpenAPI —\n  disputes, files, persons, external accounts, pricing rates/segments, shipments, orders\n  and business-account draft transfers.\nschemes:\n- name: oAuth\n  source: openapi/mollie-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.mollie.com/oauth2/authorize\n    tokenUrl: https://api.mollie.com/oauth2/tokens\n    pkce: S256\nscopes:\n- scope: balance-reports.read\n  resource: balance-reports\n  access: read\n  flows: [authorizationCode]\n  sources:\
  \ [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: balance-transfers.read\n  resource: balance-transfers\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: balance-transfers.write\n  resource: balance-transfers\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: balances.read\n  resource: balances\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: business-account-draft-transfers.read\n  resource: business-account-draft-transfers\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: business-account-draft-transfers.write\n\
  \  resource: business-account-draft-transfers\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: business-account-payee-verifications.write\n  resource: business-account-payee-verifications\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: business-account-transfers.read\n  resource: business-account-transfers\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: business-account-transfers.write\n  resource: business-account-transfers\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: business-accounts.read\n  resource: business-accounts\n  access: read\n  flows:\
  \ [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: clients.read\n  resource: clients\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: clients.write\n  resource: clients\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: customers.read\n  resource: customers\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: customers.write\n  resource: customers\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: disputes.read\n  resource: disputes\n\
  \  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: disputes.write\n  resource: disputes\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: events.read\n  resource: events\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: external-accounts.read\n  resource: external-accounts\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: external-accounts.write\n  resource: external-accounts\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: files.read\n  resource: files\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n\
  - scope: files.write\n  resource: files\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: invoices.read\n  resource: invoices\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: mandates.read\n  resource: mandates\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: mandates.write\n  resource: mandates\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: onboarding.read\n  resource: onboarding\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: onboarding.write\n\
  \  resource: onboarding\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: orders.read\n  resource: orders\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: orders.write\n  resource: orders\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: organizations.read\n  resource: organizations\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: organizations.write\n  resource: organizations\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: payment-links.read\n  resource: payment-links\n  access: read\n  flows: [authorizationCode]\n\
  \  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: payment-links.write\n  resource: payment-links\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: payments.read\n  resource: payments\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: payments.write\n  resource: payments\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: payouts.read\n  resource: payouts\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: payouts.write\n  resource: payouts\n  access: write\n\
  \  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: persons.read\n  resource: persons\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: persons.write\n  resource: persons\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: pricing-rates.read\n  resource: pricing-rates\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: pricing-rates.write\n  resource: pricing-rates\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: pricing-segments.read\n  resource: pricing-segments\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n\
  - scope: pricing-segments.write\n  resource: pricing-segments\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: profiles.read\n  resource: profiles\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: profiles.write\n  resource: profiles\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: refunds.read\n  resource: refunds\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: refunds.write\n  resource: refunds\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n\
  - scope: sales-invoices.read\n  resource: sales-invoices\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: sales-invoices.write\n  resource: sales-invoices\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: sessions.read\n  resource: sessions\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: sessions.write\n  resource: sessions\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: settlements.read\n  resource: settlements\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server,\
  \ openapi/mollie-openapi-original.yml]\n- scope: shipments.read\n  resource: shipments\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: shipments.write\n  resource: shipments\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server]\n- scope: subscriptions.read\n  resource: subscriptions\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: subscriptions.write\n  resource: subscriptions\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: terminals.read\n  resource: terminals\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n\
  - scope: terminals.write\n  resource: terminals\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: unmatched-credit-transfers.read\n  resource: unmatched-credit-transfers\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: unmatched-credit-transfers.write\n  resource: unmatched-credit-transfers\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: webhooks.read\n  resource: webhooks\n  access: read\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server, openapi/mollie-openapi-original.yml]\n- scope: webhooks.write\n  resource: webhooks\n  access: write\n  flows: [authorizationCode]\n  sources: [https://my.mollie.com/.well-known/oauth-authorization-server,\
  \ openapi/mollie-openapi-original.yml]"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mollie/refs/heads/main/scopes/mollie-scopes.yml
summary_line: 61 scopes · authorizationCode
tags:
- Company
- Payments
- Fintech
- Financial-Services
- Checkout
- E-Commerce
- Subscription
- Point-of-Sale
- Europe
- Netherlands
token_urls:
- https://api.mollie.com/oauth2/tokens
---
