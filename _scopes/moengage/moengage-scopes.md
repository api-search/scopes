---
api_specs:
- filename: moengage-data-openapi.yml
  format: yaml
  label: MoEngage Data API
  slug: moengage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-data-openapi.yml
- filename: moengage-campaign-draft-openapi.yml
  format: yaml
  label: MoEngage Campaigns API
  slug: moengage-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-campaign-draft-openapi.yml
- filename: moengage-push-openapi.yml
  format: yaml
  label: MoEngage Push API
  slug: moengage-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-push-openapi.yml
- filename: moengage-custom-segments-openapi.yml
  format: yaml
  label: MoEngage Segments API
  slug: moengage-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-custom-segments-openapi.yml
- filename: moengage-email-templates-1-openapi.yml
  format: yaml
  label: MoEngage Content and Templates API
  slug: moengage-content-and-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-email-templates-1-openapi.yml
- filename: moengage-catalog-openapi.yml
  format: yaml
  label: MoEngage Catalog, Recommendations and Coupons API
  slug: moengage-catalog-recommendations-and-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-catalog-openapi.yml
- filename: moengage-email-subscription-openapi.yml
  format: yaml
  label: MoEngage Subscriptions API
  slug: moengage-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-email-subscription-openapi.yml
- filename: moengage-analytics-openapi.yml
  format: yaml
  label: MoEngage Analytics and Flows API
  slug: moengage-analytics-and-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-analytics-openapi.yml
- filename: moengage-inform-openapi.yml
  format: yaml
  label: MoEngage Inform API
  slug: moengage-inform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-inform-openapi.yml
- filename: moengage-cards-openapi.yml
  format: yaml
  label: MoEngage Engagement Surfaces API
  slug: moengage-engagement-surfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/openapi/moengage-cards-openapi.yml
authorization_urls: []
description: ''
docs: https://www.moengage.com/docs/user-guide/ai-and-intelligence/merlin-ai/moengage-mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Moengage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MoEngage publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the MoEngage API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MoEngage
provider_slug: moengage
schemes:
- authorization_endpoint: https://moeauth.moengage.com/oauth2/authorize
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg:
  - RS256
  issuer: https://moeauth.moengage.com
  jwks_uri: https://moeauth.moengage.com/.well-known/jwks.json
  name: MoEngage OAuth (MCP)
  pkce:
  - S256
  protected_resource: https://mcp.moengage.com
  registration_endpoint: https://moeauth.moengage.com/oauth2/register
  response_types:
  - code
  source: well-known/moengage-oauth-authorization-server.json
  token_endpoint: https://moeauth.moengage.com/oauth2/token
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
  userinfo_endpoint: https://moeauth.moengage.com/oauth2/userinfo
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- campaigns:read
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the MoEngage user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC profile claims for the authenticated MoEngage user.
  flows:
  - authorizationCode
  scope: profile
- description: The authenticated user's MoEngage email address.
  flows:
  - authorizationCode
  scope: email
- description: Issues a refresh token so the connector can act without re-prompting on every session.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read access to campaigns in the authorized workspace.
  flows:
  - authorizationCode
  scope: campaigns:read
slug: moengage-scopes
source_filename: moengage-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: >-\n  https://moeauth.moengage.com/.well-known/oauth-authorization-server and\n  https://mcp.moengage.com/.well-known/oauth-protected-resource\ndocs: https://www.moengage.com/docs/user-guide/ai-and-intelligence/merlin-ai/moengage-mcp-server\nscope_note: >-\n  OAuth exists on the MCP/agent surface only. The 30 REST OpenAPI documents declare HTTP Basic and an\n  apiKey header (MOE-APPKEY) and carry no oauth2 securityScheme, so there are no REST scopes to derive.\n  Everything below was read from MoEngage's live RFC 8414 / RFC 9728 discovery documents.\nschemes:\n- name: MoEngage OAuth (MCP)\n  issuer: https://moeauth.moengage.com\n  authorization_endpoint: https://moeauth.moengage.com/oauth2/authorize\n  token_endpoint: https://moeauth.moengage.com/oauth2/token\n  userinfo_endpoint: https://moeauth.moengage.com/oauth2/userinfo\n  jwks_uri: https://moeauth.moengage.com/.well-known/jwks.json\n  registration_endpoint: https://moeauth.moengage.com/oauth2/register\n\
  \  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  id_token_signing_alg: [RS256]\n  protected_resource: https://mcp.moengage.com\n  source: well-known/moengage-oauth-authorization-server.json\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the MoEngage user.\n  flows: [authorizationCode]\n- scope: profile\n  description: Standard OIDC profile claims for the authenticated MoEngage user.\n  flows: [authorizationCode]\n- scope: email\n  description: The authenticated user's MoEngage email address.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issues a refresh token so the connector can act without re-prompting on every session.\n  flows: [authorizationCode]\n- scope: campaigns:read\n  description: Read\
  \ access to campaigns in the authorized workspace.\n  flows: [authorizationCode]\nclaims_supported:\n- sub\n- iss\n- aud\n- exp\n- iat\n- email\n- name\n- dc\n- tenant_id\n- db_name\n- roles\n- scope\n- client_id\nauthorization_model_note: >-\n  MoEngage documents that the OAuth consent screen may list only a read scope (for example campaigns:read)\n  even though the connector exposes write tools. Actual authorization is enforced by the user's MoEngage\n  role-based permissions and by which tools the client has enabled, not by the granted scope string. The\n  scopes_supported list is therefore narrower than the tool surface it fronts.\ntenancy_claims:\n  dc: The MoEngage data center the session belongs to.\n  tenant_id: The workspace identifier.\n  db_name: The backing datastore for the workspace.\n  roles: The user's MoEngage roles, which gate tool execution.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moengage/refs/heads/main/scopes/moengage-scopes.yml
summary_line: 5 scopes
tags:
- Customer Engagement
- Marketing Automation
- Customer Data Platform
- Push Notifications
- Email
- SMS
- WhatsApp
- In-App Messaging
- Segmentation
- Personalization
- Campaign Management
- Analytics
- Mobile SDK
- MCP
- MarTech
token_urls: []
---
