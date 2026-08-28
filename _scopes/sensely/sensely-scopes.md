---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sensely Scopes
name_suffix: OAuth Scopes
note: 'Sensely publishes no scopes or permissions reference. The only authorization vocabulary that can be read without credentials is the scope list advertised by its Cognito user pool, which is the stock OIDC set — Cognito supports custom resource-server scopes and none are declared here. The partner credential flow at apis.sensely.com/authenticate/authenticate is not scope-bearing: it returns an opaque token pair, and any per-partner entitlement is carried by the procedureId and program code rather than by a scope.'
overview: 'Sensely uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sensely
provider_slug: sensely
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sensely-scopes
source_filename: sensely-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://cognito-idp.us-west-1.amazonaws.com/us-west-1_pMO3JfnoS/.well-known/openid-configuration\n  (HTTP 200, fetched 2026-08-26) — the discovery document for the Amazon Cognito user pool named in\n  Sensely's own published Web SDK bundle.\napi: sensely-platform-api\nnote: >-\n  Sensely publishes no scopes or permissions reference. The only authorization vocabulary that can be\n  read without credentials is the scope list advertised by its Cognito user pool, which is the stock\n  OIDC set — Cognito supports custom resource-server scopes and none are declared here. The partner\n  credential flow at apis.sensely.com/authenticate/authenticate is not scope-bearing: it returns an\n  opaque token pair, and any per-partner entitlement is carried by the procedureId and program code\n  rather than by a scope.\nscope_count: 4\nscopes:\n- name: openid\n  description: 'Standard OIDC scope; requests an id token.'\n  source: cognito-discovery\n\
  - name: email\n  description: \"Grants access to the user's email address and email_verified claims.\"\n  source: cognito-discovery\n- name: phone\n  description: \"Grants access to the user's phone_number and phone_number_verified claims.\"\n  source: cognito-discovery\n- name: profile\n  description: 'Grants access to standard OIDC profile claims.'\n  source: cognito-discovery\ncustom_scopes: []\ngaps:\n- 'No custom resource-server scopes declared on the Cognito pool.'\n- 'No published permissions or roles reference for partner API access.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensely/refs/heads/main/scopes/sensely-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Digital Health
- Conversational AI
- Virtual Assistant
- Symptom Checker
- Patient Engagement
- Health Insurance
- Mental Health
- SDK
token_urls: []
---
