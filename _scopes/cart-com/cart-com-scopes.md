---
api_specs:
- filename: cart-com-online-store-openapi-original.yml
  format: yaml
  label: Cart.com Online Store API
  slug: online-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cart-com/refs/heads/main/openapi/cart-com-online-store-openapi-original.yml
authorization_urls:
- https://[mystorename.com]/api/oauth
description: ''
docs: https://developers.cart.com/docs/rest-api/3e66e3e0c67ec-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cart Com Scopes
name_suffix: OAuth Scopes
note: 'The published OpenAPI declares only the apiKey scheme X-AC-Auth-Token and carries no oauth2 securityScheme, so no scopes are derivable from the spec. The scope model below is captured verbatim from the provider''s Scopes and Authentication guides. Scopes are coarse-grained and paired read/write: naming a write scope supersedes its read sibling. An access token can only use the scopes requested when it was created — changing scope requires a new token. The authorizing admin-console user must also hold the matching role-based permission.'
overview: 'Cart.com publishes 17 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cart.com API on a user''s behalf.


  Tokens are issued from https://[mystorename.com]/api/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cart.com
provider_slug: cart-com
schemes:
- flows:
  - authorizationUrl: https://[mystorename.com]/api/oauth
    flow: authorizationCode
    note: Non-standard OAuth 2 variant — the token exchange is authenticated with a SHA256 signature over secret + code + client_id + scope + redirect_uri rather than a client_secret POST parameter. Tokens are returned as access_token + refresh_token and presented on the API as the X-AC-Auth-Token header, not as a Bearer token.
    refreshUrl: https://[mystorename.com]/api/oauth/refresh_token
    tokenUrl: https://[mystorename.com]/api/oauth/access_token
  name: OAuth2
  source: https://developers.cart.com/docs/rest-api/ZG9jOjU4NjM4-cart-com-online-store-api-authentication
  type: oauth2
scope_count: 17
scope_names:
- read_people
- people
- read_orders
- orders
- read_catalog
- catalog
- read_content
- content
- read_marketing
- marketing
- email
- custom_fields
- import
- settings
- system
- decrypt
- no_expiry
scopes:
- description: View customer, user, or profile data.
  flows: []
  scope: read_people
- description: View and change customer, user, or profile data; supersedes read_people if specified together.
  flows: []
  scope: people
- description: View order data.
  flows: []
  scope: read_orders
- description: View and change order data; supersedes read_orders if specified together.
  flows: []
  scope: orders
- description: View catalog data.
  flows: []
  scope: read_catalog
- description: View and change catalog data; supersedes read_catalog if specified together.
  flows: []
  scope: catalog
- description: View blog, page, and other content-related data.
  flows: []
  scope: read_content
- description: View and change blog, page, and other content-related data; supersedes read_content if specified together.
  flows: []
  scope: content
- description: View adcode, discount, and other marketing-related data.
  flows: []
  scope: read_marketing
- description: View and change adcode, discount, and other marketing-related data; supersedes read_marketing if specified together.
  flows: []
  scope: marketing
- description: Send email templates.
  flows: []
  scope: email
- description: Read and write custom field definitions and values.
  flows: []
  scope: custom_fields
- description: Use the data import resource.
  flows: []
  scope: import
- description: Read and write store settings — shipping, warehouses, tax, regions, payment gateways, redirects.
  flows: []
  scope: settings
- description: Perform system tasks — stores, microstores, sessions, file upload. Also required to manage webhook subscriptions.
  flows: []
  scope: system
- description: Allows sensitive information to be decrypted. The authorizing user must have access to view this information. Tokens with this scope must be regenerated every 90 days if combined with no_expiry.
  flows: []
  scope: decrypt
- description: Token does not expire and does not require a refresh_token.
  flows: []
  scope: no_expiry
slug: cart-com-scopes
source_filename: cart-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://developers.cart.com/docs/rest-api/3e66e3e0c67ec-scopes\ndocs: https://developers.cart.com/docs/rest-api/3e66e3e0c67ec-scopes\nnote: 'The published OpenAPI declares only the apiKey scheme X-AC-Auth-Token and carries\n  no oauth2 securityScheme, so no scopes are derivable from the spec. The scope model\n  below is captured verbatim from the provider''s Scopes and Authentication guides.\n  Scopes are coarse-grained and paired read/write: naming a write scope supersedes\n  its read sibling. An access token can only use the scopes requested when it was created\n  — changing scope requires a new token. The authorizing admin-console user must also\n  hold the matching role-based permission.'\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: https://developers.cart.com/docs/rest-api/ZG9jOjU4NjM4-cart-com-online-store-api-authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://[mystorename.com]/api/oauth\n\
  \    tokenUrl: https://[mystorename.com]/api/oauth/access_token\n    refreshUrl: https://[mystorename.com]/api/oauth/refresh_token\n    note: 'Non-standard OAuth 2 variant — the token exchange is authenticated with\n      a SHA256 signature over secret + code + client_id + scope + redirect_uri rather\n      than a client_secret POST parameter. Tokens are returned as access_token + refresh_token\n      and presented on the API as the X-AC-Auth-Token header, not as a Bearer token.'\nscopes:\n- scope: read_people\n  description: View customer, user, or profile data.\n  group: People\n  access: read\n  admin_permissions: [Customers, CustomerTypes, UserAccounts, StoreSettings]\n  applies_to: [addresses, customers, customer_association, customer_types, customer_payment_methods,\n    profiles, users]\n- scope: people\n  description: View and change customer, user, or profile data; supersedes read_people\n    if specified together.\n  group: People\n  access: write\n  admin_permissions: [Customers,\
  \ CustomerTypes, UserAccounts, StoreSettings]\n  applies_to: [addresses, customers, customer_association, customer_types, customer_payment_methods,\n    profiles, users]\n- scope: read_orders\n  description: View order data.\n  group: Orders\n  access: read\n  admin_permissions: [Orders, OrderStatuses]\n  applies_to: [carts, cart_items, credit_cards, orders, order_addresses, order_items,\n    order_payments, order_shipments, order_statuses, quotes, subscriptions]\n- scope: orders\n  description: View and change order data; supersedes read_orders if specified together.\n  group: Orders\n  access: write\n  admin_permissions: [Orders, OrderStatuses]\n  applies_to: [carts, cart_items, credit_cards, orders, order_addresses, order_items,\n    order_payments, order_shipments, order_statuses, quotes, subscriptions]\n- scope: read_catalog\n  description: View catalog data.\n  group: Catalog\n  access: read\n  admin_permissions: [Products, ProductStatuses, VariationGroups, ProductAttributes,\n \
  \   Categories, Manufacturers]\n  applies_to: [attributes, attribute_groups, categories, manufacturers, products, product_inactive_in_store,\n    product_lists, product_pictures, product_statuses, product_variants, shipping_rate_adjustments,\n    variant_groups, variant_inventory]\n- scope: catalog\n  description: View and change catalog data; supersedes read_catalog if specified together.\n  group: Catalog\n  access: write\n  admin_permissions: [Products, ProductStatuses, VariationGroups, ProductAttributes,\n    Categories, Manufacturers]\n  applies_to: [attributes, attribute_groups, categories, manufacturers, products, product_inactive_in_store,\n    product_lists, product_pictures, product_statuses, product_variants, shipping_rate_adjustments,\n    variant_groups, variant_inventory]\n- scope: read_content\n  description: View blog, page, and other content-related data.\n  group: Content\n  access: read\n  admin_permissions: [Blogs, BlogCategories, BlogPosts, ContentManagement, UrlRedirecting]\n\
  \  applies_to: [blogs, blog_categories, blog_posts, links, pages]\n- scope: content\n  description: View and change blog, page, and other content-related data; supersedes\n    read_content if specified together.\n  group: Content\n  access: write\n  admin_permissions: [Blogs, BlogCategories, BlogPosts, ContentManagement, UrlRedirecting]\n  applies_to: [blogs, blog_categories, blog_posts, links, pages]\n- scope: read_marketing\n  description: View adcode, discount, and other marketing-related data.\n  group: Marketing\n  access: read\n  admin_permissions: [AdCodes, EmailEditor, MailingList, DiscountMethods, GiftCertificates]\n  applies_to: [adcodes, coupon_codes, discount_actions, discount_methods, discount_rules,\n    drips, email_templates, gift_certificates, gift_certificate_transactions, mailing_lists]\n- scope: marketing\n  description: View and change adcode, discount, and other marketing-related data;\n    supersedes read_marketing if specified together.\n  group: Marketing\n  access:\
  \ write\n  admin_permissions: [AdCodes, EmailEditor, MailingList, DiscountMethods, GiftCertificates]\n  applies_to: [adcodes, coupon_codes, discount_actions, discount_methods, discount_rules,\n    drips, email_templates, gift_certificates, gift_certificate_transactions, mailing_lists]\n- scope: email\n  description: Send email templates.\n  group: Specialized\n  admin_permissions: [EmailEditor]\n  applies_to: ['POST /api/v1/email_templates/{id}/send']\n- scope: custom_fields\n  description: Read and write custom field definitions and values.\n  group: Specialized\n  admin_permissions: [CustomFields]\n  applies_to: [custom_fields, custom_field_values]\n- scope: import\n  description: Use the data import resource.\n  group: Specialized\n  admin_permissions: [DataImport]\n  applies_to: [import]\n- scope: settings\n  description: Read and write store settings — shipping, warehouses, tax, regions,\n    payment gateways, redirects.\n  group: Specialized\n  admin_permissions: [Shipping, Warehouses,\
  \ TaxRates, GlobalRegions, PaymentGateways,\n    UrlRedirecting]\n  applies_to: [blacklisted_ips, custom_shipping_methods, external_image_whitelist,\n    payment_methods, regions, shipping_providers, shipping_provider_services, store_locations,\n    tax_rates, url_redirects, warehouses]\n- scope: system\n  description: Perform system tasks — stores, microstores, sessions, file upload. Also\n    required to manage webhook subscriptions.\n  group: Specialized\n  admin_permissions: [FileBrowser, Sessions, StoreSettings]\n  applies_to: [microstores, stores, sessions, 'POST /api/v1/upload']\n- scope: decrypt\n  description: Allows sensitive information to be decrypted. The authorizing user must\n    have access to view this information. Tokens with this scope must be regenerated\n    every 90 days if combined with no_expiry.\n  group: Sensitive\n  applies_to: ['GET /api/v1/credit_cards/{id}/decrypted', 'GET /api/v1/order_payments/{id}/decrypted']\n- scope: no_expiry\n  description: Token does\
  \ not expire and does not require a refresh_token.\n  group: Sensitive\nx-evidence:\n  fetched: '2026-07-31'\n  urls:\n  - https://developers.cart.com/docs/rest-api/3e66e3e0c67ec-scopes\n  - https://developers.cart.com/docs/rest-api/ZG9jOjU4NjM4-cart-com-online-store-api-authentication\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cart-com/refs/heads/main/scopes/cart-com-scopes.yml
summary_line: 17 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Order Management
- Fulfillment
- Logistics
- Marketplaces
- Storefront
- Catalog
- Shipping
token_urls:
- https://[mystorename.com]/api/oauth/access_token
---
