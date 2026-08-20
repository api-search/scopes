---
api_specs:
- filename: unify-events-api-openapi.yml
  format: yaml
  label: Unify Analytics Events API
  slug: unify-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-events-api-openapi.yml
- filename: unify-event-query-jobs-api-openapi.yml
  format: yaml
  label: Unify Event Query Jobs API
  slug: unify-event-query-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-event-query-jobs-api-openapi.yml
- filename: unify-objects-api-openapi.yml
  format: yaml
  label: Unify Objects API
  slug: unify-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-objects-api-openapi.yml
- filename: unify-object-attributes-api-openapi.yml
  format: yaml
  label: Unify Object Attributes API
  slug: unify-object-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-attributes-api-openapi.yml
- filename: unify-object-attribute-options-api-openapi.yml
  format: yaml
  label: Unify Object Attribute Options API
  slug: unify-object-attribute-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-attribute-options-api-openapi.yml
- filename: unify-object-records-api-openapi.yml
  format: yaml
  label: Unify Object Records API
  slug: unify-object-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-records-api-openapi.yml
- filename: unify-object-record-query-jobs-api-openapi.yml
  format: yaml
  label: Unify Object Record Query Jobs API
  slug: unify-object-record-query-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-object-record-query-jobs-api-openapi.yml
- filename: unify-sequences-api-openapi.yml
  format: yaml
  label: Unify Sequences API
  slug: unify-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequences-api-openapi.yml
- filename: unify-sequence-enrollments-api-openapi.yml
  format: yaml
  label: Unify Sequence Enrollments API
  slug: unify-sequence-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequence-enrollments-api-openapi.yml
- filename: unify-sequence-enrollment-steps-api-openapi.yml
  format: yaml
  label: Unify Sequence Enrollment Steps API
  slug: unify-sequence-enrollment-steps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-sequence-enrollment-steps-api-openapi.yml
- filename: unify-tasks-api-openapi.yml
  format: yaml
  label: Unify Tasks API
  slug: unify-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/openapi/unify-tasks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.unifygtm.com/developers/mcp/getting-started
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Unify Scopes
name_suffix: OAuth Scopes
note: 'None of Unify''s four OpenAPI documents declares an oauth2 securityScheme - the REST APIs are x-api-key (Data/Sequences/Tasks) and HTTP Basic (Analytics), so derive-oauth-scopes.py has nothing to read from the specs. OAuth exists on a different surface: the hosted MCP server at https://mcp.unifygtm.com/mcp returns an RFC 9728 protected-resource document naming https://auth.unifygtm.com/ as its authorization server. The scopes below are read from that server''s live RFC 8414 metadata, saved verbatim at well-known/unify-oauth-authorization-server.json. IMPORTANT: scopes_supported here is the standard OIDC identity set advertised by the Auth0 tenant. Unify publishes NO product-permission scopes (nothing of the form read:sequences / write:records). Authorization for MCP tool calls is enforced by the identity of the logged-in user and their Unify tenant, not by scope - "every tool call is scoped to the Unify user and tenant that authenticated the connection. A tool can only read or act
  on data that user can already see in Unify." Do not read this file as a permission model for the REST APIs; there is none.'
overview: 'Unify publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unify API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unify
provider_slug: unify
schemes: []
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- email_verified
- name
- given_name
- family_name
- nickname
- picture
- phone
- address
- created_at
- identities
scopes:
- description: Standard OIDC scope requesting an ID token for the authenticated Unify user.
  flows: []
  scope: openid
- description: Standard OIDC scope for the user's basic profile claims.
  flows: []
  scope: profile
- description: Requests a refresh token so an MCP client can keep the connection alive without re-prompting.
  flows: []
  scope: offline_access
- description: The user's email address.
  flows: []
  scope: email
- description: ''
  flows: []
  scope: email_verified
- description: ''
  flows: []
  scope: name
- description: ''
  flows: []
  scope: given_name
- description: ''
  flows: []
  scope: family_name
- description: ''
  flows: []
  scope: nickname
- description: ''
  flows: []
  scope: picture
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: created_at
- description: Linked identity-provider records for the user.
  flows: []
  scope: identities
slug: unify-scopes
source_filename: unify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.unifygtm.com/.well-known/oauth-authorization-server\ndocs: https://docs.unifygtm.com/developers/mcp/getting-started\nchecked: '2026-08-13'\napplies_to: MCP (OAuth user login) only\nnote: >-\n  None of Unify's four OpenAPI documents declares an oauth2 securityScheme - the\n  REST APIs are x-api-key (Data/Sequences/Tasks) and HTTP Basic (Analytics), so\n  derive-oauth-scopes.py has nothing to read from the specs. OAuth exists on a\n  different surface: the hosted MCP server at https://mcp.unifygtm.com/mcp returns\n  an RFC 9728 protected-resource document naming https://auth.unifygtm.com/ as its\n  authorization server. The scopes below are read from that server's live RFC 8414\n  metadata, saved verbatim at\n  well-known/unify-oauth-authorization-server.json.\n  IMPORTANT: scopes_supported here is the standard OIDC identity set advertised by\n  the Auth0 tenant. Unify publishes NO product-permission scopes (nothing\
  \ of the\n  form read:sequences / write:records). Authorization for MCP tool calls is\n  enforced by the identity of the logged-in user and their Unify tenant, not by\n  scope - \"every tool call is scoped to the Unify user and tenant that\n  authenticated the connection. A tool can only read or act on data that user can\n  already see in Unify.\" Do not read this file as a permission model for the REST\n  APIs; there is none.\nauthorization_server:\n  issuer: https://auth.unifygtm.com/\n  platform: Auth0 (custom domain on unifygtm.com)\n  authorization_endpoint: https://auth.unifygtm.com/authorize\n  token_endpoint: https://auth.unifygtm.com/oauth/token\n  device_authorization_endpoint: https://auth.unifygtm.com/oauth/device/code\n  registration_endpoint: https://auth.unifygtm.com/oidc/register\n  revocation_endpoint: https://auth.unifygtm.com/oauth/revoke\n  userinfo_endpoint: https://auth.unifygtm.com/userinfo\n  jwks_uri: https://auth.unifygtm.com/.well-known/jwks.json\n  dynamic_client_registration:\
  \ true\n  pkce_methods: [S256, plain]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  dpop_signing_alg_values_supported: [ES256]\nprotected_resource:\n  resource: https://mcp.unifygtm.com/mcp\n  authorization_servers: [https://auth.unifygtm.com/]\n  bearer_methods_supported: [header]\n  spec: RFC 9728\n  file: well-known/unify-oauth-protected-resource.json\nflows:\n  - flow: authorizationCode\n    pkce: true\n    note: The path a Claude/Cursor/Codex MCP client uses when a person logs in to Unify.\n  - flow: deviceCode\n    grant: urn:ietf:params:oauth:grant-type:device_code\n  - flow: clientCredentials\n  - flow: refreshToken\n  - flow: tokenExchange\n    grant: urn:ietf:params:oauth:grant-type:token-exchange\n  - flow: implicit\n    note: Advertised by the tenant; not a path Unify documents for MCP.\nscopes:\n  - scope: openid\n    description: Standard OIDC scope requesting an ID token for the authenticated Unify user.\n    kind: identity\n\
  \  - scope: profile\n    description: Standard OIDC scope for the user's basic profile claims.\n    kind: identity\n  - scope: offline_access\n    description: Requests a refresh token so an MCP client can keep the connection alive without re-prompting.\n    kind: identity\n  - scope: email\n    description: The user's email address.\n    kind: identity\n  - scope: email_verified\n    kind: identity\n  - scope: name\n    kind: identity\n  - scope: given_name\n    kind: identity\n  - scope: family_name\n    kind: identity\n  - scope: nickname\n    kind: identity\n  - scope: picture\n    kind: identity\n  - scope: phone\n    kind: identity\n  - scope: address\n    kind: identity\n  - scope: created_at\n    kind: identity\n  - scope: identities\n    description: Linked identity-provider records for the user.\n    kind: identity\nalternative_auth:\n  - method: api-key\n    header: x-api-key\n    detail: >-\n      Unify documents an API-key alternative for MCP clients that cannot run the\n\
  \      OAuth flow. A key carries the full authority of the Unify user it belongs to\n      and is not scope-limited.\n    source: https://docs.unifygtm.com/developers/mcp/getting-started\ngaps:\n  - id: no-product-scopes\n    detail: >-\n      There is no way for a caller - human or agent - to request less than the full\n      authority of the authenticating user. Neither the OAuth server nor the API\n      key model offers a read-only or resource-limited grant, so least-privilege\n      delegation to an agent is not expressible today.\ncross_links:\n  authentication: authentication/unify-authentication.yml\n  mcp: mcp/unify-mcp.yml\n  well_known: well-known/unify-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unify/refs/heads/main/scopes/unify-scopes.yml
summary_line: 14 scopes
tags:
- Sales
- Marketing
- Go-To-Market
- Outbound
- Intent Data
- AI Agents
- B2B
- Data Enrichment
- Sequences
- Analytics
- Task
- Bulk API
- MCP
- Agent Skills
- Webhook
token_urls: []
---
