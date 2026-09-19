---
authorization_urls: []
description: ''
docs: https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Pay Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py returned nothing because there is no OpenAPI in the repo to derive from. These three scopes were read from Google's own MCP setup page and from the Google Wallet API Discovery document, which declares its scope set machine-readably.
overview: 'Google Pay publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Pay API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Pay
provider_slug: google-pay
schemes: []
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/paydeveloper.merchant
- https://www.googleapis.com/auth/paydeveloper.issuer.readonly
- https://www.googleapis.com/auth/wallet_object.issuer
scopes:
- description: Manage Google Pay merchant data.
  flows: []
  scope: https://www.googleapis.com/auth/paydeveloper.merchant
- description: Read Google Wallet issuer data.
  flows: []
  scope: https://www.googleapis.com/auth/paydeveloper.issuer.readonly
- description: The single scope declared by the Google Wallet API Discovery document; covers all 99 walletobjects.* methods (class and object CRUD, issuer, permissions, smarttap, media, jwt).
  flows: []
  scope: https://www.googleapis.com/auth/wallet_object.issuer
slug: google-pay-scopes
source_filename: google-pay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Google Pay\nproviderId: google-pay\ngenerated: '2026-09-12'\nmethod: searched\ndocs: https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp\nsource: >-\n  https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp (MCP scopes) ·\n  discovery/google-pay-walletobjects-v1-discovery.json auth.oauth2.scopes (Wallet API scope,\n  fetched from walletobjects.googleapis.com 2026-09-12)\nnote: >-\n  derive-oauth-scopes.py returned nothing because there is no OpenAPI in the repo to derive from.\n  These three scopes were read from Google's own MCP setup page and from the Google Wallet API\n  Discovery document, which declares its scope set machine-readably.\nscopes:\n  - scope: https://www.googleapis.com/auth/paydeveloper.merchant\n    description: Manage Google Pay merchant data.\n    surface: Google Pay & Wallet Developer MCP server\n    grants:\n      - list_merchants\n      - create_merchant\n\
  \      - update_merchant\n      - list_google_pay_integrations\n      - query_merchant_performance\n      - query_merchant_error_metrics\n      - list_principals\n      - set_principal_role\n      - delete_principal\n    source: https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp\n  - scope: https://www.googleapis.com/auth/paydeveloper.issuer.readonly\n    description: Read Google Wallet issuer data.\n    surface: Google Pay & Wallet Developer MCP server\n    read_only: true\n    grants:\n      - list_pass_issuers\n      - list_pass_classes\n    source: https://developers.google.com/pay/api/web/guides/use-pay-wallet-mcp\n  - scope: https://www.googleapis.com/auth/wallet_object.issuer\n    description: >-\n      The single scope declared by the Google Wallet API Discovery document; covers all 99\n      walletobjects.* methods (class and object CRUD, issuer, permissions, smarttap, media, jwt).\n    surface: Google Wallet API (walletobjects.googleapis.com)\n    source: discovery/google-pay-walletobjects-v1-discovery.json\n\
  scope_count: 3\ngranularity_note: >-\n  The Wallet REST API is single-scope: one coarse scope authorises read AND write across every\n  pass type and the issuer/permissions surface. An agent cannot be granted read-only Wallet REST\n  access. The newer MCP surface is the only Google Pay surface that splits a read-only scope out\n  (paydeveloper.issuer.readonly).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pay/refs/heads/main/scopes/google-pay-scopes.yml
summary_line: 3 scopes
tags:
- Agentic Commerce
- Checkout
- Contactless Payments
- Digital Wallet
- Merchants
- Mobile Payments
- Payments
- Tokenization
token_urls: []
---
