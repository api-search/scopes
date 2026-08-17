---
api_specs:
- filename: yoast-pages-api-openapi.yml
  format: yaml
  label: Yoast Pages API
  slug: yoast-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-pages-api-openapi.yml
- filename: yoast-posts-api-openapi.yml
  format: yaml
  label: Yoast Posts API
  slug: yoast-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-posts-api-openapi.yml
- filename: yoast-seo-head-api-openapi.yml
  format: yaml
  label: Yoast SEO Head API
  slug: yoast-seo-head-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-seo-head-api-openapi.yml
- filename: yoast-abilities-api-openapi.yml
  format: yaml
  label: Yoast SEO Abilities API
  slug: yoast-abilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-abilities-api-openapi.yml
- filename: yoast-schema-aggregator-openapi.yml
  format: yaml
  label: Yoast Schema Aggregator API
  slug: yoast-schema-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-schema-aggregator-openapi.yml
- filename: yoast-myyoast-provisioning-openapi.yml
  format: yaml
  label: MyYoast Provisioning API
  slug: myyoast-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-myyoast-provisioning-openapi.yml
authorization_urls:
- https://my.yoast.com/api/oauth/auth
description: ''
docs: https://developer.yoast.com/features/wp-cli/auth/
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Yoast Scopes
name_suffix: OAuth Scopes
note: 'derive-oauth-scopes.py found no oauth2 securityScheme in any OpenAPI in this repo, and that is correct — the MyYoast Provisioning API is Basic Auth. The scopes below are NOT derived from a spec; they were read live from the MyYoast OpenID Connect discovery document at https://my.yoast.com/.well-known/openid-configuration (HTTP 200, application/json). They are the standard OIDC scope set: MyYoast issues identity tokens for the Yoast SEO plugin''s site/user authentication, and publishes no product-specific scopes (nothing like seo:read or subscriptions:write). An integrator cannot request granular Yoast permissions, because none are advertised.'
overview: 'Yoast uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://my.yoast.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yoast
provider_slug: yoast
schemes:
- flows:
  - authorizationUrl: https://my.yoast.com/api/oauth/auth
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://my.yoast.com/api/oauth/token
  - flow: clientCredentials
    tokenUrl: https://my.yoast.com/api/oauth/token
  - flow: refreshToken
    tokenUrl: https://my.yoast.com/api/oauth/token
  name: MyYoast OpenID Connect
  source: well-known/yoast-openid-configuration.json
  type: openIdConnect
scope_count: 0
scope_names: []
scopes: []
slug: yoast-scopes
source_filename: yoast-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://my.yoast.com/.well-known/openid-configuration\ndocs: https://developer.yoast.com/features/wp-cli/auth/\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme in any OpenAPI in this repo, and\n  that is correct — the MyYoast Provisioning API is Basic Auth. The scopes below are NOT\n  derived from a spec; they were read live from the MyYoast OpenID Connect discovery\n  document at https://my.yoast.com/.well-known/openid-configuration (HTTP 200,\n  application/json). They are the standard OIDC scope set: MyYoast issues identity\n  tokens for the Yoast SEO plugin's site/user authentication, and publishes no\n  product-specific scopes (nothing like seo:read or subscriptions:write). An integrator\n  cannot request granular Yoast permissions, because none are advertised.\nissuer: https://my.yoast.com\nschemes:\n  - name: MyYoast OpenID Connect\n    type: openIdConnect\n    source: well-known/yoast-openid-configuration.json\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://my.yoast.com/api/oauth/auth\n        tokenUrl: https://my.yoast.com/api/oauth/token\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://my.yoast.com/api/oauth/token\n      - flow: refreshToken\n        tokenUrl: https://my.yoast.com/api/oauth/token\nscopes:\n  - name: openid\n    description: Standard OIDC scope; requests an ID token identifying the subject.\n    standard: true\n  - name: profile\n    description: Standard OIDC scope; basic profile claims.\n    standard: true\n  - name: email\n    description: Standard OIDC scope; email claims.\n    standard: true\n  - name: phone\n    description: Standard OIDC scope; phone claims.\n    standard: true\n  - name: address\n    description: Standard OIDC scope; address claims.\n    standard: true\n  - name: offline_access\n    description: Standard OIDC scope; requests a refresh token for long-lived access.\n    standard: true\nclaims_supported:\n\
  \  - sub\n  - sid\n  - auth_time\n  - iss\nscope_count: 6\nproduct_specific_scope_count: 0\ngaps:\n  - >-\n    Every advertised scope is a standard OIDC scope. MyYoast publishes no\n    product-permission scopes, so an authorized client's actual authority over Yoast\n    resources is not expressible or inspectable through the scope model.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://my.yoast.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/scopes/yoast-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- SEO
- WordPress
- Content Optimization
- Schema
- Metadata
- Structured Data
- Headless CMS
- Content Analysis
- Agent Readiness
- Plugins
token_urls:
- https://my.yoast.com/api/oauth/token
---
