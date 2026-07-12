---
authorization_urls:
- https://api.honeybook.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Honeybook Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HoneyBook publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HoneyBook API on a user''s behalf.


  Tokens are issued from https://api.honeybook.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HoneyBook
provider_slug: honeybook
schemes:
- description: Third-party integration guides reference OAuth 2.0 against api.honeybook.com, but are inconsistent on the exact token endpoint and grant type and are not independently verifiable. Modeled here as an authorization-code flow with refresh tokens, the most common pattern for a user-data platform of this kind; treat as unverified.
  flows:
  - authorizationUrl: https://api.honeybook.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.honeybook.com/oauth/token
  name: oauth2
  source: openapi/honeybook-openapi.yml
scope_count: 14
scope_names:
- clients.read
- clients.write
- contracts.read
- contracts.write
- invoices.read
- invoices.write
- payments.read
- projects.read
- projects.write
- proposals.read
- proposals.write
- scheduler.read
- scheduler.write
- webhooks.write
scopes:
- description: Read clients and inquiries.
  flows:
  - authorizationCode
  scope: clients.read
- description: Create and update clients and inquiries.
  flows:
  - authorizationCode
  scope: clients.write
- description: Read contracts.
  flows:
  - authorizationCode
  scope: contracts.read
- description: Create contracts.
  flows:
  - authorizationCode
  scope: contracts.write
- description: Read invoices.
  flows:
  - authorizationCode
  scope: invoices.read
- description: Create invoices.
  flows:
  - authorizationCode
  scope: invoices.write
- description: Read payments.
  flows:
  - authorizationCode
  scope: payments.read
- description: Read projects and pipeline stage.
  flows:
  - authorizationCode
  scope: projects.read
- description: Create and update projects.
  flows:
  - authorizationCode
  scope: projects.write
- description: Read proposals.
  flows:
  - authorizationCode
  scope: proposals.read
- description: Create proposals.
  flows:
  - authorizationCode
  scope: proposals.write
- description: Read session types and bookings.
  flows:
  - authorizationCode
  scope: scheduler.read
- description: Create bookings.
  flows:
  - authorizationCode
  scope: scheduler.write
- description: Manage webhook subscriptions.
  flows:
  - authorizationCode
  scope: webhooks.write
slug: honeybook-scopes
source_filename: honeybook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/honeybook-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/honeybook-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.honeybook.com/oauth/authorize\n    tokenUrl: https://api.honeybook.com/oauth/token\n  description: Third-party integration guides reference OAuth 2.0 against api.honeybook.com,\n    but are inconsistent on the exact token endpoint and grant type and are not independently\n    verifiable. Modeled here as an authorization-code flow with refresh tokens, the most common\n    pattern for a user-data platform of this kind; treat as unverified.\nscopes:\n- scope: clients.read\n  description: Read clients and inquiries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: clients.write\n  description: Create and update clients and inquiries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope:\
  \ contracts.read\n  description: Read contracts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: contracts.write\n  description: Create contracts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: invoices.read\n  description: Read invoices.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: invoices.write\n  description: Create invoices.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: payments.read\n  description: Read payments.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: projects.read\n  description: Read projects and pipeline stage.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: projects.write\n  description: Create and update projects.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: proposals.read\n\
  \  description: Read proposals.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: proposals.write\n  description: Create proposals.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: scheduler.read\n  description: Read session types and bookings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: scheduler.write\n  description: Create bookings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n- scope: webhooks.write\n  description: Manage webhook subscriptions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/honeybook-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/scopes/honeybook-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- CRM
- Clientflow
- Proposals
- Contracts
- Invoicing
- Payments
- Scheduling
- Creative Entrepreneurs
- Small Business
token_urls:
- https://api.honeybook.com/oauth/token
---
