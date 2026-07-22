---
api_specs:
- filename: mirakl-mmp-seller-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Seller API
  slug: mirakl-marketplace-platform-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-seller-openapi.json
- filename: mirakl-mmp-operator-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Operator API
  slug: mirakl-marketplace-platform-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-operator-openapi.json
- filename: mirakl-mms-seller-openapi.json
  format: json
  label: Mirakl Platform for Services — Seller API
  slug: mirakl-platform-for-services-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-seller-openapi.json
- filename: mirakl-mms-operator-openapi.json
  format: json
  label: Mirakl Platform for Services — Operator API
  slug: mirakl-platform-for-services-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-operator-openapi.json
- filename: mirakl-mcm-seller-openapi.json
  format: json
  label: Mirakl Catalog Manager — Seller API
  slug: mirakl-catalog-manager-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-seller-openapi.json
- filename: mirakl-mcm-operator-openapi.json
  format: json
  label: Mirakl Catalog Manager — Operator API
  slug: mirakl-catalog-manager-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-operator-openapi.json
- filename: mirakl-connect-channel-openapi.json
  format: json
  label: Mirakl Connect Channel Platform API
  slug: mirakl-connect-channel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-connect-channel-openapi.json
authorization_urls:
- https://auth.mirakl.net/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Mirakl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mirakl uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.mirakl.net/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mirakl
provider_slug: mirakl
schemes:
- description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)
  flows:
  - authorizationUrl: https://auth.mirakl.net/authorize
    flow: authorizationCode
    tokenUrl: https://auth.mirakl.net/oauth/token
  name: OAuth-2
  source: openapi/mirakl-mcm-operator-openapi.json
- description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)
  flows:
  - authorizationUrl: https://auth.mirakl.net/authorize
    flow: authorizationCode
    tokenUrl: https://auth.mirakl.net/oauth/token
  name: OAuth-2
  source: openapi/mirakl-mmp-operator-openapi.json
- description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)
  flows:
  - authorizationUrl: https://auth.mirakl.net/authorize
    flow: authorizationCode
    tokenUrl: https://auth.mirakl.net/oauth/token
  name: OAuth-2
  source: openapi/mirakl-mms-operator-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: mirakl-scopes
source_filename: mirakl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mirakl-mcm-operator-openapi.json, openapi/mirakl-mmp-operator-openapi.json,\n  openapi/mirakl-mms-operator-openapi.json\nschemes:\n- name: OAuth-2\n  source: openapi/mirakl-mcm-operator-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mirakl.net/authorize\n    tokenUrl: https://auth.mirakl.net/oauth/token\n  description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)\n- name: OAuth-2\n  source: openapi/mirakl-mmp-operator-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mirakl.net/authorize\n    tokenUrl: https://auth.mirakl.net/oauth/token\n  description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)\n\
  - name: OAuth-2\n  source: openapi/mirakl-mms-operator-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mirakl.net/authorize\n    tokenUrl: https://auth.mirakl.net/oauth/token\n  description: For more information, see our [Authentication System documentation](https://help.mirakl.com/docs/customers/page/topics/Mirakl/partners_integration/authentication_system.htm)\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/scopes/mirakl-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Commerce
- eCommerce
- Marketplace
- Dropship
- Retail
- Catalog
- Orders
- Retail Media
- B2B
token_urls:
- https://auth.mirakl.net/oauth/token
---
