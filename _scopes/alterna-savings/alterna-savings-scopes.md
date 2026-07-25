---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Alterna Savings Scopes
name_suffix: OAuth Scopes
note: OAuth2/OIDC scopes advertised by the Umbraco CMS Delivery API member-security authorization server (website member login). These are the standard OIDC baseline scopes, not banking/data-access scopes — Alterna exposes no first-party banking API and documents no data-sharing scopes.
overview: 'Alterna Savings uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alterna Savings
provider_slug: alterna-savings
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: alterna-savings-scopes
source_filename: alterna-savings-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.alterna.ca/.well-known/openid-configuration\nnote: >-\n  OAuth2/OIDC scopes advertised by the Umbraco CMS Delivery API member-security\n  authorization server (website member login). These are the standard OIDC\n  baseline scopes, not banking/data-access scopes — Alterna exposes no\n  first-party banking API and documents no data-sharing scopes.\nscheme: umbraco_member_oidc\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token identifying the authenticated site member.\n- name: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens without re-authenticating the member.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterna-savings/refs/heads/main/scopes/alterna-savings-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Cooperative
- Consumer-Driven Banking
- Interac
- Data Aggregation
token_urls: []
---
