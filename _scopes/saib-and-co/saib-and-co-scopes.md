---
authorization_urls:
- https://saibnco.cafe24api.com/api/v2/oauth/authorize
description: ''
docs: https://developers.cafe24.com/app/front/app/develop/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Saib And Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAIB & Co. publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAIB & Co. API on a user''s behalf.


  Tokens are issued from https://saibnco.cafe24api.com/api/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAIB & Co.
provider_slug: saib-and-co
schemes:
- flows:
  - authorizationUrl: https://saibnco.cafe24api.com/api/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://saibnco.cafe24api.com/api/v2/oauth/token
  name: cafe24StorefrontOAuth
  source: well-known/saib-and-co-openid-configuration.json
scope_count: 6
scope_names:
- openid
- dev.ucp.shopping.checkout:manage
- dev.ucp.shopping.cart:manage
- dev.ucp.shopping.order:read
- dev.ucp.shopping.catalog.search:read
- dev.ucp.shopping.catalog.lookup:read
scopes:
- description: OpenID Connect authentication; return an ID token for the shopper.
  flows:
  - authorizationCode
  scope: openid
- description: Manage the storefront checkout for the shopper.
  flows:
  - authorizationCode
  scope: dev.ucp.shopping.checkout:manage
- description: Manage the shopper's shopping cart.
  flows:
  - authorizationCode
  scope: dev.ucp.shopping.cart:manage
- description: Read the shopper's orders.
  flows:
  - authorizationCode
  scope: dev.ucp.shopping.order:read
- description: Search the storefront product catalog.
  flows:
  - authorizationCode
  scope: dev.ucp.shopping.catalog.search:read
- description: Look up individual products in the storefront catalog.
  flows:
  - authorizationCode
  scope: dev.ucp.shopping.catalog.lookup:read
slug: saib-and-co-scopes
source_filename: saib-and-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://saibnco.com/.well-known/openid-configuration\ndocs: https://developers.cafe24.com/app/front/app/develop/oauth\nnotes: >-\n  OAuth scopes advertised by the SAIB & Co. Cafe24 storefront (UCP) OpenID\n  Connect discovery document (scopes_supported). These are Cafe24 Unified\n  Commerce Platform storefront scopes exposed for this mall.\nschemes:\n- name: cafe24StorefrontOAuth\n  source: well-known/saib-and-co-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://saibnco.cafe24api.com/api/v2/oauth/authorize\n    tokenUrl: https://saibnco.cafe24api.com/api/v2/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; return an ID token for the shopper.\n  flows: [authorizationCode]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n- scope: dev.ucp.shopping.checkout:manage\n  description: Manage the storefront checkout for the shopper.\n  flows:\
  \ [authorizationCode]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n- scope: dev.ucp.shopping.cart:manage\n  description: Manage the shopper's shopping cart.\n  flows: [authorizationCode]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n- scope: dev.ucp.shopping.order:read\n  description: Read the shopper's orders.\n  flows: [authorizationCode]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n- scope: dev.ucp.shopping.catalog.search:read\n  description: Search the storefront product catalog.\n  flows: [authorizationCode]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n- scope: dev.ucp.shopping.catalog.lookup:read\n  description: Look up individual products in the storefront catalog.\n  flows: [authorizationCode]\n  sources: [well-known/saib-and-co-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saib-and-co/refs/heads/main/scopes/saib-and-co-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Cosmetics
- Consumer Goods
- E-Commerce
- Wellness
- Retail
- Cafe24
- OAuth
token_urls:
- https://saibnco.cafe24api.com/api/v2/oauth/token
---
