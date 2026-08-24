---
authorization_urls: []
description: Scopes advertised by the authorization-server metadata the Hodinkee commerce host serves. Hodinkee publishes no scopes reference page of its own; these are read verbatim from the live discovery document, which lists them under `scopes_supported`. Descriptions below are the plain reading of each scope name and are marked as such — they are not quoted from provider documentation.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hodinkee Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hodinkee uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hodinkee
provider_slug: hodinkee
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hodinkee-scopes
source_filename: hodinkee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://shop.hodinkee.com/.well-known/openid-configuration\nname: HODINKEE Shop OAuth scopes\ndescription: >-\n  Scopes advertised by the authorization-server metadata the Hodinkee commerce\n  host serves. Hodinkee publishes no scopes reference page of its own; these are\n  read verbatim from the live discovery document, which lists them under\n  `scopes_supported`. Descriptions below are the plain reading of each scope\n  name and are marked as such — they are not quoted from provider documentation.\nauthorization_server: https://shopify.com/authentication/1460732\nshop_id: '1460732'\nscope_count: 4\nscopes:\n- name: openid\n  standard: OpenID Connect Core\n  description: Request an ID token for the authenticated customer.\n  description_source: derived-from-standard\n- name: email\n  standard: OpenID Connect Core\n  description: Release the customer's email address and email_verified claim.\n  description_source: derived-from-standard\n\
  - name: customer-account-api:full\n  standard: Shopify Customer Account API\n  description: Full customer-scoped access to the account API (orders, addresses, profile).\n  description_source: derived-from-scope-name\n- name: customer-account-mcp-api:full\n  standard: Shopify Customer Account MCP API\n  description: >-\n    Full customer-scoped access to the MCP API. This is the scope that gates the\n    authenticated agent surface; the anonymous UCP and storefront MCP endpoints\n    do not require it.\n  description_source: derived-from-scope-name\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\ndocs: null\ndocs_note: >-\n  No provider-published scopes/permissions reference exists on any hodinkee.com\n  host. Recorded as absent rather than substituted with Shopify platform docs.\nchecked: '2026-08-22'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hodinkee/refs/heads/main/scopes/hodinkee-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Watches
- Luxury Goods
- E-Commerce
- Media
- Publishing
- Retail
- Agentic Commerce
- Model Context Protocol
- Shopify
token_urls: []
---
