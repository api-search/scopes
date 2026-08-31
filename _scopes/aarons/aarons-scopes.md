---
api_specs:
- filename: aarons-hpp-openapi.json
  format: json
  label: Aaron's Hosted Payment Page (HPP)
  slug: aarons-hpp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-hpp-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aarons Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aaron''s uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aaron's
provider_slug: aarons
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aarons-scopes
source_filename: aarons-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://login.aarons.com/.well-known/openid-configuration,\n  https://login.aarons.com/.well-known/oauth-authorization-server,\n  https://login.aarons.com/oauth2/default/.well-known/openid-configuration\nprovider: Aaron's\nproviderId: aarons\ndocs: null\nsummary: >-\n  Aaron's publishes no scope reference page. Every scope below was read out of an anonymous OAuth /\n  OIDC discovery document served by Aaron's Okta custom-domain identity host. Only one scope in the\n  set is Aaron's own — interclient_access, on the custom \"default\" authorization server the\n  myaccount.aarons.com application authenticates against. The rest are the standard OIDC set plus\n  Okta platform scopes that ship with any Okta org and are not evidence of an Aaron's API product.\nauthorization_servers:\n  - id: org\n    issuer: https://login.aarons.com\n    discovery: well-known/aarons-login-openid-configuration.json\n    scopes:\n      - name: openid\n\
  \        standard: oidc\n      - name: profile\n        standard: oidc\n      - name: email\n        standard: oidc\n      - name: address\n        standard: oidc\n      - name: phone\n        standard: oidc\n      - name: offline_access\n        standard: oauth2\n        description: Issues a refresh token.\n      - name: groups\n        standard: okta\n    note: >-\n      The /.well-known/oauth-authorization-server document on the same host additionally advertises\n      the full Okta management scope family (okta.users.*, okta.apps.*, okta.groups.* and many more).\n      Those are Okta platform administration scopes present on every Okta org — they are NOT an\n      Aaron's API surface and are deliberately not enumerated here as if they were.\n  - id: default\n    issuer: https://login.aarons.com/oauth2/default\n    discovery: well-known/aarons-login-default-openid-configuration.json\n    used_by: myaccount.aarons.com (Aaron's customer account application)\n    scopes:\n      - name:\
  \ interclient_access\n        standard: custom\n        owner: aarons\n        description: >-\n          Aaron's own custom scope on the default authorization server. Its meaning is not\n          documented anywhere public; the name and the application that requests it are the only\n          available evidence. Recorded as observed, not interpreted.\n      - name: openid\n        standard: oidc\n      - name: profile\n        standard: oidc\n      - name: email\n        standard: oidc\n      - name: address\n        standard: oidc\n      - name: phone\n        standard: oidc\n      - name: offline_access\n        standard: oauth2\n      - name: device_sso\n        standard: okta\n      - name: okta.myAccount.appAuthenticator.manage\n        standard: okta\n      - name: okta.myAccount.appAuthenticator.read\n        standard: okta\n      - name: okta.myAccount.appAuthenticator.maintenance.manage\n        standard: okta\n      - name: okta.myAccount.appAuthenticator.maintenance.read\n\
  \        standard: okta\nscope_count: 8\ncustom_scope_count: 1\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/scopes/aarons-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Lease-to-Own
- Retail
- Furniture
- Electronics
- Appliances
- Consumer Finance
- Fortune 1000
token_urls: []
---
