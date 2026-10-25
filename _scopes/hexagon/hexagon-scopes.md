---
api_specs:
- filename: developerportal
  format: yaml
  label: Hexagon Nexus API
  slug: nexus-api
  spec_type: OpenAPI
  url: https://nexus.hexagon.com/developerportal
- filename: hexagon-eam-ion-api-openapi.yml
  format: yaml
  label: HxGN EAM REST API
  slug: hxgn-eam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexagon/refs/heads/main/openapi/hexagon-eam-ion-api-openapi.yml
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
overview: 'Hexagon publishes 18 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hexagon API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hexagon
provider_slug: hexagon
schemes: []
scope_count: 18
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- roles
- web-origins
- acr
- basic
- microprofile-jwt
- user
- admin
- service_account
- hxdr_client_scope
- hxdr_claims
- hxdr_be_system_user
- mcp
scopes:
- description: Standard OIDC scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OIDC claim set - name, given_name, family_name, preferred_username.
  flows: []
  scope: profile
- description: Standard OIDC email claim.
  flows: []
  scope: email
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Standard OIDC phone claim.
  flows: []
  scope: phone
- description: Standard OIDC scope requesting a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: Keycloak built-in scope adding realm and client role mappings to the token.
  flows: []
  scope: roles
- description: Keycloak built-in scope adding allowed CORS origins to the token.
  flows: []
  scope: web-origins
- description: Keycloak built-in scope carrying the authentication context class reference.
  flows: []
  scope: acr
- description: Keycloak built-in scope carrying the minimal sub/auth_time claim set.
  flows: []
  scope: basic
- description: Keycloak built-in scope emitting MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
- description: Hexagon-specific. Undocumented.
  flows: []
  scope: user
- description: Hexagon-specific. Undocumented - name implies elevated administrative access.
  flows: []
  scope: admin
- description: Hexagon-specific. Undocumented - name implies the non-interactive client_credentials identity.
  flows: []
  scope: service_account
- description: Hexagon-specific HxDR client scope. Undocumented.
  flows: []
  scope: hxdr_client_scope
- description: Hexagon-specific HxDR claim set. Undocumented.
  flows: []
  scope: hxdr_claims
- description: Hexagon-specific HxDR back-end system-user scope. Undocumented - name implies a server-to-server identity.
  flows: []
  scope: hxdr_be_system_user
- description: The single scope the GeoCloud MCP authorization server advertises, required as the bearer scope for https://geocloud.hexagon.com/wp-json/mcp/mcp-oauth-server.
  flows: []
  scope: mcp
slug: hexagon-scopes
source_filename: hexagon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: scopes_supported read verbatim from https://hxauth.com/auth/realms/geo-hxdr-prod/.well-known/openid-configuration\n  (HTTP 200) and from https://geocloud.hexagon.com/.well-known/oauth-authorization-server (HTTP 200).\ndocs: null\ndocs_note: No scope or permission reference page is published anywhere on the public Hexagon GeoCloud or Leica Geosystems\n  documentation surface. The descriptions below are the standard OIDC/Keycloak meanings where the scope is a standard\n  one, and are marked undocumented where the scope is Hexagon-specific - the realm publishes the names but no prose.\nauthorization_servers:\n- issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n  applies_to: hexagon-ab:geocloud-graphql\n  scopes:\n  - name: openid\n    description: Standard OIDC scope requesting an ID token.\n    standard: true\n  - name: profile\n    description: Standard OIDC claim set - name, given_name, family_name, preferred_username.\n\
  \    standard: true\n  - name: email\n    description: Standard OIDC email claim.\n    standard: true\n  - name: address\n    description: Standard OIDC address claim.\n    standard: true\n  - name: phone\n    description: Standard OIDC phone claim.\n    standard: true\n  - name: offline_access\n    description: Standard OIDC scope requesting a refresh token usable while the user is offline.\n    standard: true\n  - name: roles\n    description: Keycloak built-in scope adding realm and client role mappings to the token.\n    standard: false\n  - name: web-origins\n    description: Keycloak built-in scope adding allowed CORS origins to the token.\n    standard: false\n  - name: acr\n    description: Keycloak built-in scope carrying the authentication context class reference.\n    standard: false\n  - name: basic\n    description: Keycloak built-in scope carrying the minimal sub/auth_time claim set.\n    standard: false\n  - name: microprofile-jwt\n    description: Keycloak built-in scope\
  \ emitting MicroProfile JWT claims (upn, groups).\n    standard: false\n  - name: user\n    description: Hexagon-specific. Undocumented.\n    standard: false\n    documented: false\n  - name: admin\n    description: Hexagon-specific. Undocumented - name implies elevated administrative access.\n    standard: false\n    documented: false\n  - name: service_account\n    description: Hexagon-specific. Undocumented - name implies the non-interactive client_credentials identity.\n    standard: false\n    documented: false\n  - name: hxdr_client_scope\n    description: Hexagon-specific HxDR client scope. Undocumented.\n    standard: false\n    documented: false\n  - name: hxdr_claims\n    description: Hexagon-specific HxDR claim set. Undocumented.\n    standard: false\n    documented: false\n  - name: hxdr_be_system_user\n    description: Hexagon-specific HxDR back-end system-user scope. Undocumented - name implies a server-to-server\n      identity.\n    standard: false\n    documented: false\n\
  - issuer: https://geocloud.hexagon.com\n  applies_to: hexagon-ab:geocloud-mcp\n  scopes:\n  - name: mcp\n    description: The single scope the GeoCloud MCP authorization server advertises, required as the bearer scope\n      for https://geocloud.hexagon.com/wp-json/mcp/mcp-oauth-server.\n    standard: false\n    documented: false\nscope_count: 18\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token.\n  standard: true\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: profile\n  description: Standard OIDC claim set - name, given_name, family_name, preferred_username.\n  standard: true\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: email\n  description: Standard OIDC email claim.\n  standard: true\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: address\n  description: Standard OIDC address claim.\n  standard: true\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: phone\n  description: Standard\
  \ OIDC phone claim.\n  standard: true\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: offline_access\n  description: Standard OIDC scope requesting a refresh token usable while the user is offline.\n  standard: true\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: roles\n  description: Keycloak built-in scope adding realm and client role mappings to the token.\n  standard: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: web-origins\n  description: Keycloak built-in scope adding allowed CORS origins to the token.\n  standard: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: acr\n  description: Keycloak built-in scope carrying the authentication context class reference.\n  standard: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: basic\n  description: Keycloak built-in scope carrying the minimal sub/auth_time claim set.\n  standard: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n\
  - name: microprofile-jwt\n  description: Keycloak built-in scope emitting MicroProfile JWT claims (upn, groups).\n  standard: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: user\n  description: Hexagon-specific. Undocumented.\n  standard: false\n  documented: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: admin\n  description: Hexagon-specific. Undocumented - name implies elevated administrative access.\n  standard: false\n  documented: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: service_account\n  description: Hexagon-specific. Undocumented - name implies the non-interactive client_credentials identity.\n  standard: false\n  documented: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: hxdr_client_scope\n  description: Hexagon-specific HxDR client scope. Undocumented.\n  standard: false\n  documented: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: hxdr_claims\n  description:\
  \ Hexagon-specific HxDR claim set. Undocumented.\n  standard: false\n  documented: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: hxdr_be_system_user\n  description: Hexagon-specific HxDR back-end system-user scope. Undocumented - name implies a server-to-server\n    identity.\n  standard: false\n  documented: false\n  issuer: https://hxauth.com/auth/realms/geo-hxdr-prod\n- name: mcp\n  description: The single scope the GeoCloud MCP authorization server advertises, required as the bearer scope for\n    https://geocloud.hexagon.com/wp-json/mcp/mcp-oauth-server.\n  standard: false\n  documented: false\n  issuer: https://geocloud.hexagon.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexagon/refs/heads/main/scopes/hexagon-scopes.yml
summary_line: 18 scopes
tags:
- Manufacturing
- Metrology
- Quality Inspection
- Digital Factory
- Production Monitoring
- Industrial IoT
- Smart Manufacturing
- Geospatial
token_bound: false
token_urls: []
---
