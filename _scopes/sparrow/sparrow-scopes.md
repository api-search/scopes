---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sparrow Scopes
name_suffix: OAuth Scopes
note: These are the scopes the anonymously-published OIDC discovery document on Sparrow's own sign-in domain advertises as supported. They are the standard OpenID Connect / Auth0 identity scopes for application sign-in — Sparrow publishes NO product or resource scopes, because it publishes no third-party API. Nothing here was authored by API Evangelist; the list is verbatim from scopes_supported.
overview: 'Sparrow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sparrow
provider_slug: sparrow
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: sparrow-scopes
source_filename: sparrow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://login.trysparrow.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes the anonymously-published OIDC discovery document on Sparrow's own sign-in\n  domain advertises as supported. They are the standard OpenID Connect / Auth0 identity scopes for\n  application sign-in — Sparrow publishes NO product or resource scopes, because it publishes no\n  third-party API. Nothing here was authored by API Evangelist; the list is verbatim from\n  scopes_supported.\nissuer: https://login.trysparrow.com/\nscope_count: 14\nscopes:\n- name: openid\n  description: Request an ID token; required for OpenID Connect.\n- name: profile\n  description: Basic profile claims (name, nickname, picture, created_at).\n- name: offline_access\n  description: Issue a refresh token for long-lived sessions.\n- name: name\n  description: The user's full name claim.\n- name: given_name\n  description: The user's given name claim.\n- name:\
  \ family_name\n  description: The user's family name claim.\n- name: nickname\n  description: The user's nickname claim.\n- name: email\n  description: The user's email address claim.\n- name: email_verified\n  description: Whether the user's email has been verified.\n- name: picture\n  description: The user's profile picture URL claim.\n- name: created_at\n  description: Account creation timestamp claim.\n- name: identities\n  description: Linked identity-provider identities for the user.\n- name: phone\n  description: The user's phone number claim.\n- name: address\n  description: The user's address claim.\nresource_scopes:\n  published: false\n  note: >-\n    No product/resource scopes (leave, employee, payroll, claim, document) are published anywhere on\n    Sparrow's public surface. An integrator cannot see what a Sparrow access token would be allowed\n    to do.\nevidence:\n- url: https://login.trysparrow.com/.well-known/openid-configuration\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparrow/refs/heads/main/scopes/sparrow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Leave Management
- Human Resources
- HR Tech
- Payroll
- Compliance
- Employee Benefits
- Absence Management
- SaaS
token_urls: []
---
