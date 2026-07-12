---
authorization_urls:
- https://www.wix.com/installer/install
description: ''
docs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wix Scopes
name_suffix: OAuth Scopes
note: Wix OAuth does not use scope strings in the authorization flow; app permissions are granted as permission scopes configured in the app dashboard (GUID-identified via the App Permissions API) and documented per endpoint in the API reference, with no aggregated published scopes list (see https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions).
overview: 'Wix uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://www.wixapis.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wix
provider_slug: wix
schemes:
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  source: openapi/wix-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: wix-scopes
source_filename: wix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wix-openapi.yml\ndocs: https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions\nnote: Wix OAuth does not use scope strings in the authorization flow; app permissions\n  are granted as permission scopes configured in the app dashboard (GUID-identified\n  via the App Permissions API) and documented per endpoint in the API reference,\n  with no aggregated published scopes list (see\n  https://dev.wix.com/docs/build-apps/develop-your-app/access/authorization/about-permissions).\nschemes:\n- name: oauth2\n  source: openapi/wix-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n  description: OAuth 2.0 for Wix third-party apps\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/scopes/wix-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CMS
- eCommerce
- Headless
- Website Builder
token_urls:
- https://www.wixapis.com/oauth2/token
---
