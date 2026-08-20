---
api_specs:
- filename: boom-ai-cdp-custom-objects-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Custom Objects API
  slug: boom-ai-cdp-custom-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-custom-objects-api-openapi.yml
- filename: boom-ai-cdp-events-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Events API
  slug: boom-ai-cdp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-events-api-openapi.yml
- filename: boom-ai-cdp-people-api-openapi.yml
  format: yaml
  label: Boom Ai CDP People API
  slug: boom-ai-cdp-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-people-api-openapi.yml
- filename: boom-ai-cdp-relationships-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Relationships API
  slug: boom-ai-cdp-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-relationships-api-openapi.yml
- filename: boom-ai-cdp-sources-api-openapi.yml
  format: yaml
  label: Boom Ai CDP Sources API
  slug: boom-ai-cdp-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-cdp-sources-api-openapi.yml
- filename: boom-ai-http-credentials-api-openapi.yml
  format: yaml
  label: Boom Ai HTTP credentials API
  slug: boom-ai-http-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-http-credentials-api-openapi.yml
- filename: boom-ai-initiatives-api-openapi.yml
  format: yaml
  label: Boom Ai Initiatives API
  slug: boom-ai-initiatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-initiatives-api-openapi.yml
- filename: boom-ai-journeys-api-openapi.yml
  format: yaml
  label: Boom Ai Journeys API
  slug: boom-ai-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-journeys-api-openapi.yml
- filename: boom-ai-segments-api-openapi.yml
  format: yaml
  label: Boom Ai Segments API
  slug: boom-ai-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-segments-api-openapi.yml
- filename: boom-ai-whatsapp-templates-api-openapi.yml
  format: yaml
  label: Boom Ai WhatsApp templates API
  slug: boom-ai-whatsapp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/openapi/boom-ai-whatsapp-templates-api-openapi.yml
authorization_urls:
- https://clerk.useboom.ai/oauth/authorize
description: ''
docs: https://docs.useboom.ai/use-mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Boom Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Boom Ai publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Boom Ai API on a user''s behalf.


  Tokens are issued from https://clerk.useboom.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Boom Ai
provider_slug: boom-ai
schemes:
- flows:
  - authorizationUrl: https://clerk.useboom.ai/oauth/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://clerk.useboom.ai/oauth/register
    revocationUrl: https://clerk.useboom.ai/oauth/token/revoke
    tokenUrl: https://clerk.useboom.ai/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
  introspection_endpoint: https://clerk.useboom.ai/oauth/token_info
  jwks_uri: https://clerk.useboom.ai/.well-known/jwks.json
  name: MCP OAuth (Clerk)
  source: https://clerk.useboom.ai/.well-known/oauth-authorization-server
  spec: RFC 8414
  type: oauth2
  userinfo_endpoint: https://clerk.useboom.ai/oauth/userinfo
scope_count: 7
scope_names:
- profile
- email
- user:org:read
- openid
- offline_access
- public_metadata
- private_metadata
scopes:
- description: Basic profile of the signed-in Boom user.
  flows: []
  scope: profile
- description: Email address of the signed-in Boom user.
  flows: []
  scope: email
- description: Read the user's organization membership — how the MCP server binds a session to one Boom organization. All data access is then scoped to that organization.
  flows: []
  scope: user:org:read
- description: OpenID Connect sign-in.
  flows: []
  scope: openid
- description: Refresh-token issuance for long-lived agent sessions.
  flows: []
  scope: offline_access
- description: Clerk public user metadata.
  flows: []
  scope: public_metadata
- description: Clerk private user metadata.
  flows: []
  scope: private_metadata
slug: boom-ai-scopes
source_filename: boom-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://www.useboom.ai/.well-known/oauth-protected-resource/mcp\ndocs: https://docs.useboom.ai/use-mcp\napplies_to: >-\n  The hosted MCP server ONLY (https://www.useboom.ai/mcp). The REST API has no OAuth\n  surface at all — it authenticates with a per-organization Bearer API key (boom_org_...)\n  and declares no scopes. See authentication/boom-ai-authentication.yml.\nprotected_resource:\n  resource: https://www.useboom.ai/mcp\n  metadata_url: https://www.useboom.ai/.well-known/oauth-protected-resource/mcp\n  spec: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n  authorization_servers: [https://clerk.useboom.ai]\n  discovery: >-\n    Advertised in the WWW-Authenticate header of an unauthenticated POST to the MCP\n    endpoint: Bearer error=\"invalid_token\", resource_metadata=\"…/oauth-protected-resource/mcp\".\nschemes:\n  - name: MCP OAuth (Clerk)\n    type: oauth2\n    source: https://clerk.useboom.ai/.well-known/oauth-authorization-server\n\
  \    spec: RFC 8414\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.useboom.ai/oauth/authorize\n        tokenUrl: https://clerk.useboom.ai/oauth/token\n        revocationUrl: https://clerk.useboom.ai/oauth/token/revoke\n        registrationUrl: https://clerk.useboom.ai/oauth/register\n        grant_types: [authorization_code, refresh_token]\n        dynamic_client_registration: true\n        token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    jwks_uri: https://clerk.useboom.ai/.well-known/jwks.json\n    userinfo_endpoint: https://clerk.useboom.ai/oauth/userinfo\n    introspection_endpoint: https://clerk.useboom.ai/oauth/token_info\nscopes:\n  - scope: profile\n    description: Basic profile of the signed-in Boom user.\n    required_by_resource: true\n    sources: [protected-resource-metadata, authorization-server-metadata]\n  - scope: email\n    description: Email address of the signed-in Boom user.\n    required_by_resource:\
  \ true\n    sources: [protected-resource-metadata, authorization-server-metadata]\n  - scope: user:org:read\n    description: >-\n      Read the user's organization membership — how the MCP server binds a session to one\n      Boom organization. All data access is then scoped to that organization.\n    required_by_resource: true\n    sources: [protected-resource-metadata, authorization-server-metadata]\n  - scope: openid\n    description: OpenID Connect sign-in.\n    required_by_resource: false\n    sources: [authorization-server-metadata]\n  - scope: offline_access\n    description: Refresh-token issuance for long-lived agent sessions.\n    required_by_resource: false\n    sources: [authorization-server-metadata]\n  - scope: public_metadata\n    description: Clerk public user metadata.\n    required_by_resource: false\n    sources: [authorization-server-metadata]\n  - scope: private_metadata\n    description: Clerk private user metadata.\n    required_by_resource: false\n    sources:\
  \ [authorization-server-metadata]\nauthorization_note: >-\n  The scopes are identity scopes, not capability scopes — none of them names a Boom\n  resource or an action. Authorization over Boom's data is NOT expressed in the OAuth\n  scope set: it is inherited from the signed-in user's organization membership and role,\n  with destructive actions (launching an initiative, adding participants — both of which\n  send real WhatsApp messages) gated on org-admin permission. An agent holding a token\n  cannot tell from the scope string what it is allowed to do.\nx-evidence:\n  - {url: 'https://www.useboom.ai/.well-known/oauth-protected-resource/mcp', status: 200, checked: '2026-08-13'}\n  - {url: 'https://clerk.useboom.ai/.well-known/oauth-authorization-server', status: 200, checked: '2026-08-13'}\n  - {url: 'https://clerk.useboom.ai/.well-known/openid-configuration', status: 200, checked: '2026-08-13'}\n  - {url: 'https://www.useboom.ai/mcp', status: 401, checked: '2026-08-13', note: 'POST tools/list\
  \ — invalid_token with resource_metadata challenge'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boom-ai/refs/heads/main/scopes/boom-ai-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Customer Engagement
- Customer Data Platform
- Messaging
- WhatsApp
- SMS
- Marketing Automation
- E-Commerce
- Agents
- MCP
token_urls:
- https://clerk.useboom.ai/oauth/token
---
