---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Liqid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LIQID Investments uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LIQID Investments
provider_slug: liqid
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: liqid-scopes
source_filename: liqid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://authentication.liqid.de/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  LIQID publishes no scope reference page - there is no developer program to document\n  one for. These scopes are read directly from the scopes_supported array of the\n  anonymously served OpenID Connect discovery document for the customer identity\n  provider, and are the standard OIDC claim scopes rather than a product permission model.\nscope_count: 14\nscopes:\n- name: openid\n  description: Request an ID token (OpenID Connect core).\n- name: profile\n  description: Basic profile claims.\n- name: offline_access\n  description: Issue a refresh token.\n- name: name\n  description: Full name claim.\n- name: given_name\n  description: Given name claim.\n- name: family_name\n  description: Family name claim.\n- name: nickname\n  description: Nickname claim.\n- name: email\n  description: Email address claim.\n- name: email_verified\n\
  \  description: Email verification status claim.\n- name: picture\n  description: Profile picture claim.\n- name: created_at\n  description: Account creation timestamp claim.\n- name: identities\n  description: Linked identity provider records.\n- name: phone\n  description: Phone number claim.\n- name: address\n  description: Postal address claim.\nother_surfaces:\n- host: app.liqid.de\n  source: https://app.liqid.de/.well-known/openid-configuration\n  scope_count: 36\n  note: >-\n    Not enumerated here as LIQID scopes. The app.liqid.de discovery document advertises\n    36 scopes, all of them Salesforce platform scopes (cdp_ingest_api, cdp_query_api,\n    wave_api, pardot_api, chatter_api, einstein_gpt_api, mcp_api, ...), which describe\n    the hosting platform rather than anything LIQID designed or documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liqid/refs/heads/main/scopes/liqid-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Wealth Management
- Investing
- Financial-Services
- Private Equity
- Venture Capital
- Asset Management
- Fintech
- Germany
- BaFin
token_urls: []
---
