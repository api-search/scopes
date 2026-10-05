---
authorization_urls: []
description: OAuth scopes advertised by Ameren's ForgeRock AM enterprise identity service, read verbatim from the scopes_supported array of its live OIDC discovery document. These are the identity-platform scopes; they are NOT a published Share My Usage / Green Button data scope reference, which Ameren does not publish anywhere public.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ameren Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ameren publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ameren API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ameren
provider_slug: ameren
schemes: []
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- write
- fr:idm:*
- am-introspect-all-tokens
- am-introspect-all-tokens-any-realm
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows: []
  scope: openid
- description: Standard OIDC claim bundle — name, given_name, family_name, locale, zoneinfo.
  flows: []
  scope: profile
- description: Standard OIDC email claim.
  flows: []
  scope: email
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Standard OIDC phone_number claim.
  flows: []
  scope: phone
- description: Non-standard write scope advertised by the AM instance. Its semantics are not documented publicly by Ameren; recorded as advertised, not interpreted.
  flows: []
  scope: write
- description: ForgeRock Identity Management wildcard scope — vendor-native, grants IDM API access. Product default, not an Ameren-authored scope.
  flows: []
  scope: fr:idm:*
- description: ForgeRock AM administrative scope permitting introspection of any token in the realm. Product default.
  flows: []
  scope: am-introspect-all-tokens
- description: ForgeRock AM administrative scope permitting cross-realm token introspection. Product default.
  flows: []
  scope: am-introspect-all-tokens-any-realm
slug: ameren-scopes
source_filename: ameren-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://login.eiam.ece.ameren.com/am/oauth2/.well-known/openid-configuration\nprovider: Ameren\nproviderId: ameren\ndescription: >-\n  OAuth scopes advertised by Ameren's ForgeRock AM enterprise identity service, read\n  verbatim from the scopes_supported array of its live OIDC discovery document. These are\n  the identity-platform scopes; they are NOT a published Share My Usage / Green Button data\n  scope reference, which Ameren does not publish anywhere public.\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page exists on ameren.com. The Share My Usage program\n  page describes customer authorization in prose only. Searched\n  ameren.com/partners/account-and-data/share-my-usage and the third-party registration\n  guide PDF; neither enumerates scopes.\nscope_count: 9\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    standard: true\n  - name: profile\n    description:\
  \ Standard OIDC claim bundle — name, given_name, family_name, locale, zoneinfo.\n    standard: true\n  - name: email\n    description: Standard OIDC email claim.\n    standard: true\n  - name: address\n    description: Standard OIDC address claim.\n    standard: true\n  - name: phone\n    description: Standard OIDC phone_number claim.\n    standard: true\n  - name: write\n    description: >-\n      Non-standard write scope advertised by the AM instance. Its semantics are not\n      documented publicly by Ameren; recorded as advertised, not interpreted.\n    standard: false\n  - name: 'fr:idm:*'\n    description: >-\n      ForgeRock Identity Management wildcard scope — vendor-native, grants IDM API access.\n      Product default, not an Ameren-authored scope.\n    standard: false\n    vendor: ForgeRock\n  - name: am-introspect-all-tokens\n    description: >-\n      ForgeRock AM administrative scope permitting introspection of any token in the realm.\n      Product default.\n    standard:\
  \ false\n    vendor: ForgeRock\n  - name: am-introspect-all-tokens-any-realm\n    description: >-\n      ForgeRock AM administrative scope permitting cross-realm token introspection.\n      Product default.\n    standard: false\n    vendor: ForgeRock\nevidence:\n  - url: https://login.eiam.ece.ameren.com/am/oauth2/.well-known/openid-configuration\n    status: 200\n    field: scopes_supported\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ameren/refs/heads/main/scopes/ameren-scopes.yml
summary_line: 9 scopes
tags:
- Utility
- Energy
- Electric
- Natural Gas
- Smart Grid
- Green Button
- Renewable Energy
- Fortune 500
token_bound: false
token_urls: []
---
