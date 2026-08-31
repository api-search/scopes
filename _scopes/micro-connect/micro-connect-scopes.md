---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Micro Connect Scopes
name_suffix: OAuth Scopes
note: These are the OpenID Connect / Keycloak built-in client scopes the numa-realm authorisation server advertises anonymously. Micro Connect publishes NO business-domain scope reference — there is no documented scope for revenue reporting, order-detail submission, settlement export or any other Open Platform capability. Authorisation for those capabilities is carried in Keycloak realm/client ROLES inside the access token (the Open Platform bundle reads resource_access[clientId].roles), and that role catalogue is not published. Do not read this list as an API permission model; it is the identity layer only.
overview: 'Micro Connect uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Micro Connect
provider_slug: micro-connect
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: micro-connect-scopes
source_filename: micro-connect-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  scopes_supported read verbatim from\n  https://kc.mcisaas.com/auth/realms/numa-realm/.well-known/openid-configuration (HTTP 200),\n  saved in well-known/micro-connect-kc-numa-realm-openid-configuration.json\ndocs: null\nnote: >-\n  These are the OpenID Connect / Keycloak built-in client scopes the numa-realm authorisation\n  server advertises anonymously. Micro Connect publishes NO business-domain scope reference —\n  there is no documented scope for revenue reporting, order-detail submission, settlement\n  export or any other Open Platform capability. Authorisation for those capabilities is\n  carried in Keycloak realm/client ROLES inside the access token (the Open Platform bundle\n  reads resource_access[clientId].roles), and that role catalogue is not published. Do not\n  read this list as an API permission model; it is the identity layer only.\nauthorization_server: https://kc.mcisaas.com/auth/realms/numa-realm\nscope_count:\
  \ 10\nscopes:\n- name: openid\n  description: Required OpenID Connect scope; requests an ID token.\n  standard: true\n- name: profile\n  description: Standard OIDC profile claims (name, given_name, family_name, preferred_username).\n  standard: true\n- name: email\n  description: Standard OIDC email claim.\n  standard: true\n- name: phone\n  description: Standard OIDC phone_number claims.\n  standard: true\n- name: address\n  description: Standard OIDC address claim.\n  standard: true\n- name: roles\n  description: Keycloak built-in scope; adds realm and client role mappings to the token.\n  standard: false\n- name: web-origins\n  description: Keycloak built-in scope; adds allowed CORS origins to the token.\n  standard: false\n- name: offline_access\n  description: Requests an offline refresh token.\n  standard: true\n- name: microprofile-jwt\n  description: Keycloak built-in scope; adds MicroProfile JWT claims (upn, groups).\n  standard: false\n- name: acr\n  description: Authentication\
  \ Context Class Reference; realm advertises acr_values 0 and 1.\n  standard: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/micro-connect/refs/heads/main/scopes/micro-connect-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial-Services
- Capital Markets
- Exchanges
- Revenue-Based Financing
- Fintech
- Investing
- Small Business
- Hong Kong
- Macao
- China
token_urls: []
---
