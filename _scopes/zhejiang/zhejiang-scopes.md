---
api_specs:
- filename: zhejiang-catalog-api-openapi.yml
  format: yaml
  label: Zhejiang University Catalog API
  slug: zhejiang-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zhejiang/refs/heads/main/openapi/zhejiang-catalog-api-openapi.yml
- filename: zhejiang-repositories-api-openapi.yml
  format: yaml
  label: Zhejiang University Repositories API
  slug: zhejiang-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zhejiang/refs/heads/main/openapi/zhejiang-repositories-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Zhejiang Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zhejiang University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zhejiang University
provider_slug: zhejiang
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zhejiang-scopes
source_filename: zhejiang-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "# Zhejiang University — authorization scopes\ngenerated: '2026-08-19'\nmethod: probed\nsource: Live probes 2026-08-19 of zju.edu.cn hosts.\nx-operator: institution\nscopes: []\nfinding: >-\n  No scope vocabulary exists on any institution-operated ZJU surface. The public\n  mirror service is unauthenticated and therefore has no scopes. The CAS SSO platform\n  and the Shibboleth IdP are federation surfaces, not OAuth authorization servers:\n  Shibboleth expresses release policy as SAML attribute release, not as scopes, and\n  the attribute-release policy is not published on the public metadata endpoint.\n  No OAuth 2.0 authorization server, discovery document, or scope list was found.\nprobes:\n  - url: https://idp.zju.edu.cn/idp/shibboleth\n    status: 200\n    detail: SAML metadata; no scope vocabulary. AttributeService advertised, policy not published.\n  - url: https://zjuam.zju.edu.cn/cas/login?locale=en\n    status: 200\n    detail: CAS interactive login; no scope model.\n\
  \  - url: https://mirrors.zju.edu.cn/mirrorz.json\n    status: 200\n    detail: Anonymous read; no authorization layer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhejiang/refs/heads/main/scopes/zhejiang-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Research
- China
- C9 League
- Double First-Class
- Identity Federation
- Single Sign-On
- Open Source Mirror
- Library
token_urls: []
---
