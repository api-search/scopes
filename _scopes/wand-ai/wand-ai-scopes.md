---
authorization_urls: []
description: The scopes_supported list published by Wand's Keycloak OpenID Connect discovery document. These are Keycloak's standard realm scopes; Wand publishes no scope or permission reference page, and no product-specific scopes (agent, task, workspace, knowledge-vault …) are advertised anywhere public. Descriptions below are the standard OpenID Connect / Keycloak meanings, not Wand prose.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Wand Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wand uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wand
provider_slug: wand-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: wand-ai-scopes
source_filename: wand-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://auth.wand.ai/realms/master/.well-known/openid-configuration\nname: Wand OAuth 2.0 / OpenID Connect scopes\ndescription: >-\n  The scopes_supported list published by Wand's Keycloak OpenID Connect discovery document. These\n  are Keycloak's standard realm scopes; Wand publishes no scope or permission reference page, and no\n  product-specific scopes (agent, task, workspace, knowledge-vault …) are advertised anywhere\n  public. Descriptions below are the standard OpenID Connect / Keycloak meanings, not Wand prose.\nx-evidence:\n  fetched: '2026-09-04'\n  url: https://auth.wand.ai/realms/master/.well-known/openid-configuration\n  http_status: 200\nissuer: https://auth.wand.ai/realms/master\ndocs: null\ndocs_note: Wand publishes no scopes or permissions reference page.\nscope_count: 11\nscopes:\n- name: openid\n  description: Required to make the request an OpenID Connect authentication request.\n  standard: OpenID Connect\
  \ Core 1.0\n- name: profile\n  description: Basic profile claims — name, given_name, family_name, preferred_username.\n  standard: OpenID Connect Core 1.0\n- name: email\n  description: The email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n- name: address\n  description: The address claim.\n  standard: OpenID Connect Core 1.0\n- name: phone\n  description: The phone_number and phone_number_verified claims.\n  standard: OpenID Connect Core 1.0\n- name: offline_access\n  description: Requests a refresh token usable while the user is not present.\n  standard: OpenID Connect Core 1.0\n- name: roles\n  description: Keycloak realm and client role mappings in the token.\n  standard: Keycloak built-in\n- name: web-origins\n  description: Keycloak CORS allowed-origins claim.\n  standard: Keycloak built-in\n- name: microprofile-jwt\n  description: Eclipse MicroProfile JWT claims (upn, groups).\n  standard: MicroProfile JWT RBAC\n- name: acr\n  description: Authentication context\
  \ class reference claim.\n  standard: OpenID Connect Core 1.0\n- name: picture\n  description: The picture claim.\n  standard: OpenID Connect Core 1.0\ngaps:\n- >-\n  These are identity scopes only. No authorization scopes for the Wand platform API surface are\n  published, so an integrator cannot tell from public material what a token is allowed to do.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wand-ai/refs/heads/main/scopes/wand-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic AI
- Enterprise Software
- Workforce Automation
- Orchestration
- Process Automation
- Collaboration
- Governance
token_urls: []
---
