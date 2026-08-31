---
authorization_urls: []
description: ''
docs:
- https://developer.fxiaoke.com/openapi_v2/start/auth/auth-code.html
- https://developer.fxiaoke.com/openapi_v2/start/guide/codes.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fxiaoke Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fxiaoke uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fxiaoke
provider_slug: fxiaoke
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fxiaoke-scopes
source_filename: fxiaoke-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://open.fxiaoke.com/.well-known/oauth-authorization-server\ndocs:\n- https://developer.fxiaoke.com/openapi_v2/start/auth/auth-code.html\n- https://developer.fxiaoke.com/openapi_v2/start/guide/codes.html\nscope_count: 0\npublished: false\nsummary: >-\n  Fxiaoke documents OAuth but publishes NO scope registry. This file records that\n  measured absence; no OAuthScopes pointer is emitted in apis.yml, because a pointer\n  would assert the provider publishes a scope catalog it does not.\n\nevidence:\n- source: https://open.fxiaoke.com/.well-known/oauth-authorization-server\n  http_status: 200\n  finding: >-\n    The RFC 8414 metadata document omits scopes_supported entirely. It advertises\n    grant_types, response_types, code_challenge_methods, token_endpoint_auth_methods,\n    subject_types and id_token_signing_alg_values — but no scopes.\n- source: https://developer.fxiaoke.com/openapi_v2/start/auth/auth-code.html\n  http_status:\
  \ 200\n  finding: >-\n    The documented authorization-code flow's parameter table lists appId, redirectUrl,\n    responseType, state and thirdTraceId. There is no scope parameter in the documented\n    request, and no consent-screen description.\n- source: https://developer.fxiaoke.com/openapi_v2/start/guide/codes.html\n  http_status: 200\n  finding: >-\n    A scope parameter demonstrably exists somewhere in the platform — the global return\n    code table defines 10006 \"缺少参数scope\" (missing parameter scope) and 11006\n    \"参数scope不合法\" (invalid parameter scope) — but no valid values are published\n    anywhere on the public surface.\n\nauthorization_model:\n  actual: admin-granted per-app permissions\n  description: >-\n    In practice authorization is not scope-based from the developer's side. A tenant\n    administrator creates a self-built application and grants it access to enterprise\n    data, employees and departments through the Fxiaoke admin console. The application\n    receives\
  \ no scope string; it discovers its limits by being denied at call time.\n  denial_codes:\n  - {code: 15003, meaning: APP没有访问权限 — app lacks access permission}\n  - {code: 20014, meaning: 应用没有获取该员工的数据的权限 — no permission for this employee's data}\n  - {code: 20020, meaning: 应用没有获取该企业的数据的权限 — no permission for this enterprise's data}\n  - {code: 20021, meaning: app is disabled for this enterprise}\n  - {code: 20022, meaning: 企业没有对该app授权 — the enterprise has not authorized this app}\n  - {code: 20023, meaning: APP没有访问department的权限 — no permission to access this department}\n  consequence: >-\n    An agent or integrator cannot determine, before calling, what an app is permitted to\n    do. There is no introspection endpoint, no granted-permission list in the token\n    response, and no scope registry — permission boundaries are discovered only through\n    runtime denials returned as HTTP 200 with a non-zero errorCode.\n\nscopes: []\n\nref:\n  authentication: authentication/fxiaoke-authentication.yml\n\
  \  errors: errors/fxiaoke-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxiaoke/refs/heads/main/scopes/fxiaoke-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise
- CRM
- Sales
- Marketing
- Customer Service
- Software-as-a-Service
- China
- PaaS
token_urls: []
---
