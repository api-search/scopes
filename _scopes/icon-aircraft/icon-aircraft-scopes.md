---
api_specs:
- filename: icon-aircraft-content-api-openapi.yml
  format: yaml
  label: ICON Aircraft Content API
  slug: icon-aircraft-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-content-api-openapi.yml
- filename: icon-aircraft-store-api-openapi.yml
  format: yaml
  label: Shop ICON Storefront API
  slug: icon-aircraft-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-store-api-openapi.yml
authorization_urls: []
description: ''
docs: https://store.iconaircraft.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Icon Aircraft Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ICON Aircraft uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ICON Aircraft
provider_slug: icon-aircraft
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: icon-aircraft-scopes
source_filename: icon-aircraft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: well-known/icon-aircraft-store-oauth-authorization-server.json\ndocs: https://store.iconaircraft.com/.well-known/oauth-authorization-server\nsummary: >-\n  ICON Aircraft publishes no OAuth scope reference of its own. The only OAuth surface on any of its\n  hosts is the Shopify customer-account authorization server advertised by the Shop ICON storefront\n  and named as the authorization server for the UCP/MCP endpoint. The four scopes below are read\n  verbatim from that server's own RFC 8414 metadata document, probed anonymously on 2026-08-22.\n  Nothing is inferred, and none of them grant access to ICON Aircraft's own data beyond a shopper's\n  own account. Neither OpenAPI in this repository declares an oauth2 securityScheme, because every\n  operation described in them answers without a token.\nauthorization_server: https://shopify.com/authentication/376732\nauthorization_endpoint: https://shopify.com/authentication/376732/oauth/authorize\n\
  token_endpoint: https://shopify.com/authentication/376732/oauth/token\nprotected_resources:\n- https://store.iconaircraft.com\n- https://store.iconaircraft.com/api/ucp/mcp\nflows:\n- authorization_code\n- refresh_token\n- urn:ietf:params:oauth:grant-type:jwt-bearer\npkce:\n- S256\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token for the signed-in shopper.\n  category: identity\n  grants_access_to_icon_data: false\n- name: email\n  description: Releases the shopper's email address as an OIDC claim.\n  category: identity\n  grants_access_to_icon_data: false\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the authenticated shopper — their own\n    orders, addresses and payment methods on the Shop ICON store.\n  category: buyer\n  grants_access_to_icon_data: false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify customer-account\
  \ MCP API for the authenticated shopper. This is the\n    scope an agent would present on buyer-scoped UCP tools such as get_order; tools/list and the\n    catalog tools do not require it.\n  category: buyer\n  grants_access_to_icon_data: false\nnotes:\n- >-\n  These are platform scopes defined by Shopify, exposed under ICON Aircraft's storefront domain and\n  bound to ICON's merchant id 376732. ICON did not author them and does not extend them.\n- >-\n  There is no scope, on any server, that grants a developer access to ICON Aircraft product,\n  aircraft, order or service data. The company operates no such API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/scopes/icon-aircraft-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Aerospace
- Aviation
- Aircraft Manufacturing
- Light Sport Aircraft
- Seaplanes
- General Aviation
- Flight Training
- Manufacturing
- Consumer Products
- E-Commerce
- Content
- Agentic Commerce
token_urls: []
---
