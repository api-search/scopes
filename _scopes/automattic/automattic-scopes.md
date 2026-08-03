---
api_specs:
- filename: automattic-wordpress-com-rest-v1-1-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.1
  slug: wordpresscom-rest-api-v11
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-1-openapi.yml
- filename: automattic-wordpress-com-rest-v1-2-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.2
  slug: wordpresscom-rest-api-v12
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-2-openapi.yml
- filename: automattic-wordpress-com-rest-v1-3-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.3
  slug: wordpresscom-rest-api-v13
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-3-openapi.yml
- filename: automattic-wordpress-com-wp-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wp/v2 namespace
  slug: wordpresscom-rest-api-wpv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wp-v2-openapi.yml
- filename: automattic-wordpress-com-wpcom-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wpcom/v2 namespace
  slug: wordpresscom-rest-api-wpcomv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wpcom-v2-openapi.yml
- filename: automattic-akismet-openapi.yml
  format: yaml
  label: Akismet API
  slug: akismet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-akismet-openapi.yml
- filename: automattic-jetpack-ai-plugin-openapi.yaml
  format: yaml
  label: Jetpack AI-Plugin API
  slug: jetpack-ai-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-jetpack-ai-plugin-openapi.yaml
authorization_urls:
- https://public-api.wordpress.com/oauth2-1/authorize
description: ''
docs: https://developer.wordpress.com/docs/api/oauth2/
flows:
- authorizationCode
- refreshToken
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Automattic Scopes
name_suffix: OAuth Scopes
note: The scope list is taken verbatim from the WordPress.com OAuth 2.0 authorization server metadata (scopes_supported), and the descriptions from Automattic's published OAuth2 documentation. The same list is repeated in the RFC 9728 protected-resource metadata that guards the MCP server. This file supersedes the derived pass, which only saw the scope names carried into the OpenAPI security schemes.
overview: 'Automattic publishes 21 OAuth 2.0 scopes via the authorizationCode, refreshToken, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Automattic API on a user''s behalf.


  Tokens are issued from https://public-api.wordpress.com/oauth2-1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Automattic
provider_slug: automattic
schemes:
- flows:
  - authorizationUrl: https://public-api.wordpress.com/oauth2-1/authorize
    flow: authorizationCode
    tokenUrl: https://public-api.wordpress.com/oauth2-1/token
  - flow: refreshToken
    tokenUrl: https://public-api.wordpress.com/oauth2-1/token
  - flow: clientCredentials
    tokenUrl: https://public-api.wordpress.com/oauth2-1/token
  introspection_endpoint: https://public-api.wordpress.com/oauth2-1/token-info
  issuer: https://public-api.wordpress.com
  jwks_uri: https://public-api.wordpress.com/.well-known/jwks.json
  legacy_endpoints:
    authorizationUrl: https://public-api.wordpress.com/oauth2/authorize
    tokenUrl: https://public-api.wordpress.com/oauth2/token
  name: oauth2
  pkce:
  - S256
  registration_endpoint: https://public-api.wordpress.com/oauth2-1/register
  resource_indicators_supported: true
  revocation_endpoint: https://public-api.wordpress.com/oauth2-1/revoke
  source: https://public-api.wordpress.com/.well-known/oauth-authorization-server
  spec: OAuth 2.1
  token_expiry: two weeks (per https://developer.wordpress.com/docs/api/oauth2/)
  userinfo_endpoint: https://public-api.wordpress.com/oauth2-1/userinfo
scope_count: 21
scope_names:
- global
- auth
- openid
- profile
- email
- users
- sites
- posts
- comments
- taxonomy
- follow
- sharing
- freshly-pressed
- notifications
- insights
- read
- stats
- media
- menus
- batch
- videos
scopes:
- description: Comprehensive access across all of the user's WordPress.com sites and services.
  flows:
  - authorizationCode
  scope: global
- description: Limited scope providing access only to the /me/ endpoint.
  flows:
  - authorizationCode
  scope: auth
- description: OpenID Connect — request an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: OpenID Connect profile claims (name, preferred_username, picture, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: OpenID Connect email claims (email, email_verified).
  flows:
  - authorizationCode
  scope: email
- description: View user information.
  flows:
  - authorizationCode
  scope: users
- description: View general site information and options.
  flows:
  - authorizationCode
  scope: sites
- description: View and manage posts.
  flows:
  - authorizationCode
  scope: posts
- description: View and manage post comments.
  flows:
  - authorizationCode
  scope: comments
- description: View and manage tags and categories.
  flows:
  - authorizationCode
  scope: taxonomy
- description: Follow and unfollow blogs.
  flows:
  - authorizationCode
  scope: follow
- description: Connect social media services.
  flows:
  - authorizationCode
  scope: sharing
- description: View Freshly Pressed posts.
  flows:
  - authorizationCode
  scope: freshly-pressed
- description: View and manage user notifications.
  flows:
  - authorizationCode
  scope: notifications
- description: View analytics for your application.
  flows:
  - authorizationCode
  scope: insights
- description: Manage and view Reader subscriptions.
  flows:
  - authorizationCode
  scope: read
- description: View site statistics.
  flows:
  - authorizationCode
  scope: stats
- description: Manage site media.
  flows:
  - authorizationCode
  scope: media
- description: View and manage site menus.
  flows:
  - authorizationCode
  scope: menus
- description: Batch multiple GET requests.
  flows:
  - authorizationCode
  scope: batch
- description: View video information.
  flows:
  - authorizationCode
  scope: videos
slug: automattic-scopes
source_filename: automattic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://public-api.wordpress.com/.well-known/openid-configuration\ndocs: https://developer.wordpress.com/docs/api/oauth2/\nnote: >-\n  The scope list is taken verbatim from the WordPress.com OAuth 2.0 authorization server metadata\n  (scopes_supported), and the descriptions from Automattic's published OAuth2 documentation. The\n  same list is repeated in the RFC 9728 protected-resource metadata that guards the MCP server.\n  This file supersedes the derived pass, which only saw the scope names carried into the OpenAPI\n  security schemes.\nschemes:\n- name: oauth2\n  source: https://public-api.wordpress.com/.well-known/oauth-authorization-server\n  issuer: https://public-api.wordpress.com\n  spec: OAuth 2.1\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://public-api.wordpress.com/oauth2-1/authorize\n    tokenUrl: https://public-api.wordpress.com/oauth2-1/token\n  - flow: refreshToken\n    tokenUrl: https://public-api.wordpress.com/oauth2-1/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://public-api.wordpress.com/oauth2-1/token\n  pkce: [S256]\n  revocation_endpoint: https://public-api.wordpress.com/oauth2-1/revoke\n  introspection_endpoint: https://public-api.wordpress.com/oauth2-1/token-info\n  registration_endpoint: https://public-api.wordpress.com/oauth2-1/register\n  userinfo_endpoint: https://public-api.wordpress.com/oauth2-1/userinfo\n  jwks_uri: https://public-api.wordpress.com/.well-known/jwks.json\n  resource_indicators_supported: true\n  token_expiry: two weeks (per https://developer.wordpress.com/docs/api/oauth2/)\n  legacy_endpoints:\n    authorizationUrl: https://public-api.wordpress.com/oauth2/authorize\n    tokenUrl: https://public-api.wordpress.com/oauth2/token\nscopes:\n- scope: global\n  description: Comprehensive access across all of the user's WordPress.com sites and services.\n  flows: [authorizationCode]\n- scope: auth\n  description: Limited scope providing access only to the /me/ endpoint.\n  flows:\
  \ [authorizationCode]\n- scope: openid\n  description: OpenID Connect — request an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: OpenID Connect profile claims (name, preferred_username, picture, updated_at).\n  flows: [authorizationCode]\n- scope: email\n  description: OpenID Connect email claims (email, email_verified).\n  flows: [authorizationCode]\n- scope: users\n  description: View user information.\n  flows: [authorizationCode]\n- scope: sites\n  description: View general site information and options.\n  flows: [authorizationCode]\n- scope: posts\n  description: View and manage posts.\n  flows: [authorizationCode]\n- scope: comments\n  description: View and manage post comments.\n  flows: [authorizationCode]\n- scope: taxonomy\n  description: View and manage tags and categories.\n  flows: [authorizationCode]\n- scope: follow\n  description: Follow and unfollow blogs.\n  flows: [authorizationCode]\n- scope: sharing\n  description: Connect social media services.\n\
  \  flows: [authorizationCode]\n- scope: freshly-pressed\n  description: View Freshly Pressed posts.\n  flows: [authorizationCode]\n- scope: notifications\n  description: View and manage user notifications.\n  flows: [authorizationCode]\n- scope: insights\n  description: View analytics for your application.\n  flows: [authorizationCode]\n- scope: read\n  description: Manage and view Reader subscriptions.\n  flows: [authorizationCode]\n- scope: stats\n  description: View site statistics.\n  flows: [authorizationCode]\n- scope: media\n  description: Manage site media.\n  flows: [authorizationCode]\n- scope: menus\n  description: View and manage site menus.\n  flows: [authorizationCode]\n- scope: batch\n  description: Batch multiple GET requests.\n  flows: [authorizationCode]\n- scope: videos\n  description: View video information.\n  flows: [authorizationCode]\nclaims_supported: [sub, iss, aud, exp, iat, auth_time, nonce, name, preferred_username, picture,\n  email, email_verified, updated_at]\n\
  scoping_note: >-\n  A WordPress.com token can additionally be bound to a single site. The /me response exposes\n  token_scope and token_site_id, so a client can tell at runtime whether it holds a global or a\n  site-scoped grant.\nx-evidence:\n  fetched: '2026-07-31'\n  urls:\n  - https://public-api.wordpress.com/.well-known/openid-configuration\n  - https://public-api.wordpress.com/.well-known/oauth-authorization-server\n  - https://public-api.wordpress.com/.well-known/oauth-protected-resource\n  - https://developer.wordpress.com/docs/api/oauth2/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/scopes/automattic-scopes.yml
summary_line: 21 scopes · authorizationCode/refreshToken/clientCredentials
tags:
- Company
- Content Management
- Publishing
- Blogging
- Website Hosting
- Web Publishing
- Content
- Comments
- Spam Filtering
- Media
- Analytics
- Domains
- E-Commerce
- Open Source
- Developer Tools
- Model Context Protocol
token_urls:
- https://public-api.wordpress.com/oauth2-1/token
---
