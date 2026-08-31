---
authorization_urls: []
description: 'Specright runs two independent authorization servers with two independent scope vocabularies. The Keycloak realm at login.specright.com backs the product API and advertises 19 scopes, several of them Specright-specific rather than stock Keycloak. The WordPress authorization server at www.specright.com backs the MCP endpoint and advertises exactly one scope. Every scope below was read from a live discovery document; none were inferred.

  Specright publishes no scope reference page — there is no docs URL describing what these scopes grant. The descriptions below distinguish stock OIDC/Keycloak scopes (whose meaning is defined by the specs) from Specright''s own, which are recorded by name only.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Specright Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Specright uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Specright
provider_slug: specright
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: specright-scopes
source_filename: specright-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: >-\n  https://login.specright.com/realms/Specright/.well-known/openid-configuration (200,\n  fetched 2026-08-28) and\n  https://www.specright.com/.well-known/oauth-authorization-server (200, fetched 2026-08-28).\nname: Specright OAuth scopes\ndescription: >-\n  Specright runs two independent authorization servers with two independent scope\n  vocabularies. The Keycloak realm at login.specright.com backs the product API and\n  advertises 19 scopes, several of them Specright-specific rather than stock Keycloak. The\n  WordPress authorization server at www.specright.com backs the MCP endpoint and advertises\n  exactly one scope. Every scope below was read from a live discovery document; none were\n  inferred.\n\n  Specright publishes no scope reference page — there is no docs URL describing what these\n  scopes grant. The descriptions below distinguish stock OIDC/Keycloak scopes (whose\n  meaning is defined by the specs) from Specright's\
  \ own, which are recorded by name only.\n\nauthorization_servers:\n\n  - id: specright-product-api\n    issuer: https://login.specright.com/realms/Specright\n    discovery: https://login.specright.com/realms/Specright/.well-known/openid-configuration\n    status: 200\n    protects: https://api.specright.com/v1\n    scope_count: 19\n    scopes:\n      - name: specright-api\n        vendor_defined: true\n        description: >-\n          The scope the Specright developer portal itself requests when exchanging\n          credentials at the Keycloak token endpoint. Observed in the portal's own client\n          code as the API access scope. Specright publishes no definition of what it grants.\n      - name: specright-network\n        vendor_defined: true\n        description: Specright-defined. No published definition.\n      - name: supplier-network\n        vendor_defined: true\n        description: >-\n          Specright-defined. Name suggests the supplier-collaboration surface that backs\n\
  \          the /suppliers operations, but Specright publishes no definition.\n      - name: service_account\n        vendor_defined: true\n        description: >-\n          Specright-defined. Consistent with the client_credentials grant the realm\n          advertises — the machine-to-machine path an agent would use.\n      - name: automation_role\n        vendor_defined: true\n        description: Specright-defined. No published definition.\n      - name: organization\n        vendor_defined: true\n        description: Specright-defined. No published definition.\n      - name: standalone\n        vendor_defined: true\n        description: Specright-defined. No published definition.\n      - name: basic\n        vendor_defined: false\n        description: Keycloak built-in — adds sub and auth_time claims to the token.\n      - name: openid\n        vendor_defined: false\n        description: OpenID Connect Core. Required to receive an ID token.\n      - name: profile\n        vendor_defined:\
  \ false\n        description: OIDC standard claim set — name, family_name, given_name, preferred_username.\n      - name: email\n        vendor_defined: false\n        description: OIDC standard — email and email_verified.\n      - name: address\n        vendor_defined: false\n        description: OIDC standard — the address claim.\n      - name: phone\n        vendor_defined: false\n        description: OIDC standard — phone_number and phone_number_verified.\n      - name: offline_access\n        vendor_defined: false\n        description: OIDC standard — requests a refresh token usable while the user is absent.\n      - name: roles\n        vendor_defined: false\n        description: Keycloak built-in — realm and client role mappings in the token.\n      - name: groups\n        vendor_defined: false\n        description: Keycloak built-in — group membership claim.\n      - name: web-origins\n        vendor_defined: false\n        description: Keycloak built-in — CORS allowed-origins\
  \ claim.\n      - name: microprofile-jwt\n        vendor_defined: false\n        description: Keycloak built-in — Eclipse MicroProfile JWT claims (upn, groups).\n      - name: acr\n        vendor_defined: false\n        description: Keycloak built-in — authentication context class reference.\n\n  - id: specright-website-mcp\n    issuer: https://www.specright.com\n    discovery: https://www.specright.com/.well-known/oauth-authorization-server\n    status: 200\n    protects: https://www.specright.com/wp-json/mcp/mcp-oauth-server\n    scope_count: 1\n    scopes:\n      - name: mcp\n        vendor_defined: true\n        description: >-\n          The single scope guarding the WordPress MCP server. Also named in the RFC 9728\n          protected-resource document at\n          https://www.specright.com/.well-known/oauth-protected-resource. No sub-scopes,\n          so an agent granted \"mcp\" receives the whole tool surface undifferentiated.\n\nfindings:\n  - >-\n    The product API's own reference\
  \ never mentions OAuth scopes at all — it documents\n    API-key and bearer authentication and stops there. The scope vocabulary is only visible\n    by reading the Keycloak discovery document directly, which no Specright page links to.\n  - >-\n    The MCP authorization server offers exactly one coarse scope, so consent is\n    all-or-nothing for any agent connecting to it.\n  - >-\n    Seven of the 19 realm scopes are Specright-defined and undocumented. An integrator\n    cannot tell from any published source which scope grants which API capability.\n\ndocs: null\ndocs_note: >-\n  Searched developer.specright.com, www.specright.com/plans-pricing, the integrations\n  section and the 2020 API launch post. No scopes or permissions reference page is\n  published anywhere on Specright's public surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/specright/refs/heads/main/scopes/specright-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Specification Management
- Supply Chain
- Packaging
- Product Lifecycle Management
- Manufacturing
- Sustainability
- Supplier Collaboration
- Bill of Materials
- Salesforce
- Enterprise Software
token_urls: []
---
