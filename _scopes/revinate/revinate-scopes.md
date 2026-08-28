---
api_specs:
- filename: revinate-porter-openapi.yml
  format: yaml
  label: Revinate Porter API
  slug: porter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/openapi/revinate-porter-openapi.yml
authorization_urls: []
description: ''
docs: https://porter.revinate.com/documentation
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Revinate Scopes
name_suffix: OAuth Scopes
note: 'These scopes are read verbatim from the scopes_supported array of Revinate''s live OpenID Connect discovery document at auth.revinate.com, an Auth0-hosted issuer. IMPORTANT BOUNDARY: this issuer authenticates users into the Revinate web application; the public Porter REST API does not use OAuth at all and has no scope surface — it authenticates with four HMAC-SHA256 headers and access is provisioned per API key by a Revinate account manager. The scope list below is therefore the identity surface, not an API authorization surface. Every scope present is a standard OIDC scope or a standard OIDC claim-scope; Revinate declares no custom/product scopes.'
overview: 'Revinate uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Revinate
provider_slug: revinate
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: revinate-scopes
source_filename: revinate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://auth.revinate.com/.well-known/openid-configuration\ndocs: https://porter.revinate.com/documentation\napplies_to: Revinate application platform (home.revinate.com) — NOT the Porter API\nnote: >-\n  These scopes are read verbatim from the scopes_supported array of Revinate's live OpenID Connect\n  discovery document at auth.revinate.com, an Auth0-hosted issuer. IMPORTANT BOUNDARY: this issuer\n  authenticates users into the Revinate web application; the public Porter REST API does not use\n  OAuth at all and has no scope surface — it authenticates with four HMAC-SHA256 headers and access\n  is provisioned per API key by a Revinate account manager. The scope list below is therefore the\n  identity surface, not an API authorization surface. Every scope present is a standard OIDC scope\n  or a standard OIDC claim-scope; Revinate declares no custom/product scopes.\nissuer: https://auth.revinate.com/\nauthorization_endpoint:\
  \ https://auth.revinate.com/authorize\ntoken_endpoint: https://auth.revinate.com/oauth/token\nscope_count: 14\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token.\n  standard: true\n- name: profile\n  description: Requests the default profile claims (name, family_name, given_name, nickname, picture, etc.).\n  standard: true\n- name: offline_access\n  description: Requests a refresh token for long-lived access.\n  standard: true\n- name: email\n  description: Requests the email claim.\n  standard: true\n- name: email_verified\n  description: Requests the email_verified claim.\n  standard: true\n- name: name\n  description: Requests the full name claim.\n  standard: true\n- name: given_name\n  description: Requests the given name claim.\n  standard: true\n- name: family_name\n  description: Requests the family name claim.\n  standard: true\n- name: nickname\n  description: Requests the nickname claim.\n  standard: true\n- name: picture\n  description: Requests\
  \ the profile picture claim.\n  standard: true\n- name: phone\n  description: Requests the phone_number claim.\n  standard: true\n- name: address\n  description: Requests the address claim.\n  standard: true\n- name: created_at\n  description: Requests the account created_at claim.\n  standard: true\n- name: identities\n  description: Auth0 identities claim — linked identity-provider accounts for the user.\n  standard: false\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n- implicit\n- password\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\npkce_methods_supported:\n- S256\n- plain\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revinate/refs/heads/main/scopes/revinate-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Hospitality
- Hotels
- Reviews
- Reputation Management
- Guest Data Platform
- CRM
- Sentiment Analysis
- Travel
- Marketing
- Customer Feedback
token_urls: []
---
