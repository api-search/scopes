---
api_specs:
- filename: zalando-orders-openapi.yml
  format: yaml
  label: zDirect Platform Orders API
  slug: zalando-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-orders-openapi.yml
- filename: zalando-products-openapi.yml
  format: yaml
  label: zDirect Platform Products API
  slug: zalando-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-products-openapi.yml
- filename: zalando-product-attributes-openapi.yml
  format: yaml
  label: Merchant Product Attributes API
  slug: zalando-product-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-product-attributes-openapi.yml
- filename: zalando-article-requirements-openapi.yml
  format: yaml
  label: Article Requirements API
  slug: zalando-article-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-article-requirements-openapi.yml
- filename: zalando-prices-openapi.yml
  format: yaml
  label: Merchant Price Service API
  slug: zalando-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-prices-openapi.yml
- filename: zalando-price-reporting-openapi.yml
  format: yaml
  label: Price Reporting API
  slug: zalando-price-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-price-reporting-openapi.yml
- filename: zalando-stocks-openapi.yml
  format: yaml
  label: Merchant Stock Service API
  slug: zalando-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-stocks-openapi.yml
- filename: zalando-offer-blocking-openapi.yml
  format: yaml
  label: Article Availability (Offer Blocking) API
  slug: zalando-offer-blocking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-offer-blocking-openapi.yml
- filename: zalando-sales-channels-openapi.yml
  format: yaml
  label: Sales Channels API
  slug: zalando-sales-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-sales-channels-openapi.yml
- filename: zalando-logistic-centers-openapi.yml
  format: yaml
  label: Logistic Centers API
  slug: zalando-logistic-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-logistic-centers-openapi.yml
- filename: zalando-zfs-stock-movements-openapi.yml
  format: yaml
  label: ZFS Stock Movements API
  slug: zalando-zfs-stock-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-stock-movements-openapi.yml
- filename: zalando-zfs-cross-border-movements-openapi.yml
  format: yaml
  label: ZFS Cross-Border Movements Report API
  slug: zalando-zfs-cross-border-movements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/openapi/zalando-zfs-cross-border-movements-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Zalando Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zalando publishes 16 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zalando API on a user''s behalf.


  Tokens are issued from https://api.merchants.zalando.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zalando
provider_slug: zalando
schemes:
- description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth 2 to handle the client credentials process flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-logistic-centers-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-offer-blocking-openapi.yml
- description: This API uses OAuth2 OIDC with Client Credentials flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-orders-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-price-reporting-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-prices-openapi.yml
- description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth 2 to handle the client credentials process flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-product-attributes-openapi.yml
- description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth 2 to handle the client credentials process flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-products-openapi.yml
- description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth 2 to handle the client credentials process flow.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-sales-channels-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-stocks-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token
  name: OAuth2
  source: openapi/zalando-zfs-cross-border-movements-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token
  name: merchant_platform
  source: openapi/zalando-zfs-stock-movements-openapi.yml
scope_count: 16
scope_names:
- orders/read
- orders/write
- products/attributes/read
- products/blockers/read
- products/blockers/write
- products/price/read
- products/price/write
- products/read
- products/stock/write
- products/write
- profile/logistic-centers/read
- profile/sales-channels/read
- zfs.icm-reports.read
- zfs/liquidated-item/read
- zfs/received-item/read
- zfs/returned-item/read
scopes:
- description: Read access.
  flows:
  - clientCredentials
  scope: orders/read
- description: Write access.
  flows:
  - clientCredentials
  scope: orders/write
- description: scope to read a product
  flows:
  - clientCredentials
  scope: products/attributes/read
- description: Grant read access for Offer Blockers to external Merchants.
  flows:
  - clientCredentials
  scope: products/blockers/read
- description: Grant write access for Offer Blockers to external Merchants.
  flows:
  - clientCredentials
  scope: products/blockers/write
- description: Grant read access for product prices to external Merchants.
  flows:
  - clientCredentials
  scope: products/price/read
- description: Grant write access to product prices.
  flows:
  - clientCredentials
  scope: products/price/write
- description: scope to read a product
  flows:
  - clientCredentials
  scope: products/read
- description: Grant write access for stocks to external Merchants.
  flows:
  - clientCredentials
  scope: products/stock/write
- description: scope to create or update a product
  flows:
  - clientCredentials
  scope: products/write
- description: scope to get logistic centers
  flows:
  - clientCredentials
  scope: profile/logistic-centers/read
- description: scope to get sales channels
  flows:
  - clientCredentials
  scope: profile/sales-channels/read
- description: Access to ZFS ICM and Cross-border Reports of a merchant.
  flows:
  - clientCredentials
  scope: zfs.icm-reports.read
- description: ''
  flows: []
  scope: zfs/liquidated-item/read
- description: Access to ZFS received items of a merchant.
  flows:
  - clientCredentials
  scope: zfs/received-item/read
- description: Access to ZFS returned items of a merchant.
  flows:
  - clientCredentials
  scope: zfs/returned-item/read
slug: zalando-scopes
source_filename: zalando-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zalando-logistic-centers-openapi.yml, openapi/zalando-offer-blocking-openapi.yml,\n  openapi/zalando-orders-openapi.yml, openapi/zalando-price-reporting-openapi.yml, openapi/zalando-prices-openapi.yml,\n  openapi/zalando-product-attributes-openapi.yml, openapi/zalando-products-openapi.yml, openapi/zalando-sales-channels-openapi.yml,\n  openapi/zalando-stocks-openapi.yml, openapi/zalando-zfs-cross-border-movements-openapi.yml,\n  openapi/zalando-zfs-stock-movements-openapi.yml\nschemes:\n- name: merchant_platform\n  source: openapi/zalando-logistic-centers-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.merchants.zalando.com/auth/token\n  description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth\n    2 to handle the client credentials process flow.\n- name: merchant_platform\n  source: openapi/zalando-offer-blocking-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://api.merchants.zalando.com/auth/token\n- name: merchant_platform\n  source: openapi/zalando-orders-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token\n  description: This API uses OAuth2 OIDC with Client Credentials flow.\n- name: merchant_platform\n  source: openapi/zalando-price-reporting-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.merchants.zalando.com/auth/token\n- name: merchant_platform\n  source: openapi/zalando-prices-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.merchants.zalando.com/auth/token\n- name: merchant_platform\n  source: openapi/zalando-product-attributes-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token\n  description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth\n    2 to handle the client credentials process\
  \ flow.\n- name: merchant_platform\n  source: openapi/zalando-products-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token\n  description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth\n    2 to handle the client credentials process flow.\n- name: merchant_platform\n  source: openapi/zalando-sales-channels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.merchants.zalando.com/auth/token\n  description: The Products service uses the OpenID Connect (OIDC) authentication layer of OAuth\n    2 to handle the client credentials process flow.\n- name: merchant_platform\n  source: openapi/zalando-stocks-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.merchants.zalando.com/auth/token\n- name: OAuth2\n  source: openapi/zalando-zfs-cross-border-movements-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token\n\
  - name: merchant_platform\n  source: openapi/zalando-zfs-stock-movements-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-sandbox.merchants.zalando.com/auth/token\nscopes:\n- scope: orders/read\n  description: Read access.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-orders-openapi.yml\n- scope: orders/write\n  description: Write access.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-orders-openapi.yml\n- scope: products/attributes/read\n  description: scope to read a product\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-product-attributes-openapi.yml\n- scope: products/blockers/read\n  description: Grant read access for Offer Blockers to external Merchants.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-offer-blocking-openapi.yml\n- scope: products/blockers/write\n  description: Grant write access for Offer Blockers to external Merchants.\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/zalando-offer-blocking-openapi.yml\n- scope: products/price/read\n  description: Grant read access for product prices to external Merchants.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-price-reporting-openapi.yml\n- scope: products/price/write\n  description: Grant write access to product prices.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-prices-openapi.yml\n- scope: products/read\n  description: scope to read a product\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-products-openapi.yml\n- scope: products/stock/write\n  description: Grant write access for stocks to external Merchants.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-stocks-openapi.yml\n- scope: products/write\n  description: scope to create or update a product\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-products-openapi.yml\n- scope: profile/logistic-centers/read\n  description: scope to get logistic centers\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-logistic-centers-openapi.yml\n- scope: profile/sales-channels/read\n  description: scope to get sales channels\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-sales-channels-openapi.yml\n- scope: zfs.icm-reports.read\n  description: Access to ZFS ICM and Cross-border Reports of a merchant.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-zfs-cross-border-movements-openapi.yml\n- scope: zfs/liquidated-item/read\n  sources:\n  - openapi/zalando-zfs-stock-movements-openapi.yml\n- scope: zfs/received-item/read\n  description: Access to ZFS received items of a merchant.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-zfs-stock-movements-openapi.yml\n- scope: zfs/returned-item/read\n  description: Access to ZFS returned items of a merchant.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/zalando-zfs-stock-movements-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zalando/refs/heads/main/scopes/zalando-scopes.yml
summary_line: 16 scopes · clientCredentials
tags:
- Company
- Consumer; Marketplace
- Fashion
- E-Commerce
- Retail
- Marketplace
- Fulfillment
- Merchant Platform
- Orders
- Products
token_urls:
- https://api.merchants.zalando.com/auth/token
- https://api-sandbox.merchants.zalando.com/auth/token
---
