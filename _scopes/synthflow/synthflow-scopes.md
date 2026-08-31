---
api_specs:
- filename: synthflow-default-api-openapi.yml
  format: yaml
  label: Synthflow Default API
  slug: synthflow-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-default-api-openapi.yml
- filename: synthflow-chat-api-openapi.yml
  format: yaml
  label: Synthflow Chat API
  slug: synthflow-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-chat-api-openapi.yml
- filename: synthflow-contacts-api-openapi.yml
  format: yaml
  label: Synthflow Contacts API
  slug: synthflow-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-contacts-api-openapi.yml
- filename: synthflow-mcp-api-openapi.yml
  format: yaml
  label: Synthflow MCP API
  slug: synthflow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-mcp-api-openapi.yml
- filename: synthflow-memorystores-api-openapi.yml
  format: yaml
  label: Synthflow Memory Stores API
  slug: synthflow-memorystores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-memorystores-api-openapi.yml
- filename: synthflow-phonenumbers-api-openapi.yml
  format: yaml
  label: Synthflow Phone Numbers API
  slug: synthflow-phonenumbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-phonenumbers-api-openapi.yml
- filename: synthflow-webhooklogs-api-openapi.yml
  format: yaml
  label: Synthflow Webhook Logs API
  slug: synthflow-webhooklogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/openapi/synthflow-webhooklogs-api-openapi.yml
authorization_urls:
- https://kind-prelude-27.authkit.app/oauth2/authorize
description: OAuth scopes reachable on the Synthflow estate. These belong to the MCP surface only — the REST Platform API declares no oauth2 security scheme and has no scope model at all (a single bearer API key carries full workspace authority). The scopes below are the IDENTITY scopes advertised by Synthflow's delegated authorization server; they are not Synthflow capability scopes, and no per-tool or per-resource scope is published.
docs: ''
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Synthflow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Synthflow publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Synthflow API on a user''s behalf.


  Tokens are issued from https://kind-prelude-27.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Synthflow
provider_slug: synthflow
schemes:
- first_party: false
  flows:
  - authorizationUrl: https://kind-prelude-27.authkit.app/oauth2/authorize
    flow: authorizationCode
    pkce_methods:
    - S256
    tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token
  - deviceAuthorizationUrl: https://kind-prelude-27.authkit.app/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token
  - flow: refreshToken
    tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token
  issuer: https://kind-prelude-27.authkit.app
  name: mcp-oauth
  provenance: Named as the authorization server by Synthflow's own RFC 9728 protected-resource metadata at mcp.synthflow.ai; WorkOS is independently named as Synthflow's identity infrastructure provider in https://docs.synthflow.ai/security.
  provider: WorkOS AuthKit
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC — issue an ID token identifying the authenticated Synthflow user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Email address claim for the authenticated user.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token so an MCP client can keep the connection alive without re-prompting.
  flows:
  - authorizationCode
  - deviceCode
  - refreshToken
  scope: offline_access
slug: synthflow-scopes
source_filename: synthflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server\nresource_metadata: https://mcp.synthflow.ai/.well-known/oauth-protected-resource\ndescription: >-\n  OAuth scopes reachable on the Synthflow estate. These belong to the MCP surface only —\n  the REST Platform API declares no oauth2 security scheme and has no scope model at all\n  (a single bearer API key carries full workspace authority). The scopes below are the\n  IDENTITY scopes advertised by Synthflow's delegated authorization server; they are not\n  Synthflow capability scopes, and no per-tool or per-resource scope is published.\n\napplies_to:\n  surface: mcp\n  resource: https://mcp.synthflow.ai/mcp\n  regions:\n    - https://mcp.synthflow.ai/mcp\n    - https://mcp.us.synthflow.ai/mcp\n    - https://mcp.eu.synthflow.ai/mcp\n\nschemes:\n  - name: mcp-oauth\n    issuer: https://kind-prelude-27.authkit.app\n    first_party: false\n    provider: WorkOS\
  \ AuthKit\n    provenance: >-\n      Named as the authorization server by Synthflow's own RFC 9728 protected-resource\n      metadata at mcp.synthflow.ai; WorkOS is independently named as Synthflow's identity\n      infrastructure provider in https://docs.synthflow.ai/security.\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://kind-prelude-27.authkit.app/oauth2/authorize\n        tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token\n        pkce_methods: [S256]\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://kind-prelude-27.authkit.app/oauth2/device_authorization\n        tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token\n      - flow: refreshToken\n        tokenUrl: https://kind-prelude-27.authkit.app/oauth2/token\n\nscopes:\n  - scope: openid\n    description: 'OIDC — issue an ID token identifying the authenticated Synthflow user.'\n    flows: [authorizationCode, deviceCode]\n    sources: ['https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server']\n\
  \  - scope: profile\n    description: 'Basic profile claims for the authenticated user.'\n    flows: [authorizationCode, deviceCode]\n    sources: ['https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server']\n  - scope: email\n    description: 'Email address claim for the authenticated user.'\n    flows: [authorizationCode, deviceCode]\n    sources: ['https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server']\n  - scope: offline_access\n    description: 'Issue a refresh token so an MCP client can keep the connection alive without re-prompting.'\n    flows: [authorizationCode, deviceCode, refreshToken]\n    sources: ['https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server']\n\nauthorization_model:\n  granularity: workspace\n  capability_scopes_published: false\n  note: >-\n    All four advertised scopes are identity scopes. Once authorized, the MCP session is\n    scoped to the connected workspace and carries the full published tool\
  \ set — including\n    delete_agent, delete_knowledge_base and batch_update_agents_by_filter. There is no\n    read-only grant, and a user cannot consent to a subset of tools at the OAuth layer.\n  compensating_control: >-\n    Synthflow pushes safety down to the tool layer instead: destructive tools require a\n    second call carrying confirmed=true, and the provider explicitly advises keeping write\n    and delete tools behind client-side approval. That is a real control, but it is\n    advisory and client-enforced, not an authorization-server boundary.\n  subaccount_targeting: 'Tools that accept workspace_id can act on a managed subaccount within the same session.'\n\nrest_api:\n  oauth2: false\n  scopes: none\n  note: >-\n    The REST Platform API uses a static bearer API key with no scopes. derive-oauth-scopes\n    would produce an empty file for the spec; this artifact exists because the MCP surface\n    genuinely has an OAuth model.\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n\
  \    - {url: 'https://mcp.synthflow.ai/.well-known/oauth-protected-resource', status: 200}\n    - {url: 'https://kind-prelude-27.authkit.app/.well-known/oauth-authorization-server', status: 200}\n    - {url: 'https://mcp.synthflow.ai/mcp', status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthflow/refs/heads/main/scopes/synthflow-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Voice
- Voice Agents
- No-Code
- Telephony
- Phone
- Outbound
- Inbound
- CRM
- Webhook
- Custom Actions
- HIPAA
- SOC 2
- MCP
- Agent Skills
- Conversational AI
- SIP
- Simulations
- Knowledge Base
token_urls:
- https://kind-prelude-27.authkit.app/oauth2/token
---
