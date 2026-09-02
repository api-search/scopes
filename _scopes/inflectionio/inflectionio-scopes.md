---
api_specs:
- filename: inflectionio-contact-activity-api-openapi.yml
  format: yaml
  label: Inflection.io Contact Activity API
  slug: inflectionio-contact-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-contact-activity-api-openapi.yml
- filename: inflectionio-contacts-api-openapi.yml
  format: yaml
  label: Inflection.io Contacts API
  slug: inflectionio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-contacts-api-openapi.yml
- filename: inflectionio-emails-api-openapi.yml
  format: yaml
  label: Inflection.io Emails API
  slug: inflectionio-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-emails-api-openapi.yml
- filename: inflectionio-email-versions-api-openapi.yml
  format: yaml
  label: Inflection.io Email Versions API
  slug: inflectionio-email-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-email-versions-api-openapi.yml
- filename: inflectionio-lists-and-members-api-openapi.yml
  format: yaml
  label: Inflection.io Lists and Members API
  slug: inflectionio-lists-and-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/openapi/inflectionio-lists-and-members-api-openapi.yml
authorization_urls:
- https://auth-v2.inflection.io/oauth2/authorize
description: ''
docs: https://docs.inflection.io/agents/connected-apps-oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Inflectionio Scopes
name_suffix: OAuth Scopes
note: 'The OpenAPI declares only an http/bearer securityScheme, so nothing about OAuth is derivable from the spec. Inflection nonetheless runs a full OAuth 2.1 + PKCE authorization server for Connected Apps, documented in the developer docs and discoverable anonymously via RFC 8414 metadata. Scopes below are read from that live metadata document and from the docs'' authorization-request reference. Scope granularity is coarse: a single application scope (inflection_app) grants the app the acting user''s own permissions, so authorization is by USER ROLE, not by scope.'
overview: 'Inflection.io publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Inflection.io API on a user''s behalf.


  Tokens are issued from https://auth-v2.inflection.io/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Inflection.io
provider_slug: inflectionio
schemes:
- flows:
  - authorizationUrl: https://auth-v2.inflection.io/oauth2/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    introspectionUrl: https://auth-v2.inflection.io/oauth2/introspect
    jwksUri: https://auth-v2.inflection.io/oauth2/jwks
    refreshUrl: https://auth-v2.inflection.io/oauth2/token
    registrationUrl: https://auth-v2.inflection.io/client-app/connect/register
    revocationUrl: https://auth-v2.inflection.io/oauth2/revoke
    tokenUrl: https://auth-v2.inflection.io/oauth2/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - private_key_jwt
  name: OAuth 2.1 Connected App
  pkce: required
  pkce_methods:
  - S256
  source: https://docs.inflection.io/agents/connected-apps-oauth
  type: oauth2
scope_count: 3
scope_names:
- inflection_app
- profile
- email
scopes:
- description: The application scope required on every authorization request. Grants the connected app the permissions of the user who authorized it — admins and members read and write, viewers are read-only. Also the only scope advertised by the MCP protected-resource metadata.
  flows:
  - authorizationCode
  scope: inflection_app
- description: Advertised in the authorization server's scopes_supported. Not documented in the Connected Apps guide.
  flows:
  - authorizationCode
  scope: profile
- description: Advertised in the authorization server's scopes_supported. Not documented in the Connected Apps guide.
  flows:
  - authorizationCode
  scope: email
slug: inflectionio-scopes
source_filename: inflectionio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.inflection.io/agents/connected-apps-oauth\ndocs: https://docs.inflection.io/agents/connected-apps-oauth\ndiscovery: https://auth-v2.inflection.io/.well-known/oauth-authorization-server\nnote: >-\n  The OpenAPI declares only an http/bearer securityScheme, so nothing about OAuth is derivable from the\n  spec. Inflection nonetheless runs a full OAuth 2.1 + PKCE authorization server for Connected Apps,\n  documented in the developer docs and discoverable anonymously via RFC 8414 metadata. Scopes below are\n  read from that live metadata document and from the docs' authorization-request reference. Scope\n  granularity is coarse: a single application scope (inflection_app) grants the app the acting user's\n  own permissions, so authorization is by USER ROLE, not by scope.\nschemes:\n- name: OAuth 2.1 Connected App\n  type: oauth2\n  source: https://docs.inflection.io/agents/connected-apps-oauth\n  pkce: required\n  pkce_methods:\
  \ [S256]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth-v2.inflection.io/oauth2/authorize\n    tokenUrl: https://auth-v2.inflection.io/oauth2/token\n    refreshUrl: https://auth-v2.inflection.io/oauth2/token\n    revocationUrl: https://auth-v2.inflection.io/oauth2/revoke\n    introspectionUrl: https://auth-v2.inflection.io/oauth2/introspect\n    jwksUri: https://auth-v2.inflection.io/oauth2/jwks\n    registrationUrl: https://auth-v2.inflection.io/client-app/connect/register\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt]\nscopes:\n- scope: inflection_app\n  description: >-\n    The application scope required on every authorization request. Grants the connected app the\n    permissions of the user who authorized it — admins and members read and write, viewers are\n    read-only. Also the only scope advertised by the MCP protected-resource metadata.\n  flows: [authorizationCode]\n\
  \  required: true\n  sources:\n  - https://auth-v2.inflection.io/.well-known/oauth-authorization-server\n  - https://mcp.inflection.io/.well-known/oauth-protected-resource\n  - https://docs.inflection.io/agents/connected-apps-oauth\n- scope: profile\n  description: Advertised in the authorization server's scopes_supported. Not documented in the Connected Apps guide.\n  flows: [authorizationCode]\n  sources: [https://auth-v2.inflection.io/.well-known/oauth-authorization-server]\n- scope: email\n  description: Advertised in the authorization server's scopes_supported. Not documented in the Connected Apps guide.\n  flows: [authorizationCode]\n  sources: [https://auth-v2.inflection.io/.well-known/oauth-authorization-server]\npat_permissions:\n  note: >-\n    Personal Access Tokens are the other credential type and carry coarse permissions rather than OAuth\n    scopes. PATs do not work against the MCP server.\n  permissions:\n  - {name: READ, description: Required for every GET request.}\n\
  \  - {name: WRITE, description: Required for POST, PATCH and DELETE requests.}\ntoken_lifetimes:\n  oauth_access_token_seconds: 900\n  oauth_access_token_note: 15-minute access-token lifetime with refresh-token rotation and reuse detection (MCP trust page).\n  authorization_code_seconds: 300\n  authorization_code_note: Authorization codes are valid for 5 minutes and are single-use; reuse invalidates the session.\n  pat: long-lived until revoked\nsee:\n- authentication/inflectionio-authentication.yml\n- mcp/inflectionio-mcp.yml\n- well-known/inflectionio-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflectionio/refs/heads/main/scopes/inflectionio-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Software-as-a-Service
- Marketing
- Marketing Automation
- Email Marketing
- Customer Data
- B2B
- Contacts
- MCP
- Agents
- Artificial Intelligence
- Customer Journeys
- Webhook
token_urls:
- https://auth-v2.inflection.io/oauth2/token
---
