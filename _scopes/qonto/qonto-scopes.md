---
api_specs:
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Business API
  slug: qonto-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Transactions & Statements API
  slug: qonto-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Transfers API
  slug: qonto-sepa-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto International Transfers API
  slug: qonto-international-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Internal Transfers API
  slug: qonto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Cards API
  slug: qonto-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Client Invoices & Quotes API
  slug: qonto-client-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Supplier Invoices API
  slug: qonto-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Direct Debit API
  slug: qonto-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Payment Links API
  slug: qonto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Terminals API
  slug: qonto-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Webhooks API
  slug: qonto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Onboarding API
  slug: qonto-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Embed SDK & Hosted Pages API
  slug: qonto-embed-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
authorization_urls:
- https://oauth.qonto.com/oauth2/auth
description: ''
docs: https://docs.qonto.com/get-started/business-api/authentication/oauth/available-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Qonto Scopes
name_suffix: OAuth Scopes
note: Scopes derived from the OpenAPI oauth2 flow and confirmed against Qonto's published "Available scopes" reference. Qonto uses per-resource scopes of the form <resource>.<read|write> (e.g. organization.read, payment.write, card.write, sepa_direct_debit.write, webhook).
overview: 'Qonto publishes 35 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Qonto API on a user''s behalf.


  Tokens are issued from https://thirdparty.qonto.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qonto
provider_slug: qonto
schemes:
- description: OAuth 2.0 authorization code flow. Access tokens are valid 1 hour; refresh tokens 90 days (offline_access). Bearer access token sent in the Authorization header.
  flows:
  - authorizationUrl: https://oauth.qonto.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://thirdparty.qonto.com/oauth2/token
  name: OAuth
  source: openapi/qonto-openapi.yml
scope_count: 35
scope_names:
- attachment.read
- attachment.write
- beneficiary.trust
- card.read
- card.write
- client.read
- client.write
- client_invoice.write
- client_invoices.read
- einvoicing.read
- embed_auth_link.write
- insurance_contract.read
- insurance_contract.write
- internal_transfer.write
- international_transfer.write
- membership.read
- membership.write
- offline_access
- openid
- organization.read
- payment.write
- payment_link.read
- payment_link.write
- product.read
- product.write
- sepa_direct_debit.read
- sepa_direct_debit.write
- subscription.read
- supplier_invoice.read
- supplier_invoice.write
- team.read
- team.write
- terminal.read
- terminal.write
- webhook
scopes:
- description: Read attachments
  flows:
  - authorizationCode
  scope: attachment.read
- description: Upload attachments
  flows:
  - authorizationCode
  scope: attachment.write
- description: Trust SEPA beneficiaries
  flows:
  - authorizationCode
  scope: beneficiary.trust
- description: Read cards
  flows:
  - authorizationCode
  scope: card.read
- description: Manage cards
  flows:
  - authorizationCode
  scope: card.write
- description: Read clients (customers)
  flows:
  - authorizationCode
  scope: client.read
- description: Manage clients (customers)
  flows:
  - authorizationCode
  scope: client.write
- description: Manage client invoices, quotes, credit notes
  flows:
  - authorizationCode
  scope: client_invoice.write
- description: Read client invoices, quotes, credit notes
  flows:
  - authorizationCode
  scope: client_invoices.read
- description: Read e-invoicing settings
  flows:
  - authorizationCode
  scope: einvoicing.read
- description: Create Embed Auth Links
  flows:
  - authorizationCode
  scope: embed_auth_link.write
- description: Read insurance contracts
  flows:
  - authorizationCode
  scope: insurance_contract.read
- description: Manage insurance contracts
  flows:
  - authorizationCode
  scope: insurance_contract.write
- description: Create internal transfers
  flows:
  - authorizationCode
  scope: internal_transfer.write
- description: Create international transfers and beneficiaries
  flows:
  - authorizationCode
  scope: international_transfer.write
- description: Read the authenticated membership
  flows:
  - authorizationCode
  scope: membership.read
- description: Create memberships
  flows:
  - authorizationCode
  scope: membership.write
- description: Issue a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect ID token
  flows:
  - authorizationCode
  scope: openid
- description: Read organization, accounts, memberships, labels, transactions
  flows:
  - authorizationCode
  scope: organization.read
- description: Create SEPA transfers and manage beneficiaries
  flows:
  - authorizationCode
  scope: payment.write
- description: Read payment links
  flows:
  - authorizationCode
  scope: payment_link.read
- description: Manage payment links
  flows:
  - authorizationCode
  scope: payment_link.write
- description: Read products
  flows:
  - authorizationCode
  scope: product.read
- description: Manage products
  flows:
  - authorizationCode
  scope: product.write
- description: Read SEPA Direct Debit collections/mandates
  flows:
  - authorizationCode
  scope: sepa_direct_debit.read
- description: Manage SEPA Direct Debit mandates/subscriptions
  flows:
  - authorizationCode
  scope: sepa_direct_debit.write
- description: Read the organization subscription plan
  flows:
  - authorizationCode
  scope: subscription.read
- description: Read supplier invoices
  flows:
  - authorizationCode
  scope: supplier_invoice.read
- description: Manage supplier invoices
  flows:
  - authorizationCode
  scope: supplier_invoice.write
- description: Read teams
  flows:
  - authorizationCode
  scope: team.read
- description: Create teams
  flows:
  - authorizationCode
  scope: team.write
- description: Read terminals and terminal payments
  flows:
  - authorizationCode
  scope: terminal.read
- description: Create terminal payments
  flows:
  - authorizationCode
  scope: terminal.write
- description: Manage webhook subscriptions
  flows:
  - authorizationCode
  scope: webhook
slug: qonto-scopes
source_filename: qonto-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/qonto-openapi.yml\ndocs: https://docs.qonto.com/get-started/business-api/authentication/oauth/available-scopes\nnote: >-\n  Scopes derived from the OpenAPI oauth2 flow and confirmed against Qonto's\n  published \"Available scopes\" reference. Qonto uses per-resource scopes of the\n  form <resource>.<read|write> (e.g. organization.read, payment.write,\n  card.write, sepa_direct_debit.write, webhook).\nschemes:\n- name: OAuth\n  source: openapi/qonto-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.qonto.com/oauth2/auth\n    tokenUrl: https://thirdparty.qonto.com/oauth2/token\n  description: OAuth 2.0 authorization code flow. Access tokens are valid 1 hour; refresh tokens\n    90 days (offline_access). Bearer access token sent in the Authorization header.\nscopes:\n- scope: attachment.read\n  description: Read attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n\
  - scope: attachment.write\n  description: Upload attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: beneficiary.trust\n  description: Trust SEPA beneficiaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: card.read\n  description: Read cards\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: card.write\n  description: Manage cards\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: client.read\n  description: Read clients (customers)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: client.write\n  description: Manage clients (customers)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: client_invoice.write\n  description: Manage client invoices, quotes, credit notes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: client_invoices.read\n\
  \  description: Read client invoices, quotes, credit notes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: einvoicing.read\n  description: Read e-invoicing settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: embed_auth_link.write\n  description: Create Embed Auth Links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: insurance_contract.read\n  description: Read insurance contracts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: insurance_contract.write\n  description: Manage insurance contracts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: internal_transfer.write\n  description: Create internal transfers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: international_transfer.write\n  description: Create international transfers and beneficiaries\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: membership.read\n  description: Read the authenticated membership\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: membership.write\n  description: Create memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: offline_access\n  description: Issue a refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: openid\n  description: OpenID Connect ID token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: organization.read\n  description: Read organization, accounts, memberships, labels, transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: payment.write\n  description: Create SEPA transfers and manage beneficiaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: payment_link.read\n\
  \  description: Read payment links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: payment_link.write\n  description: Manage payment links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: product.read\n  description: Read products\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: product.write\n  description: Manage products\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: sepa_direct_debit.read\n  description: Read SEPA Direct Debit collections/mandates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: sepa_direct_debit.write\n  description: Manage SEPA Direct Debit mandates/subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: subscription.read\n  description: Read the organization subscription plan\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n\
  - scope: supplier_invoice.read\n  description: Read supplier invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: supplier_invoice.write\n  description: Manage supplier invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: team.read\n  description: Read teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: team.write\n  description: Create teams\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: terminal.read\n  description: Read terminals and terminal payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: terminal.write\n  description: Create terminal payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n- scope: webhook\n  description: Manage webhook subscriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/qonto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/scopes/qonto-scopes.yml
summary_line: 35 scopes · authorizationCode
tags:
- Business Banking
- Neobank
- Fintech
- Payments
- SEPA
- Open Banking
- EUR
- Europe
token_urls:
- https://thirdparty.qonto.com/oauth2/token
---
