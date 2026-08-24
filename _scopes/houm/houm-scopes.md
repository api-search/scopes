---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Houm Scopes
name_suffix: OAuth Scopes
note: Read verbatim from scopes_supported in the OpenID Connect discovery document Houm's Auth0 custom domain serves at auth.houm.com. These are the standard OIDC scopes an Auth0 tenant advertises — Houm publishes no API-specific or product-specific scope reference, because it publishes no public API. No scope descriptions are provided by the issuer; the descriptions below are the OpenID Connect Core 1.0 / Auth0 standard meanings of each claim scope, not Houm's own text.
overview: 'Houm uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Houm
provider_slug: houm
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: houm-scopes
source_filename: houm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://auth.houm.com/.well-known/openid-configuration\nname: Houm OAuth / OIDC scopes\nnote: >-\n  Read verbatim from scopes_supported in the OpenID Connect discovery document Houm's Auth0 custom\n  domain serves at auth.houm.com. These are the standard OIDC scopes an Auth0 tenant advertises —\n  Houm publishes no API-specific or product-specific scope reference, because it publishes no\n  public API. No scope descriptions are provided by the issuer; the descriptions below are the\n  OpenID Connect Core 1.0 / Auth0 standard meanings of each claim scope, not Houm's own text.\ndocs: null\nscope_count: 14\nscopes:\n- name: openid\n  description: Required to obtain an ID token; identifies the request as OpenID Connect.\n- name: profile\n  description: Basic profile claims (name, family_name, given_name, nickname, picture, updated_at).\n- name: offline_access\n  description: Issues a refresh token so the client can obtain new access\
  \ tokens without the user present.\n- name: name\n  description: The end-user's full name claim.\n- name: given_name\n  description: The end-user's given name claim.\n- name: family_name\n  description: The end-user's family name claim.\n- name: nickname\n  description: The end-user's nickname claim.\n- name: email\n  description: The end-user's email address claim.\n- name: email_verified\n  description: Whether the end-user's email address has been verified.\n- name: picture\n  description: URL of the end-user's profile picture.\n- name: created_at\n  description: Auth0 claim carrying the timestamp the user record was created.\n- name: identities\n  description: Auth0 claim carrying the linked identity providers for the user.\n- name: phone\n  description: The end-user's phone_number and phone_number_verified claims.\n- name: address\n  description: The end-user's postal address claim.\nevidence:\n- url: https://auth.houm.com/.well-known/openid-configuration\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/houm/refs/heads/main/scopes/houm-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Real Estate
- Proptech
- Property Management
- Rentals
- Marketplace
- Latin America
- Chile
- Mexico
- Colombia
token_urls: []
---
