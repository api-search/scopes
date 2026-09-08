---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Fannie Mae Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes Fannie Mae''s own OAuth 2.0 / OpenID Connect authorization server advertises, read from its published discovery document. Fannie Mae does NOT publish a scope reference page, and no public OpenAPI declares per-operation security requirements, so the mapping of scope to API operation is not public. Descriptions below marked `inferred: true` are our reading of the scope name, not a Fannie Mae definition — nothing here is quoted from a Fannie Mae scopes document, because no such document is published.'
overview: 'Fannie Mae uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fannie Mae
provider_slug: fannie-mae
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fannie-mae-scopes
source_filename: fannie-mae-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  scopes_supported from https://fmsso.fanniemae.com/.well-known/openid-configuration (HTTP 200,\n  fetched 2026-09-07; saved verbatim as well-known/fannie-mae-fmsso-openid-configuration.json)\nnote: >-\n  These are the scopes Fannie Mae's own OAuth 2.0 / OpenID Connect authorization server advertises,\n  read from its published discovery document. Fannie Mae does NOT publish a scope reference page, and\n  no public OpenAPI declares per-operation security requirements, so the mapping of scope to API\n  operation is not public. Descriptions below marked `inferred: true` are our reading of the scope\n  name, not a Fannie Mae definition — nothing here is quoted from a Fannie Mae scopes document,\n  because no such document is published.\nauthorization_server: https://fmsso.fanniemae.com\ndocs: null\ndocs_note: No public OAuth scope reference page was found on any fanniemae.com host.\nscope_count: 15\nscopes:\n  - name: openid\n\
  \    description: Standard OpenID Connect scope — requests an ID token.\n    inferred: false\n    standard: OpenID Connect Core 1.0\n  - name: profile\n    description: Standard OpenID Connect scope — basic profile claims.\n    inferred: false\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description: Standard OpenID Connect scope — email claims.\n    inferred: false\n    standard: OpenID Connect Core 1.0\n  - name: address\n    description: Standard OpenID Connect scope — address claim.\n    inferred: false\n    standard: OpenID Connect Core 1.0\n  - name: phone\n    description: Standard OpenID Connect scope — phone claims.\n    inferred: false\n    standard: OpenID Connect Core 1.0\n  - name: idmz\n    description: >-\n      Requested by the Developer Portal client alongside openid and profile; observed in the live\n      302 to the authorization endpoint. Appears to scope access to the internet-DMZ external-party\n      surface.\n    inferred: true\n    observed_in_use:\
  \ true\n  - name: api-int.fanniemae.com\n    description: >-\n      Host-named scope. Names an internal API gateway host (api-int.fanniemae.com does not resolve\n      publicly), which is direct evidence that Fannie Mae gates API access by target gateway.\n    inferred: true\n  - name: apigee_hostnamegroups\n    description: >-\n      Names Apigee hostname groups — evidence that the API gateway behind the developer program is\n      Apigee.\n    inferred: true\n  - name: treasuryapps\n    description: Scopes access to Fannie Mae treasury applications.\n    inferred: true\n  - name: pamfa\n    description: Application-specific scope; the application it names is not publicly documented.\n    inferred: true\n  - name: extfromint\n    description: External-from-internal federation scope.\n    inferred: true\n  - name: intextusers\n    description: Internal/external user directory scope.\n    inferred: true\n  - name: p1cintext\n    description: PingOne-cloud internal/external bridging scope.\n\
  \    inferred: true\n  - name: formloginonly\n    description: Restricts the authentication experience to form login.\n    inferred: true\n  - name: write:user\n    description: Write access to user records.\n    inferred: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fannie-mae/refs/heads/main/scopes/fannie-mae-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Federal-Government
- Housing
- Mortgages
- Finance
- GSE
- Fortune 100
token_urls: []
---
