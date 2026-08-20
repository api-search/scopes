---
authorization_urls:
- https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/authorize
description: 'Sprout Social publishes no scope reference page in its API documentation. The scope list below was read from the live RFC 8414 authorization server metadata document that the documentation names by URL (saved verbatim at well-known/sprout-social-oauth-authorization-server.json), which is the provider''s own authoritative statement of scopes_supported. Scopes are coarse-grained: they identify the organization and integration context rather than granting per-resource read/write permissions. Endpoint-level authorization is enforced by Sprout user permissions ("API Permissions") and by customer-account scoping in the URL path, not by OAuth scope.'
docs: https://api.sproutsocial.com/docs/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Sprout Social Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sprout Social publishes 6 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sprout Social API on a user''s behalf.


  Tokens are issued from https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sprout Social
provider_slug: sprout-social
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token
  - authorizationUrl: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token
  issuer: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c
  name: SproutOAuth2
  source: well-known/sprout-social-oauth-authorization-server.json
scope_count: 6
scope_names:
- openid
- profile
- email
- organization_id
- integration_id
- support
scopes:
- description: Standard OpenID Connect scope. Requests an ID token identifying the authenticated Sprout user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OpenID Connect scope. Releases profile claims such as given_name and family_name.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OpenID Connect scope. Releases the email claim.
  flows:
  - authorizationCode
  scope: email
- description: Sprout-specific scope binding the token to a Sprout organization. This is the scope used in the machine-to-machine token request published in the Sprout API documentation.
  flows:
  - clientCredentials
  - authorizationCode
  scope: organization_id
- description: Sprout-specific scope binding the token to a registered integration. Surfaces as the iid claim on issued tokens.
  flows:
  - clientCredentials
  - authorizationCode
  scope: integration_id
- description: Sprout-specific scope. Not documented in the public API reference; its grant semantics are not published.
  flows:
  - authorizationCode
  scope: support
slug: sprout-social-scopes
source_filename: sprout-social-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/.well-known/oauth-authorization-server\ndocs: https://api.sproutsocial.com/docs/\nname: Sprout Social OAuth 2.0 scopes\ndescription: >-\n  Sprout Social publishes no scope reference page in its API documentation. The scope\n  list below was read from the live RFC 8414 authorization server metadata document\n  that the documentation names by URL (saved verbatim at\n  well-known/sprout-social-oauth-authorization-server.json), which is the provider's\n  own authoritative statement of scopes_supported. Scopes are coarse-grained: they\n  identify the organization and integration context rather than granting per-resource\n  read/write permissions. Endpoint-level authorization is enforced by Sprout user\n  permissions (\"API Permissions\") and by customer-account scoping in the URL path, not\n  by OAuth scope.\n\nschemes:\n- name: SproutOAuth2\n  issuer: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c\n\
  \  source: well-known/sprout-social-oauth-authorization-server.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token\n  - flow: authorizationCode\n    authorizationUrl: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/authorize\n    tokenUrl: https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token\n    pkce: S256\n\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope. Requests an ID token identifying the authenticated\n    Sprout user.\n  flows: [authorizationCode]\n  standard: true\n  sources: [well-known/sprout-social-oauth-authorization-server.json]\n- scope: profile\n  description: >-\n    Standard OpenID Connect scope. Releases profile claims such as given_name and\n    family_name.\n  flows: [authorizationCode]\n  standard: true\n  sources: [well-known/sprout-social-oauth-authorization-server.json]\n\
  - scope: email\n  description: Standard OpenID Connect scope. Releases the email claim.\n  flows: [authorizationCode]\n  standard: true\n  sources: [well-known/sprout-social-oauth-authorization-server.json]\n- scope: organization_id\n  description: >-\n    Sprout-specific scope binding the token to a Sprout organization. This is the scope\n    used in the machine-to-machine token request published in the Sprout API\n    documentation.\n  flows: [clientCredentials, authorizationCode]\n  standard: false\n  documented_in_api_docs: true\n  sources: [well-known/sprout-social-oauth-authorization-server.json, https://api.sproutsocial.com/docs/]\n- scope: integration_id\n  description: >-\n    Sprout-specific scope binding the token to a registered integration. Surfaces as\n    the iid claim on issued tokens.\n  flows: [clientCredentials, authorizationCode]\n  standard: false\n  sources: [well-known/sprout-social-oauth-authorization-server.json]\n- scope: support\n  description: >-\n    Sprout-specific\
  \ scope. Not documented in the public API reference; its grant\n    semantics are not published.\n  flows: [authorizationCode]\n  standard: false\n  sources: [well-known/sprout-social-oauth-authorization-server.json]\n\nsummary:\n  scope_count: 6\n  standard_oidc_scopes: 3\n  provider_specific_scopes: 3\n  granularity: coarse\n  per_resource_scopes: false\n\ngaps:\n- No scopes/permissions reference page is published in the API documentation; only the\n  organization_id scope appears in a documented example request.\n- There are no read/write or per-endpoint scopes. An agent cannot request least\n  privilege at the OAuth layer — a token that can read analytics can also create\n  publishing posts, subject only to the Sprout user permissions behind it.\n- The `support` scope is advertised by the authorization server but is undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprout-social/refs/heads/main/scopes/sprout-social-scopes.yml
summary_line: 6 scopes · clientCredentials/authorizationCode
tags:
- Social-Media
- Social Media Management
- Publishing
- Analytics
- Reporting
- Messaging
- Listening
token_urls:
- https://identity.sproutsocial.com/oauth2/84e39c75-d770-45d9-90a9-7b79e3037d2c/v1/token
---
