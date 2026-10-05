---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pbs Biotech Scopes
name_suffix: OAuth Scopes
note: These are the Shopify customer-account scopes advertised by the discovery document served on PBS Biotech's own store hosts. There is no PBS Biotech-authored scope surface — the company publishes no API of its own. No scope reference page is published; the descriptions below are the standard meanings of the scope identifiers as advertised, not additional claims.
overview: 'PBS Biotech publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the PBS Biotech API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PBS Biotech
provider_slug: pbs-biotech
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the signed-in buyer.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope; releases the email and email_verified claims.
  flows: []
  scope: email
- description: Full access to the signed-in buyer's customer account (orders, addresses, profile).
  flows: []
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API for the signed-in buyer — the authenticated counterpart to the anonymous storefront UCP/MCP endpoint.
  flows: []
  scope: customer-account-mcp-api:full
slug: pbs-biotech-scopes
source_filename: pbs-biotech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported from https://shoppbsbiotech.com/.well-known/openid-configuration and\n  https://account.shoppbsbiotech.com/.well-known/openid-configuration (both HTTP 200, probed 2026-08-26).\nauthorization_server: https://shopify.com/authentication/71340753133\nprotected_resource: https://account.shoppbsbiotech.com\nnote: >-\n  These are the Shopify customer-account scopes advertised by the discovery document served on PBS\n  Biotech's own store hosts. There is no PBS Biotech-authored scope surface — the company publishes no\n  API of its own. No scope reference page is published; the descriptions below are the standard meanings\n  of the scope identifiers as advertised, not additional claims.\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token for the signed-in buyer.\n- name: email\n  description: Standard OpenID Connect scope; releases the email and email_verified\
  \ claims.\n- name: 'customer-account-api:full'\n  description: Full access to the signed-in buyer's customer account (orders, addresses, profile).\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account MCP API for the signed-in buyer — the authenticated counterpart\n    to the anonymous storefront UCP/MCP endpoint.\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pbs-biotech/refs/heads/main/scopes/pbs-biotech-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Life Sciences
- Biotechnology
- Bioprocessing
- Cell Therapy
- Laboratory Equipment
- Manufacturing
- E-Commerce
- Agentic Commerce
- MCP
token_bound: false
token_urls: []
---
