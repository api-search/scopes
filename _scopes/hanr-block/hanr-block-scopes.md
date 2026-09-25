---
authorization_urls: []
description: OAuth 2.0 scopes H&R Block's PingFederate authorization server advertises anonymously in its discovery document. This is the complete scopes_supported array as published — no scope reference page is reachable (developer.hrblock.com and apiportal.hrblock.com refuse connections), so descriptions for the two proprietary scopes are marked unknown rather than guessed.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hanr Block Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'H&R Block uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: H&R Block
provider_slug: hanr-block
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hanr-block-scopes
source_filename: hanr-block-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://login.hrblock.com/.well-known/openid-configuration\nprovider: H&R Block\nproviderId: hanr-block\ndescription: >-\n  OAuth 2.0 scopes H&R Block's PingFederate authorization server advertises anonymously in\n  its discovery document. This is the complete scopes_supported array as published — no\n  scope reference page is reachable (developer.hrblock.com and apiportal.hrblock.com refuse\n  connections), so descriptions for the two proprietary scopes are marked unknown rather\n  than guessed.\nissuer: https://login.hrblock.com\ndocs: null\nscope_count: 7\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    standard: true\n  - name: profile\n    description: Standard OIDC claim set — name claims (givenName, sn).\n    standard: true\n  - name: email\n    description: Standard OIDC claim set — the mail claim.\n    standard: true\n  - name: address\n    description: Standard OIDC\
  \ address claim set.\n    standard: true\n  - name: phone\n    description: Standard OIDC phone_number claim set.\n    standard: true\n  - name: hrbGuaid\n    description: >-\n      Proprietary H&R Block scope. Name suggests a global unique account identifier\n      (GUAID). No published definition is reachable; not inferred further.\n    standard: false\n  - name: hrbUcid\n    description: >-\n      Proprietary H&R Block scope. Name suggests a universal customer identifier (UCID).\n      No published definition is reachable; not inferred further.\n    standard: false\nx-evidence:\n  - url: https://login.hrblock.com/.well-known/openid-configuration\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanr-block/refs/heads/main/scopes/hanr-block-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Tax Preparation
- Financial Services
- Fortune 1000
- Identity
- Authentication
- OpenID Connect
- Consumer Software
token_urls: []
---
