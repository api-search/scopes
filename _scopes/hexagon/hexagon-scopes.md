---
api_specs:
- filename: developerportal
  format: yaml
  label: Hexagon Nexus API
  slug: nexus-api
  spec_type: OpenAPI
  url: https://nexus.hexagon.com/developerportal
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hexagon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hexagon uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hexagon
provider_slug: hexagon
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hexagon-scopes
source_filename: hexagon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: >-\n  scopes_supported read verbatim from\n  https://hxauth.com/auth/realms/geo-hxdr-prod/.well-known/openid-configuration\n  (HTTP 200) and from\n  https://geocloud.hexagon.com/.well-known/oauth-authorization-server (HTTP 200).\ndocs: null\ndocs_note: >-\n  No scope or permission reference page is published anywhere on the public\n  Hexagon GeoCloud or Leica Geosystems documentation surface. The descriptions\n  below are the standard OIDC/Keycloak meanings where the scope is a standard one,\n  and are marked undocumented where the scope is Hexagon-specific - the realm\n  publishes the names but no prose.\nauthorization_servers:\n  - issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n    applies_to: hexagon-ab:geocloud-graphql\n    scopes:\n      - name: openid\n        description: Standard OIDC scope requesting an ID token.\n        standard: true\n      - name: profile\n        description: Standard OIDC claim set - name,\
  \ given_name, family_name, preferred_username.\n        standard: true\n      - name: email\n        description: Standard OIDC email claim.\n        standard: true\n      - name: address\n        description: Standard OIDC address claim.\n        standard: true\n      - name: phone\n        description: Standard OIDC phone claim.\n        standard: true\n      - name: offline_access\n        description: Standard OIDC scope requesting a refresh token usable while the user is offline.\n        standard: true\n      - name: roles\n        description: Keycloak built-in scope adding realm and client role mappings to the token.\n        standard: false\n      - name: web-origins\n        description: Keycloak built-in scope adding allowed CORS origins to the token.\n        standard: false\n      - name: acr\n        description: Keycloak built-in scope carrying the authentication context class reference.\n        standard: false\n      - name: basic\n        description: Keycloak built-in\
  \ scope carrying the minimal sub/auth_time claim set.\n        standard: false\n      - name: microprofile-jwt\n        description: Keycloak built-in scope emitting MicroProfile JWT claims (upn, groups).\n        standard: false\n      - name: user\n        description: Hexagon-specific. Undocumented.\n        standard: false\n        documented: false\n      - name: admin\n        description: Hexagon-specific. Undocumented - name implies elevated administrative access.\n        standard: false\n        documented: false\n      - name: service_account\n        description: >-\n          Hexagon-specific. Undocumented - name implies the non-interactive\n          client_credentials identity.\n        standard: false\n        documented: false\n      - name: hxdr_client_scope\n        description: Hexagon-specific HxDR client scope. Undocumented.\n        standard: false\n        documented: false\n      - name: hxdr_claims\n        description: Hexagon-specific HxDR claim set. Undocumented.\n\
  \        standard: false\n        documented: false\n      - name: hxdr_be_system_user\n        description: >-\n          Hexagon-specific HxDR back-end system-user scope. Undocumented - name\n          implies a server-to-server identity.\n        standard: false\n        documented: false\n  - issuer: https://geocloud.hexagon.com\n    applies_to: hexagon-ab:geocloud-mcp\n    scopes:\n      - name: mcp\n        description: >-\n          The single scope the GeoCloud MCP authorization server advertises,\n          required as the bearer scope for\n          https://geocloud.hexagon.com/wp-json/mcp/mcp-oauth-server.\n        standard: false\n        documented: false\nscope_count: 18\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexagon/refs/heads/main/scopes/hexagon-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Manufacturing
- Metrology
- Quality Inspection
- Digital Factory
- Production Monitoring
- Industrial IoT
- Smart Manufacturing
- Geospatial
token_urls: []
---
