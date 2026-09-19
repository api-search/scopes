---
api_specs:
- filename: authelia-authentication-api-openapi.yml
  format: yaml
  label: Authelia Authentication API
  slug: authelia-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-authentication-api-openapi.yml
- filename: authelia-authorization-api-openapi.yml
  format: yaml
  label: Authelia Authorization API
  slug: authelia-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-authorization-api-openapi.yml
- filename: authelia-first-factor-api-openapi.yml
  format: yaml
  label: Authelia First Factor API
  slug: authelia-first-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-first-factor-api-openapi.yml
- filename: authelia-oauth-2-0-api-openapi.yml
  format: yaml
  label: Authelia OAuth 2.0 API
  slug: authelia-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-oauth-2-0-api-openapi.yml
- filename: authelia-openid-connect-1-0-api-openapi.yml
  format: yaml
  label: Authelia OpenID Connect 1.0 API
  slug: authelia-openid-connect-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-openid-connect-1-0-api-openapi.yml
- filename: authelia-password-change-api-openapi.yml
  format: yaml
  label: Authelia Password Change API
  slug: authelia-password-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-password-change-api-openapi.yml
- filename: authelia-password-reset-api-openapi.yml
  format: yaml
  label: Authelia Password Reset API
  slug: authelia-password-reset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-password-reset-api-openapi.yml
- filename: authelia-second-factor-api-openapi.yml
  format: yaml
  label: Authelia Second Factor API
  slug: authelia-second-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-second-factor-api-openapi.yml
- filename: authelia-state-api-openapi.yml
  format: yaml
  label: Authelia State API
  slug: authelia-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-state-api-openapi.yml
- filename: authelia-user-elevation-api-openapi.yml
  format: yaml
  label: Authelia User Elevation API
  slug: authelia-user-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-user-elevation-api-openapi.yml
- filename: authelia-user-information-api-openapi.yml
  format: yaml
  label: Authelia User Information API
  slug: authelia-user-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-user-information-api-openapi.yml
- filename: authelia-utilities-api-openapi.yml
  format: yaml
  label: Authelia Utilities API
  slug: authelia-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-utilities-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 / OpenID Connect 1.0 scopes an Authelia deployment will accept in a registered client's `scopes` list. Authelia additionally supports operator-defined CUSTOM scopes, so this list is the built-in set, not a closed universe.
docs: https://www.authelia.com/integration/openid-connect/openid-connect-1.0-claims/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Authelia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Authelia publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Authelia API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Authelia
provider_slug: authelia
schemes:
- discovery: <base>/.well-known/openid-configuration
  name: openid
  source: openapi/authelia-api-openapi.yml#/components/securitySchemes/openid
  type: openIdConnect
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- groups
- offline_access
- offline
- authelia.bearer.authz
scopes:
- description: Required for any OpenID Connect 1.0 request. Grants the sub claim and signals that an ID Token is requested.
  flows: []
  scope: openid
- description: Standard profile claims (name, preferred_username and related standard attributes).
  flows: []
  scope: profile
- description: Standard email claims (email, email_verified, and alternate addresses where available).
  flows: []
  scope: email
- description: Standard address claim.
  flows: []
  scope: address
- description: Standard phone claims (phone_number, phone_number_verified).
  flows: []
  scope: phone
- description: Authelia extension. Grants the groups claim carrying the user's group memberships from the authentication backend, used by relying parties for authorization.
  flows: []
  scope: groups
- description: Requests a refresh token (RFC 6749 / OIDC Core offline access).
  flows: []
  scope: offline_access
- description: Legacy alias for offline_access retained for compatibility with older relying parties.
  flows: []
  scope: offline
- description: Authelia extension. Grants an access token usable as an RFC 6750 bearer token against the PROXY AUTHORIZATION endpoints in place of the session cookie. Not available by default — the authz endpoint must be explicitly configured to accept the Bearer scheme, the client must be registered with this scope, and the token audience must exactly match or prefix the requested URL. Authelia's docs state these tokens are NOT intended for use with the Authelia API itself.
  flows: []
  scope: authelia.bearer.authz
slug: authelia-scopes
source_filename: authelia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\ndocs: https://www.authelia.com/integration/openid-connect/openid-connect-1.0-claims/\nsource: >-\n  https://www.authelia.com/integration/openid-connect/openid-connect-1.0-claims/,\n  https://www.authelia.com/integration/openid-connect/oauth-2.0-bearer-token-usage/,\n  https://www.authelia.com/configuration/identity-providers/openid-connect/clients/ and\n  https://github.com/authelia/authelia/blob/master/internal/configuration/validator/const.go\n  (validOIDCClientScopes — the authoritative list the server validates client registrations against).\ndescription: >-\n  OAuth 2.0 / OpenID Connect 1.0 scopes an Authelia deployment will accept in a registered client's\n  `scopes` list. Authelia additionally supports operator-defined CUSTOM scopes, so this list is the\n  built-in set, not a closed universe.\nschemes:\n- name: openid\n  type: openIdConnect\n  discovery: <base>/.well-known/openid-configuration\n  source: openapi/authelia-api-openapi.yml#/components/securitySchemes/openid\n\
  grant_types: [authorization_code, refresh_token, client_credentials, implicit, urn:ietf:params:oauth:grant-type:device_code]\nscopes:\n- scope: openid\n  description: >-\n    Required for any OpenID Connect 1.0 request. Grants the sub claim and signals that an ID Token is\n    requested.\n  standard: true\n- scope: profile\n  description: Standard profile claims (name, preferred_username and related standard attributes).\n  standard: true\n- scope: email\n  description: Standard email claims (email, email_verified, and alternate addresses where available).\n  standard: true\n- scope: address\n  description: Standard address claim.\n  standard: true\n- scope: phone\n  description: Standard phone claims (phone_number, phone_number_verified).\n  standard: true\n- scope: groups\n  description: >-\n    Authelia extension. Grants the groups claim carrying the user's group memberships from the\n    authentication backend, used by relying parties for authorization.\n  standard: false\n- scope:\
  \ offline_access\n  description: Requests a refresh token (RFC 6749 / OIDC Core offline access).\n  standard: true\n- scope: offline\n  description: Legacy alias for offline_access retained for compatibility with older relying parties.\n  standard: false\n- scope: authelia.bearer.authz\n  description: >-\n    Authelia extension. Grants an access token usable as an RFC 6750 bearer token against the PROXY\n    AUTHORIZATION endpoints in place of the session cookie. Not available by default — the authz endpoint\n    must be explicitly configured to accept the Bearer scheme, the client must be registered with this\n    scope, and the token audience must exactly match or prefix the requested URL. Authelia's docs state\n    these tokens are NOT intended for use with the Authelia API itself.\n  standard: false\n  docs: https://www.authelia.com/integration/openid-connect/oauth-2.0-bearer-token-usage/\n  constraints:\n    grant_types: [authorization_code, refresh_token, client_credentials]\n  \
  \  response_modes: [form_post, form_post.jwt]\n    response_types: [code]\n    audience_required: true\ncustom_scopes:\n  supported: true\n  description: >-\n    Operators can define arbitrary scopes under identity_providers.oidc.scopes and bind them to custom\n    claims via a claims policy, then permit individual clients to request them. Custom scope names are\n    deployment-specific and therefore not enumerable here.\n  docs: https://www.authelia.com/integration/openid-connect/openid-connect-1.0-claims/\nnotes:\n- >-\n  Because Authelia supports the OIDC claims parameter, the ID Token is deliberately minimal; scope-granted\n  claims are generally read from the UserInfo endpoint with the access token rather than from the ID Token.\n- >-\n  This file upgrades a 2026-07-11 derived artifact that listed only the five scopes visible in a\n  best-effort scaffold spec and carried an example-host authorizationUrl.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/scopes/authelia-scopes.yml
summary_line: 9 scopes
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open-Source
- OpenID Connect
- Self-Hosted
- SSO
token_urls: []
---
