---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Zartico Scopes
name_suffix: OAuth Scopes
note: 'IMPORTANT READING NOTE. Zartico authors NO product scopes. Both authorization servers are Okta tenants, and everything advertised in scopes_supported is an Okta platform default: the seven standard OpenID Connect scopes, plus 78 okta.* org-management scopes that govern the Okta tenant itself (users, groups, apps, policies, logs, brands, domains), not Zartico destination data. There is no Zartico resource server behind these scopes that a third party can call, and Zartico publishes no scopes/permissions reference page - repeated searching of www.zartico.com and support.zartico.com found none. The okta.* list is recorded once, compressed, so a reader can see WHAT it is rather than mistaking 85 entries for a rich Zartico permission model.'
overview: 'Zartico uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zartico
provider_slug: zartico
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: zartico-scopes
source_filename: zartico-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://login.zartico.com/.well-known/openid-configuration (200) and\n  https://login.zartico.com/.well-known/oauth-authorization-server (200);\n  https://platform.zartico.com/.well-known/openid-configuration (200) and\n  https://platform.zartico.com/.well-known/oauth-authorization-server (200)\ndocs: null\nnote: |\n  IMPORTANT READING NOTE. Zartico authors NO product scopes. Both authorization servers are Okta\n  tenants, and everything advertised in scopes_supported is an Okta platform default: the seven\n  standard OpenID Connect scopes, plus 78 okta.* org-management scopes that govern the Okta\n  tenant itself (users, groups, apps, policies, logs, brands, domains), not Zartico destination\n  data. There is no Zartico resource server behind these scopes that a third party can call, and\n  Zartico publishes no scopes/permissions reference page - repeated searching of www.zartico.com\n  and support.zartico.com found none.\
  \ The okta.* list is recorded once, compressed, so a reader\n  can see WHAT it is rather than mistaking 85 entries for a rich Zartico permission model.\nscopes:\n  - name: openid\n    description: OpenID Connect authentication; returns an ID token.\n    standard: OpenID Connect Core 1.0\n    servers: [login.zartico.com, platform.zartico.com]\n  - name: email\n    description: The end user's email address and email_verified claim.\n    standard: OpenID Connect Core 1.0\n    servers: [login.zartico.com, platform.zartico.com]\n  - name: profile\n    description: Default profile claims - name, given_name, family_name, locale, updated_at.\n    standard: OpenID Connect Core 1.0\n    servers: [login.zartico.com, platform.zartico.com]\n  - name: address\n    description: The end user's postal address claim.\n    standard: OpenID Connect Core 1.0\n    servers: [login.zartico.com, platform.zartico.com]\n  - name: phone\n    description: The end user's phone_number and phone_number_verified claims.\n\
  \    standard: OpenID Connect Core 1.0\n    servers: [login.zartico.com, platform.zartico.com]\n  - name: offline_access\n    description: Issues a refresh token so the client can renew access without the user present.\n    standard: OpenID Connect Core 1.0\n    servers: [login.zartico.com, platform.zartico.com]\n  - name: groups\n    description: Group memberships of the end user, as configured in the Okta tenant.\n    standard: Okta extension\n    servers: [login.zartico.com, platform.zartico.com]\nvendor_default_scopes:\n  prefix: okta.*\n  count: 78\n  vendor: Okta\n  scope_of_control: The Okta organization itself, not Zartico product data.\n  examples:\n    - okta.users.read\n    - okta.users.manage\n    - okta.groups.read\n    - okta.apps.manage\n    - okta.policies.manage\n    - okta.logs.read\n    - okta.sessions.manage\n    - okta.apiTokens.manage\n  note: >-\n    Advertised identically by both authorization servers. Present because they are Okta org\n    authorization server\
  \ defaults - they are not evidence of a Zartico-designed permission model.\ncounts:\n  zartico_authored_scopes: 0\n  standard_oidc_scopes: 7\n  vendor_default_scopes: 78\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zartico/refs/heads/main/scopes/zartico-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Travel
- Tourism
- Destination Marketing
- Location Intelligence
- Geospatial
- Analytics
- Data
- Business Intelligence
- OGC
token_urls: []
---
