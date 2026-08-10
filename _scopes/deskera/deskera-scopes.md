---
authorization_urls:
- https://oauth.deskera.com/
description: ''
docs: https://deskera.github.io/Developer-Documentation/docs/books/oauthv2
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Deskera Scopes
name_suffix: OAuth Scopes
note: Deskera publishes no OpenAPI document, so these scopes are read from the provider's own OAuth documentation and from the per-operation Security tables in the developer docs — not derived from securitySchemes. Deskera does not publish a granular scopes/permissions reference page; the OAuth surface is coarse-grained.
overview: 'Deskera publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deskera API on a user''s behalf.


  Tokens are issued from https://bifrost-us.deskera.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deskera
provider_slug: deskera
schemes:
- flows:
  - authorizationUrl: https://oauth.deskera.com/
    flow: authorizationCode
    tokenUrl: https://bifrost-us.deskera.com/oauth/token
  name: Authorization
  type: oauth2
scope_count: 3
scope_names:
- write
- read
- global
scopes:
- description: Write access requested on the OAuth authorization link (?client_id=...&scope=write&response_type=code). The scope used in every authorization-link example Deskera publishes.
  flows:
  - authorizationCode
  scope: write
- description: Read access. Documented in combination with write on the token exchange (grant_type=authorization_code&scope=read+write).
  flows:
  - authorizationCode
  scope: read
- description: The scope value carried on the per-operation "Security" tables in the generated API reference (Security Schema "Authorization", Scopes "global") — recorded on 3,739 documented operations. Deskera does not decompose this into per-resource scopes.
  flows:
  - authorizationCode
  scope: global
slug: deskera-scopes
source_filename: deskera-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\ndocs: https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\nnote: >-\n  Deskera publishes no OpenAPI document, so these scopes are read from the\n  provider's own OAuth documentation and from the per-operation Security tables in\n  the developer docs — not derived from securitySchemes. Deskera does not publish a\n  granular scopes/permissions reference page; the OAuth surface is coarse-grained.\nschemes:\n- name: Authorization\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.deskera.com/\n    tokenUrl: https://bifrost-us.deskera.com/oauth/token\nscopes:\n- scope: write\n  description: >-\n    Write access requested on the OAuth authorization link\n    (?client_id=...&scope=write&response_type=code). The scope used in every\n    authorization-link example Deskera publishes.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - https://deskera.github.io/Developer-Documentation/docs/books/oauthv2\n- scope: read\n  description: >-\n    Read access. Documented in combination with write on the token exchange\n    (grant_type=authorization_code&scope=read+write).\n  flows:\n  - authorizationCode\n  sources:\n  - https://deskera.github.io/Developer-Documentation/docs/environment/prod\n- scope: global\n  description: >-\n    The scope value carried on the per-operation \"Security\" tables in the generated\n    API reference (Security Schema \"Authorization\", Scopes \"global\") — recorded on\n    3,739 documented operations. Deskera does not decompose this into per-resource\n    scopes.\n  flows:\n  - authorizationCode\n  sources:\n  - https://deskera.github.io/Developer-Documentation/docs/books/invoiceapi\n  - https://deskera.github.io/Developer-Documentation/docs/sales/contactsapi\ngaps:\n- No published scopes/permissions reference page.\n- No per-resource or per-verb scopes; authorization is effectively\
  \ account-wide\n  read/write plus a \"global\" operation scope.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://raw.githubusercontent.com/Deskera/Developer-Documentation/master/docs/books/oauthv2.md\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deskera/refs/heads/main/scopes/deskera-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- ERP
- Accounting
- CRM
- Human Resources
- Payroll
- Inventory
- Invoicing
- Small Business
- SaaS
token_urls:
- https://bifrost-us.deskera.com/oauth/token
---
