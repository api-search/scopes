---
api_specs:
- filename: ss-c-technologies-marketdataservice-api-openapi.yml
  format: yaml
  label: SS&C Technologies Market Data Service API
  slug: ss-c-technologies-marketdataservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-marketdataservice-api-openapi.yml
- filename: ss-c-technologies-submitorderservice-api-openapi.yml
  format: yaml
  label: SS&C Technologies Submit Order Service API
  slug: ss-c-technologies-submitorderservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-submitorderservice-api-openapi.yml
- filename: ss-c-technologies-userservices-api-openapi.yml
  format: yaml
  label: SS&C Technologies User Services API
  slug: ss-c-technologies-userservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-userservices-api-openapi.yml
- filename: ss-c-technologies-xapiserver-api-openapi.yml
  format: yaml
  label: SS&C Technologies XAPI Server API
  slug: ss-c-technologies-xapiserver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-xapiserver-api-openapi.yml
- filename: ss-c-technologies-utility-services-api-openapi.yml
  format: yaml
  label: SS&C Technologies Utility Services API
  slug: ss-c-technologies-utility-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/openapi/ss-c-technologies-utility-services-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.ssctech.com/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ss C Technologies Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes_supported values the SS&C APIM Keycloak realm advertises in its own OpenID Connect discovery document, read anonymously on 2026-09-13. They are NOT derived from an OpenAPI: the Eze EMS xAPI spec declares no oauth2 securityScheme, so there is no scope surface to derive there. Most entries below are Keycloak built-ins; only events_enrichment_api_member and voucher are realm-specific, and SS&C publishes no scope reference page describing what either grants — the portal''s own documentation is behind SSO.'
overview: 'SS&C Technologies uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SS&C Technologies
provider_slug: ss-c-technologies
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ss-c-technologies-scopes
source_filename: ss-c-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: https://ssoprod.ssnc.cloud/auth/realms/APIM/.well-known/openid-configuration\ndocs: https://developer.ssctech.com/\napplies_to: SS&C APIM Developer Portal (developer.ssctech.com / apim.ssnc.cloud)\nnote: >-\n  These are the scopes_supported values the SS&C APIM Keycloak realm advertises in its own OpenID\n  Connect discovery document, read anonymously on 2026-09-13. They are NOT derived from an OpenAPI:\n  the Eze EMS xAPI spec declares no oauth2 securityScheme, so there is no scope surface to derive\n  there. Most entries below are Keycloak built-ins; only events_enrichment_api_member and voucher\n  are realm-specific, and SS&C publishes no scope reference page describing what either grants —\n  the portal's own documentation is behind SSO.\nscope_count: 14\nprovider_specific_scope_count: 2\npkce_supported:\n- plain\n- S256\nscopes:\n- name: openid\n  description: OpenID Connect authentication request marker (standard).\n  standard:\
  \ true\n- name: profile\n  description: Basic profile claims (standard OIDC claim set).\n  standard: true\n- name: email\n  description: Email address claims (standard OIDC claim set).\n  standard: true\n- name: address\n  description: Address claims (standard OIDC claim set).\n  standard: true\n- name: phone\n  description: Phone number claims (standard OIDC claim set).\n  standard: true\n- name: roles\n  description: Keycloak realm and client role claims.\n  standard: true\n- name: web-origins\n  description: Keycloak CORS allowed-origins claim.\n  standard: true\n- name: acr\n  description: Authentication context class reference (standard).\n  standard: true\n- name: basic\n  description: Keycloak basic claim set (sub, auth_time).\n  standard: true\n- name: microprofile-jwt\n  description: Eclipse MicroProfile JWT claim mapping (upn, groups).\n  standard: true\n- name: offline_access\n  description: Requests a refresh token usable while the user is offline (standard).\n  standard: true\n\
  - name: service_account\n  description: Keycloak service-account client scope, used for client_credentials grants.\n  standard: true\n- name: events_enrichment_api_member\n  description: >-\n    Realm-specific scope. Its name binds it to an SS&C events-enrichment API product surfaced\n    through the APIM gateway. SS&C publishes no description of what it grants; recorded verbatim\n    from scopes_supported.\n  standard: false\n- name: voucher\n  description: >-\n    Realm-specific scope with no published description. Recorded verbatim from scopes_supported.\n  standard: false\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- implicit\n- password\n- refresh_token\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:uma-ticket\n- urn:openid:params:grant-type:ciba\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ss-c-technologies/refs/heads/main/scopes/ss-c-technologies-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Financial Services
- Investment Management
- Fund Administration
- Wealth Management
- Execution Management
- Order Management
- Market Data
- Trading
- gRPC
- Enterprise Software
token_urls: []
---
