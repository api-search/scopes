---
authorization_urls: []
description: ''
docs: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Toutiao Scopes
name_suffix: OAuth Scopes
note: Toutiao does not publish a public scopes reference page. ByteDance documents the naming convention and where the list lives, but the enumerated list itself is rendered only inside the authenticated open-platform console (管理中心 → 应用详情 → 接口权限). What follows is exactly what the provider states publicly — the convention plus the individual permissions named in the docs. It is deliberately NOT a guessed enumeration.
overview: 'Toutiao publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Toutiao API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toutiao
provider_slug: toutiao
schemes:
- authorizationUrl: https://open.snssdk.com/oauth/authorize/
  flows:
  - authorizationCode
  name: ToutiaoOAuth2
  tokenUrl: https://open.snssdk.com/oauth/access_token/
scope_count: 1
scope_names:
- mobile_alert
scopes:
- description: Grants the application the authorized user's phone number as an AES-encrypted encrypt_mobile field on the user-info response. Named explicitly in the published Toutiao/Xigua OAuth documentation.
  flows:
  - authorizationCode
  scope: mobile_alert
slug: toutiao-scopes
source_filename: toutiao-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\ndocs: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\nnote: >-\n  Toutiao does not publish a public scopes reference page. ByteDance documents the naming\n  convention and where the list lives, but the enumerated list itself is rendered only\n  inside the authenticated open-platform console (管理中心 → 应用详情 → 接口权限). What follows is\n  exactly what the provider states publicly — the convention plus the individual permissions\n  named in the docs. It is deliberately NOT a guessed enumeration.\nschemes:\n- name: ToutiaoOAuth2\n  authorizationUrl: https://open.snssdk.com/oauth/authorize/\n  tokenUrl: https://open.snssdk.com/oauth/access_token/\n  flows:\n  - authorizationCode\nconvention:\n  namespace: 'toutiao.*'\n  description: >-\n    Toutiao and Xigua applications are registered as Douyin Open\
  \ Platform applications.\n    On the permissions page, scopes prefixed toutiao. apply to Toutiao and scopes prefixed\n    xigua. apply to Xigua Video; both are granted per-application after review.\n  sibling_namespace: 'xigua.*'\n  source: https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\nscopes:\n- scope: mobile_alert\n  description: >-\n    Grants the application the authorized user's phone number as an AES-encrypted\n    encrypt_mobile field on the user-info response. Named explicitly in the published\n    Toutiao/Xigua OAuth documentation.\n  flows:\n  - authorizationCode\n  sources:\n  - https://open.douyin.com/platform/resource/docs/develop/permission/toutiao-or-xigua/OAuth2.0/\npermissions:\n- name: 视频发布及管理 (video publishing and management)\n  description: >-\n    The interface permission behind the Toutiao content-publishing solution. Documented as\n    enabled by default for every application that passes review, and located in the console\n\
  \    at 管理中心 → 应用详情 → 接口权限 → 视频发布及管理. Restricted to short-video format; articles and\n    micro-posts are explicitly out of scope.\n  console_only: true\n  sources:\n  - https://open.douyin.com/platform/resource/docs/ability/content-management/toutiao-publish-solution/\ncoverage:\n  scopes_published: 1\n  namespaces_published: 2\n  full_list_public: false\n  blocker: >-\n    The enumerated scope list is console-gated behind an approved developer application;\n    it is not reachable without registering and passing the 1-3 business day review.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toutiao/refs/heads/main/scopes/toutiao-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- News
- Content
- Media
- Social
- Recommendation
- Publishing
- ByteDance
- China
- OAuth
token_urls: []
---
