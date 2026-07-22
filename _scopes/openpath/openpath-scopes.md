---
api_specs:
- filename: openpath-openapi-original.json
  format: json
  label: Openpath API
  slug: openpath-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/openapi/openpath-openapi-original.json
authorization_urls: []
description: ''
docs: https://openpath.readme.io/docs/using-the-api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Openpath Scopes
name_suffix: OAuth Scopes
note: The Openpath API primarily authorizes with fine-grained JWT scope strings of the form o{orgId}-<resource>:<r|w> (e.g. o123-hw:r, o123-site:w, o:w, s-o:r) issued by the Login API. In addition, an OpenID Connect / OAuth2 authorization server (issuer helium.prod.openpath.com) advertises the standard OIDC scopes below for authorization_code + PKCE flows.
overview: 'Openpath publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Openpath API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Openpath
provider_slug: openpath
schemes: []
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect authentication; returns an ID token
  flows:
  - authorizationCode
  scope: openid
- description: Access to basic profile claims (name, given_name, family_name, preferred_username)
  flows:
  - authorizationCode
  scope: profile
- description: Access to the email and email_verified claims
  flows:
  - authorizationCode
  scope: email
slug: openpath-scopes
source_filename: openpath-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.openpath.com/.well-known/openid-configuration\ndocs: https://openpath.readme.io/docs/using-the-api\nnote: >-\n  The Openpath API primarily authorizes with fine-grained JWT scope strings of\n  the form o{orgId}-<resource>:<r|w> (e.g. o123-hw:r, o123-site:w, o:w, s-o:r)\n  issued by the Login API. In addition, an OpenID Connect / OAuth2 authorization\n  server (issuer helium.prod.openpath.com) advertises the standard OIDC scopes\n  below for authorization_code + PKCE flows.\nissuer: https://helium.prod.openpath.com\nauthorization_endpoint: https://helium.prod.openpath.com/oauth/authorize\ntoken_endpoint: https://helium.prod.openpath.com/oauth/token\ngrant_types: [\"authorization_code\", \"refresh_token\"]\ncode_challenge_methods: [\"S256\"]\nscopes:\n- scope: openid\n  description: \"OpenID Connect authentication; returns an ID token\"\n  flows: [authorizationCode]\n- scope: profile\n  description: \"Access to basic\
  \ profile claims (name, given_name, family_name, preferred_username)\"\n  flows: [authorizationCode]\n- scope: email\n  description: \"Access to the email and email_verified claims\"\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpath/refs/heads/main/scopes/openpath-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Security
- Access Control
- Physical Security
- Identity
- Credentials
- IoT
- Smart Building
- Avigilon Alta
- Motorola Solutions
token_urls: []
---
