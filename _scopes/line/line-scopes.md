---
api_specs:
- filename: line-messaging-api-openapi.yml
  format: yaml
  label: LINE Messaging API
  slug: line-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-messaging-api-openapi.yml
- filename: line-webhook-openapi.yml
  format: yaml
  label: LINE Messaging API Webhook
  slug: line-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-webhook-openapi.yml
- filename: line-channel-access-token-openapi.yml
  format: yaml
  label: LINE Channel Access Token API
  slug: line-channel-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-channel-access-token-openapi.yml
- filename: line-insight-openapi.yml
  format: yaml
  label: LINE Insight API
  slug: line-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-insight-openapi.yml
- filename: line-manage-audience-openapi.yml
  format: yaml
  label: LINE Manage Audience API
  slug: line-manage-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-manage-audience-openapi.yml
- filename: line-liff-openapi.yml
  format: yaml
  label: LIFF Server API
  slug: line-liff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-liff-openapi.yml
- filename: line-module-openapi.yml
  format: yaml
  label: LINE Module API
  slug: line-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-module-openapi.yml
- filename: line-module-attach-openapi.yml
  format: yaml
  label: LINE Module Attach API
  slug: line-module-attach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-module-attach-openapi.yml
- filename: line-shop-openapi.yml
  format: yaml
  label: LINE Mission Sticker API
  slug: line-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/openapi/line-shop-openapi.yml
authorization_urls: []
description: Scopes apply to LINE Login v2.1 — the end-user OAuth 2.0 / OpenID Connect surface — not to the Messaging API. Messaging API calls carry a channel access token, which is scoped to a channel and carries no scope claim at all; entitlement there is a property of the channel and the Official Account plan. Consequently no scope is derivable from the harvested OpenAPI documents, which declare only an HTTP Bearer scheme.
docs: https://developers.line.biz/en/docs/line-login/integrate-line-login/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Line Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LINE uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LINE
provider_slug: line
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: line-scopes
source_filename: line-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://access.line.me/.well-known/openid-configuration (probed 2026-08-13,\n  HTTP 200) and\n  https://developers.line.biz/en/docs/line-login/integrate-line-login/\ndocs: https://developers.line.biz/en/docs/line-login/integrate-line-login/\ndescription: >-\n  Scopes apply to LINE Login v2.1 — the end-user OAuth 2.0 / OpenID Connect\n  surface — not to the Messaging API. Messaging API calls carry a channel\n  access token, which is scoped to a channel and carries no scope claim at all;\n  entitlement there is a property of the channel and the Official Account plan.\n  Consequently no scope is derivable from the harvested OpenAPI documents,\n  which declare only an HTTP Bearer scheme.\nprovider: LINE Login v2.1\nauthorization_server: https://access.line.me\ndiscovery: https://access.line.me/.well-known/openid-configuration\nflows:\n  authorization_code:\n    authorization_endpoint: https://access.line.me/oauth2/v2.1/authorize\n\
  \    token_endpoint: https://api.line.me/oauth2/v2.1/token\n    revocation_endpoint: https://api.line.me/oauth2/v2.1/revoke\n    userinfo_endpoint: https://api.line.me/oauth2/v2.1/userinfo\n    jwks_uri: https://api.line.me/oauth2/v2.1/certs\n    response_types_supported: [code]\n    subject_types_supported: [pairwise]\n    id_token_signing_alg_values_supported: [ES256]\n    code_challenge_methods_supported: [S256]\n    pkce: >-\n      Supported and optional. Only S256 is accepted — the `plain` method is not\n      supported. A request without code_challenge simply does not use PKCE.\nscopes:\n  - name: profile\n    description: >-\n      Permission to get the user's profile — user ID, display name, profile\n      image URL and status message. Displayed as a required permission on the\n      consent screen when requested.\n    grants:\n      - GET https://api.line.me/v2/profile\n      - Access to userId, displayName, pictureUrl, statusMessage\n  - name: openid\n    description: >-\n  \
  \    Permission to obtain an ID token (JWT, ES256-signed) alongside the access\n      token, turning the OAuth flow into an OpenID Connect authentication.\n      Required for the userinfo endpoint.\n    grants:\n      - ID token issuance\n      - GET https://api.line.me/oauth2/v2.1/userinfo\n  - name: email\n    description: >-\n      Permission to receive the user's email address in the ID token. Requires\n      the openid scope and requires the channel to have applied for and been\n      granted the email permission in the LINE Developers Console.\n    grants:\n      - email claim in the ID token\n    note: >-\n      Gated — the channel must submit an application before the scope can be\n      requested.\ncombinations_documented:\n  - scope: profile\n    id_token: false\n  - scope: profile openid\n    id_token: true\n  - scope: profile openid email\n    id_token: true\n    email_claim: true\n  - scope: openid\n    id_token: true\n  - scope: openid email\n    id_token: true\n    email_claim:\
  \ true\nchannel_access_tokens:\n  scoped: false\n  note: >-\n    The Channel Access Token API issues four token types — long-lived,\n    short-lived v2.0, JWT-assertion v2.1 and stateless v3 — none of which\n    carries an OAuth scope. Authorization is channel-level and plan-level:\n    corporate/partner-only endpoints return 403 \"Access to this API is not\n    available for your account\" rather than an insufficient_scope error.\n  see: authentication/line-authentication.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/line/refs/heads/main/scopes/line-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Messaging
- Chatbots
- Social Login
- Mini Apps
- Marketing
- Webhooks
- OpenID Connect
- Audience
- Analytics
- Japan
token_urls: []
---
