---
api_specs:
- filename: meow-openapi.yaml
  format: yaml
  label: Meow API
  slug: meow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meow/refs/heads/main/openapi/meow-openapi.yaml
authorization_urls: []
description: ''
docs: https://developer.meow.com/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Meow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Meow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meow
provider_slug: meow
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: meow-scopes
source_filename: meow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/meow-openapi.yaml\ndocs: https://developer.meow.com/authentication\nmcp_docs: https://developer.meow.com/mcp/authentication\nnotes: >-\n  Meow scopes exist on two surfaces. The REST API key carries fine-grained\n  scopes (declared as x-scopes on the apiKeyAuth security scheme and documented\n  on the changelog as they shipped). The Meow MCP server exposes four coarse\n  OAuth 2.1 meow.* scopes that map onto groups of the API-key scopes. The\n  narrower of role and granted scope always wins.\noauth_scopes:\n- scope: meow.read\n  description: >-\n    All read access: accounts, balances, transactions, payment networks,\n    contacts, billing, bills, and cards. Always granted (locked on).\n  maps_to:\n  - accounts:read\n  - accounts:balances\n  - accounts:transactions\n  - accounts:payment_networks\n  - contacts:read\n  - billing:products:read\n  - billing:customers:read\n  - billing:invoices:read\n  - billing:accounts:read\n\
  \  - billpay:read\n  - cards:read\n- scope: meow.transfers\n  description: Draft ACH, scheduled ACH, wire, book, and crypto payments (for human approval).\n  maps_to:\n  - transfers:ach:write\n  - transfers:wire:write\n  - transfers:book:write\n  - transfers:crypto:write\n- scope: meow.cards\n  description: Issue, update, freeze, and revoke virtual cards.\n  maps_to:\n  - cards:write\n- scope: meow.billing\n  description: Create and manage invoicing products, customers, and invoices.\n  maps_to:\n  - billing:invoices:write\n  - billing:customers:write\n  - billing:products:write\napi_key_scopes:\n- scope: accounts:read\n  description: Read account information.\n- scope: accounts:write\n  description: Create, update, and close bank accounts.\n- scope: accounts:payment-networks\n  description: List payment networks supported by an account.\n- scope: accounts:transactions\n  description: List account transactions.\n- scope: accounts:balances\n  description: List account balances.\n- scope:\
  \ accounts:statements\n  description: Access account statements.\n- scope: accounts:tax-documents\n  description: Access account tax documents (1099 family).\n- scope: entity:create\n  description: Create a business entity.\n- scope: transfers:crypto:write\n  description: Create crypto (USDC) transactions.\n- scope: transfers:usdc:write\n  description: Legacy USDC transfer scope (superseded by transfers:crypto:write).\n- scope: transfers:ach:write\n  description: Create ACH transfers.\n- scope: transfers:wire:write\n  description: Create wire transfers.\n- scope: transfers:book:write\n  description: Create internal book transfers.\n- scope: contacts:read\n  description: Read payment contacts.\n- scope: contacts:write\n  description: Create, update, and delete payment contacts.\n- scope: billing:products:read\n  description: Read invoicing products.\n- scope: billing:products:write\n  description: Create and manage invoicing products.\n- scope: billing:customers:read\n  description: Read\
  \ invoicing customers.\n- scope: billing:customers:write\n  description: Create and manage invoicing customers.\n- scope: billing:invoices:read\n  description: Read invoices and line items.\n- scope: billing:invoices:write\n  description: Create and manage invoices.\n- scope: billing:accounts:read\n  description: Read collection accounts.\n- scope: billpay:read\n  description: Read bills.\n- scope: billpay:write\n  description: Create, update, and delete bills.\n- scope: onboarding:read\n  description: Read business-entity onboarding status.\n- scope: onboarding:write\n  description: Manage business-entity onboarding (representatives, documents, submission).\n- scope: cards:read\n  description: Read cards, card transactions, and spending insights.\n- scope: cards:write\n  description: Issue, update, freeze, and revoke cards.\n- scope: webhooks:read\n  description: Read webhook subscriptions and delivery history.\n- scope: webhooks:write\n  description: Create, update, and delete webhook\
  \ subscriptions.\n- scope: partner:onboarding:read\n  description: Read partner onboarding applications.\n- scope: partner:onboarding:write\n  description: Create and manage partner onboarding applications.\n- scope: partner:webhooks:read\n  description: Read partner webhook subscriptions and deliveries.\n- scope: partner:webhooks:write\n  description: Create and manage partner webhook subscriptions.\n- scope: simulations:write\n  description: Run sandbox simulation endpoints (sandbox/dev only).\n- scope: banking:limits:read\n  description: Read daily withdrawal limits.\n- scope: banking:limits:write\n  description: Set daily withdrawal limits.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meow/refs/heads/main/scopes/meow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Banking
- Fintech
- Business Banking
- Payments
- Cards
- Invoicing
- Treasury
- Cryptocurrency
- Webhooks
- MCP
- API
token_urls: []
---
