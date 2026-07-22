---
authorization_urls: []
description: 'Wix''s OAuth authorization surface uses named permission scopes rather than a single published scope registry. Apps declare the permission scopes they need in the app dashboard (https://dev.wix.com/apps/my-apps); site owners grant them at install time, and access tokens are minted with those permissions via the OAuth 2 client-credentials flow. The authoritative scope list is distributed across the API reference: every REST endpoint, SDK method, and webhook documents the permission scopes that grant access to it. Scopes are hierarchical: broad "manage" scopes contain narrower ones (App Market guidelines require requesting the minimum set — e.g. an app requesting "Manage Stores - All Permissions" must not also request "Manage Products", which it already contains). Wix publishes no OpenAPI, so no machine-derived scope enumeration is possible; this artifact captures the model and the published example scope names verbatim.'
docs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Wixcom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wix.com publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wix.com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wix.com
provider_slug: wixcom
schemes:
- flows:
  - flow: clientCredentials
    tokenOperation: https://dev.wix.com/docs/api-reference/app-management/oauth-2/create-access-token
  name: OAuth2ClientCredentials
scope_count: 2
scope_names:
- Manage Stores - All Permissions
- Manage Products
scopes:
- description: Full management of Wix Stores; contains narrower Stores permissions such as Manage Products (example quoted in the App Market guidelines).
  flows: []
  scope: Manage Stores - All Permissions
- description: Manage Wix Stores products (contained within Manage Stores - All Permissions).
  flows: []
  scope: Manage Products
slug: wixcom-scopes
source_filename: wixcom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions\nsource: https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions\ndescription: >-\n  Wix's OAuth authorization surface uses named permission scopes rather than\n  a single published scope registry. Apps declare the permission scopes they\n  need in the app dashboard (https://dev.wix.com/apps/my-apps); site owners\n  grant them at install time, and access tokens are minted with those\n  permissions via the OAuth 2 client-credentials flow. The authoritative\n  scope list is distributed across the API reference: every REST endpoint,\n  SDK method, and webhook documents the permission scopes that grant access\n  to it. Scopes are hierarchical: broad \"manage\" scopes contain narrower\n  ones (App Market guidelines require requesting the minimum set — e.g. an\n  app requesting \"Manage Stores - All Permissions\"\
  \ must not also request\n  \"Manage Products\", which it already contains). Wix publishes no OpenAPI,\n  so no machine-derived scope enumeration is possible; this artifact\n  captures the model and the published example scope names verbatim.\nschemes:\n  - name: OAuth2ClientCredentials\n    flows:\n      - flow: clientCredentials\n        tokenOperation: https://dev.wix.com/docs/api-reference/app-management/oauth-2/create-access-token\nscope_model:\n  granted_via: app dashboard permission configuration + site-owner consent at install\n  documented_per_operation: true\n  hierarchy: broad \"manage\" scopes include narrower read/manage scopes\n  configuration_docs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/configure-permissions-for-your-app\nscopes:\n  - scope: Manage Stores - All Permissions\n    description: >-\n      Full management of Wix Stores; contains narrower Stores permissions\n      such as Manage Products (example quoted in the App Market guidelines).\n\
  \  - scope: Manage Products\n    description: Manage Wix Stores products (contained within Manage Stores - All Permissions).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wixcom/refs/heads/main/scopes/wixcom-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Website Builder
- eCommerce
- CMS
- Bookings
- Payments
- Headless
- SaaS
- No Code
token_urls: []
---
