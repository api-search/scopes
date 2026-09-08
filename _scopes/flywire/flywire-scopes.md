---
authorization_urls: []
description: ''
docs: https://solutions.flywire.com/en/invoicing/invoicing-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Flywire Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flywire uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flywire
provider_slug: flywire
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: flywire-scopes
source_filename: flywire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://solutions.flywire.com/en/invoicing/invoicing-api\ndocs: https://solutions.flywire.com/en/invoicing/invoicing-api\nnotes: >-\n  OAuth 2.0 scopes apply to the Flywire INVOICING API only. Flywire runs three\n  different authorization models across three APIs, and only this one has scopes:\n  the Payments API (api-platform.flywire.com) uses a static X-Authentication-Key\n  header with no scope surface, and the Payment Request API (app.flywire.com) uses\n  an HMAC-SHA256 request digest. Scopes are granted to an APPLICATION at\n  registration — there is no consent screen, no authorization-code flow and no\n  user-delegated grant; the only flow is client_credentials. There is also no\n  published OAuth discovery document: /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration 404 on api.flywire.com, invoicing.flywire.com,\n  app.flywire.com and www.flywire.com (probed 2026-09-02), so an agent cannot\n\
  \  discover these scopes at runtime — they exist only in prose on this page.\n  Derived baseline could not be produced: Flywire publishes no OpenAPI, so\n  derive-oauth-scopes.py returned zero schemes. Every scope below is read verbatim\n  from the provider's own scope table.\napi: Flywire Invoicing API\noauth:\n  version: '2.0'\n  grant_types: [client_credentials]\n  token_endpoint: https://api.flywire.com/oauth/token\n  token_request_content: JSON body with grant_type, client_id, client_secret\n  token_response_fields: [access_token, expires_in]\n  token_use: 'Authorization: Bearer {access_token}'\n  discovery_document: null\n  registration: Manual — scopes are granted to the application when Flywire registers it.\nscope_count: 16\nscopes:\n- name: invoicing.contact.read\n  grants: 'Contacts: search, read, count'\n  resource: contact\n  access: read\n- name: invoicing.contact.write\n  grants: 'Contacts: create, update, delete'\n  resource: contact\n  access: write\n- name: invoicing.invoice.read\n\
  \  grants: 'Invoices: search, read, count, export'\n  resource: invoice\n  access: read\n- name: invoicing.invoice.write\n  grants: 'Invoices: create, update, delete, send reminders'\n  resource: invoice\n  access: write\n- name: invoicing.creditnote.read\n  grants: 'Credit notes: search, read, count'\n  resource: creditnote\n  access: read\n- name: invoicing.creditnote.write\n  grants: 'Credit notes: create, update, delete, allocate'\n  resource: creditnote\n  access: write\n- name: invoicing.payments.read\n  grants: 'Payments: search, read, export'\n  resource: payments\n  access: read\n- name: invoicing.payments.write\n  grants: 'Payments: record manual payments, initiate payments, delete'\n  resource: payments\n  access: write\n- name: invoicing.company.read\n  grants: Company, company settings, pay now codes, bank accounts, predefined services\n  resource: company\n  access: read\n- name: invoicing.company.update\n  grants: Company settings and webhook subscriptions\n  resource: company\n\
  \  access: write\n- name: invoicing.company.write\n  grants: Company creation\n  resource: company\n  access: write\n- name: invoicing.payment_method.read\n  grants: Stored payer payment methods (read)\n  resource: payment_method\n  access: read\n- name: invoicing.payment_method.write\n  grants: Stored payer payment methods (write)\n  resource: payment_method\n  access: write\n- name: invoicing.payment.charge\n  grants: Charging a stored payment method\n  resource: payment\n  access: write\n- name: invoicing.payment_request.read\n  grants: Payment requests (read)\n  resource: payment_request\n  access: read\n- name: invoicing.payment_request.write\n  grants: Payment requests (write)\n  resource: payment_request\n  access: write\nauthorization_axes:\n- axis: scope\n  rule: The token must carry the scope for the resource and operation.\n  failure: 403 with no body\n- axis: company\n  rule: >-\n    The token must be scoped to the company in the URL. The :reference path\n    segment is matched\
  \ against the accounts the token was issued for; a token for\n    another company gets 403, whatever its scopes.\n  failure: 403 with no body\nunreachable_operations_note: >-\n  Permissions that belong to dashboard users (rather than to applications) are\n  never granted to an application token — an operation that requires one is not\n  reachable through the API at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flywire/refs/heads/main/scopes/flywire-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Payments
- Cross-Border Payments
- Fintech
- Education Payments
- Healthcare Payments
- Travel Payments
- B2B Payments
- Checkout
- Webhook
token_urls: []
---
