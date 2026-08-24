---
api_specs:
- filename: kontaktio-device-management-openapi.yml
  format: yaml
  label: Kontakt.io Device Management API
  slug: kontaktio-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-device-management-openapi.yml
- filename: kontaktio-location-occupancy-openapi.yml
  format: yaml
  label: Kontakt.io Location & Occupancy API
  slug: kontaktio-location-occupancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-location-occupancy-openapi.yml
- filename: kontaktio-spaces-openapi.yml
  format: yaml
  label: Kontakt.io Spaces API
  slug: kontaktio-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-spaces-openapi.yml
- filename: kontaktio-entity-management-openapi.yml
  format: yaml
  label: Kontakt.io Entity Management Integration API
  slug: kontaktio-entity-management-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-entity-management-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Kontaktio Scopes
name_suffix: OAuth Scopes
note: 'No OpenAPI in this repo declares an oauth2 securityScheme — the specs declare http/bearer and apiKey only — so derive-oauth-scopes.py correctly found nothing. The OAuth surface is documented in prose instead: the Entity Management Integration API authenticates with the OAuth2 client-credentials grant against a per-tenant Keycloak realm. Kontakt.io publishes NO API permission scopes; the scope string in the documented token request is the standard OIDC set, and API authorization is carried by a Keycloak CLIENT ROLE (integration-api) rather than by scopes. Recorded as searched from the docs so a later derived pass cannot overwrite it.'
overview: 'Kontakt.io publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kontakt.io API on a user''s behalf.


  Tokens are issued from https://kc.cloud.{region}.kontakt.io/realms/{tenant}/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kontakt.io
provider_slug: kontaktio
schemes:
- flows:
  - flow: clientCredentials
    note: '{tenant} is the account Tenant Name, taken from the account URL https://{tenant}.app.cloud.{region}.kontakt.io'
    region_values:
    - us
    - uk
    tokenUrl: https://kc.cloud.{region}.kontakt.io/realms/{tenant}/protocol/openid-connect/token
    token_lifetime_seconds: 300
  name: keycloak-client-credentials
  source: https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow
scope_count: 4
scope_names:
- openid
- profile
- email
- mcp
scopes:
- description: Standard OIDC scope requested in the documented token call.
  flows:
  - clientCredentials
  scope: openid
- description: Standard OIDC scope requested in the documented token call.
  flows:
  - clientCredentials
  scope: profile
- description: Standard OIDC scope requested in the documented token call.
  flows:
  - clientCredentials
  scope: email
- description: Scope advertised by the MCP authorization server metadata at https://kontakt.io/.well-known/oauth-authorization-server for the WordPress-hosted MCP server. Unrelated to Kio Cloud APIs.
  flows:
  - authorizationCode
  scope: mcp
slug: kontaktio-scopes
source_filename: kontaktio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow\ndocs: https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow\nnote: 'No OpenAPI in this repo declares an oauth2 securityScheme — the specs declare\n  http/bearer and apiKey only — so derive-oauth-scopes.py correctly found nothing.\n  The OAuth surface is documented in prose instead: the Entity Management Integration\n  API authenticates with the OAuth2 client-credentials grant against a per-tenant\n  Keycloak realm. Kontakt.io publishes NO API permission scopes; the scope string in\n  the documented token request is the standard OIDC set, and API authorization is\n  carried by a Keycloak CLIENT ROLE (integration-api) rather than by scopes. Recorded\n  as searched from the docs so a later derived pass cannot overwrite it.'\n\
  schemes:\n- name: keycloak-client-credentials\n  source: https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://kc.cloud.{region}.kontakt.io/realms/{tenant}/protocol/openid-connect/token\n    token_lifetime_seconds: 300\n    region_values:\n    - us\n    - uk\n    note: '{tenant} is the account Tenant Name, taken from the account URL https://{tenant}.app.cloud.{region}.kontakt.io'\nscopes:\n- scope: openid\n  description: Standard OIDC scope requested in the documented token call.\n  flows:\n  - clientCredentials\n  kind: oidc-standard\n- scope: profile\n  description: Standard OIDC scope requested in the documented token call.\n  flows:\n  - clientCredentials\n  kind: oidc-standard\n- scope: email\n  description: Standard OIDC scope requested in the documented token call.\n  flows:\n  - clientCredentials\n  kind: oidc-standard\n- scope: mcp\n  description:\
  \ Scope advertised by the MCP authorization server metadata at https://kontakt.io/.well-known/oauth-authorization-server\n    for the WordPress-hosted MCP server. Unrelated to Kio Cloud APIs.\n  flows:\n  - authorizationCode\n  kind: mcp\nroles:\n- name: integration-api\n  kind: keycloak-client-role\n  description: Client role that grants an Integration API Client access to the Entity\n    Management Integration API. Assigned per client in Kio Cloud under Users > Integration\n    API.\n- name: integration-api (user role)\n  kind: keycloak-user-role\n  description: User Management role required for a person to create and manage Integration\n    API Clients. Assigning it requires the User Management Administrator role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/scopes/kontaktio-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Company
- IoT
- RTLS
- Healthcare
- Asset Tracking
- Location
- Occupancy
- Bluetooth
- Device Management
- Telemetry
- Sensors
- Streaming
token_urls:
- https://kc.cloud.{region}.kontakt.io/realms/{tenant}/protocol/openid-connect/token
---
