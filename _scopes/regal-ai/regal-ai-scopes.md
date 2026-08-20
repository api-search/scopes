---
api_specs:
- filename: regal-reporting-webhooks-asyncapi.yml
  format: yaml
  label: Regal Reporting Webhooks
  slug: regal-reporting-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/asyncapi/regal-reporting-webhooks-asyncapi.yml
- filename: regal-ai-branded-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Branded Phone Numbers API
  slug: regal-ai-branded-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-branded-phone-numbers-api-openapi.yml
- filename: regal-ai-business-profiles-api-openapi.yml
  format: yaml
  label: Regal Business Profiles API
  slug: regal-ai-business-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-business-profiles-api-openapi.yml
- filename: regal-ai-campaigns-api-openapi.yml
  format: yaml
  label: Regal Campaigns API
  slug: regal-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-campaigns-api-openapi.yml
- filename: regal-ai-dispositions-api-openapi.yml
  format: yaml
  label: Regal Dispositions API
  slug: regal-ai-dispositions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-dispositions-api-openapi.yml
- filename: regal-ai-events-api-openapi.yml
  format: yaml
  label: Regal Events API
  slug: regal-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-events-api-openapi.yml
- filename: regal-ai-messages-api-openapi.yml
  format: yaml
  label: Regal Messages API
  slug: regal-ai-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-messages-api-openapi.yml
- filename: regal-ai-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Phone Numbers API
  slug: regal-ai-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-phone-numbers-api-openapi.yml
- filename: regal-ai-users-api-openapi.yml
  format: yaml
  label: Regal Users API
  slug: regal-ai-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-users-api-openapi.yml
- filename: regal-ai-call-handoffs-api-openapi.yml
  format: yaml
  label: Regal Call Handoffs API
  slug: regal-ai-call-handoffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-ai-call-handoffs-api-openapi.yml
authorization_urls:
- https://mcp.regal.ai/v1/external-mcp/authorize
description: ''
docs: https://developer.regal.ai/docs/regal-mcp
flows:
- authorizationCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Regal Ai Scopes
name_suffix: OAuth Scopes
note: Regal's REST APIs are API-key only and have no scope surface at all — the OpenAPI securityScheme is a single apiKey in the Authorization header, and derive-oauth-scopes.py correctly finds zero oauth2 schemes across every spec in this repo. The OAuth surface belongs entirely to the hosted MCP server at mcp.regal.ai, which advertises RFC 8414 authorization-server metadata anonymously. The scopes below are read verbatim from that metadata; they are OIDC identity scopes, not Regal permission scopes. Authorization is brand-scoped by the authenticated Okta identity rather than by requested scope, so there is no per-resource scope catalogue to capture. Do not read this file as evidence of a fine-grained permission model — it is evidence of an OIDC login boundary in front of 60 MCP tools.
overview: 'Regal publishes 4 OAuth 2.0 scopes via the authorizationCode and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Regal API on a user''s behalf.


  Tokens are issued from https://mcp.regal.ai/v1/external-mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Regal
provider_slug: regal-ai
schemes:
- code_challenge_methods:
  - S256
  dynamic_client_registration: https://mcp.regal.ai/v1/external-mcp/register
  flows:
  - authorizationUrl: https://mcp.regal.ai/v1/external-mcp/authorize
    flow: authorizationCode
    revocationUrl: https://mcp.regal.ai/v1/external-mcp/revoke
    tokenUrl: https://mcp.regal.ai/v1/external-mcp/token
  - flow: refreshToken
    tokenUrl: https://mcp.regal.ai/v1/external-mcp/token
  identity_provider: Okta
  issuer: https://mcp.regal.ai/
  name: RegalMCPOAuth
  source: https://mcp.regal.ai/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC authentication of the Regal user behind the MCP client.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated Regal user.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim for the authenticated Regal user.
  flows:
  - authorizationCode
  scope: email
- description: Refresh-token issuance so the MCP client can keep a session without re-prompting.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: regal-ai-scopes
source_filename: regal-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.regal.ai/.well-known/oauth-authorization-server\ndocs: https://developer.regal.ai/docs/regal-mcp\nnote: >-\n  Regal's REST APIs are API-key only and have no scope surface at all — the OpenAPI\n  securityScheme is a single apiKey in the Authorization header, and derive-oauth-scopes.py\n  correctly finds zero oauth2 schemes across every spec in this repo. The OAuth surface\n  belongs entirely to the hosted MCP server at mcp.regal.ai, which advertises RFC 8414\n  authorization-server metadata anonymously. The scopes below are read verbatim from that\n  metadata; they are OIDC identity scopes, not Regal permission scopes. Authorization is\n  brand-scoped by the authenticated Okta identity rather than by requested scope, so there\n  is no per-resource scope catalogue to capture. Do not read this file as evidence of a\n  fine-grained permission model — it is evidence of an OIDC login boundary in front of 60\n  MCP tools.\n\
  applies_to: mcp/regal-ai-mcp.yml\nschemes:\n  - name: RegalMCPOAuth\n    type: oauth2\n    source: https://mcp.regal.ai/.well-known/oauth-authorization-server\n    issuer: https://mcp.regal.ai/\n    identity_provider: Okta\n    dynamic_client_registration: https://mcp.regal.ai/v1/external-mcp/register\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.regal.ai/v1/external-mcp/authorize\n        tokenUrl: https://mcp.regal.ai/v1/external-mcp/token\n        revocationUrl: https://mcp.regal.ai/v1/external-mcp/revoke\n      - flow: refreshToken\n        tokenUrl: https://mcp.regal.ai/v1/external-mcp/token\nscopes:\n  - scope: openid\n    description: OIDC authentication of the Regal user behind the MCP client.\n    flows: [authorizationCode]\n    sources: [https://mcp.regal.ai/.well-known/oauth-authorization-server]\n  - scope: profile\n    description:\
  \ Basic profile claims for the authenticated Regal user.\n    flows: [authorizationCode]\n    sources: [https://mcp.regal.ai/.well-known/oauth-authorization-server]\n  - scope: email\n    description: Email claim for the authenticated Regal user.\n    flows: [authorizationCode]\n    sources: [https://mcp.regal.ai/.well-known/oauth-authorization-server]\n  - scope: offline_access\n    description: Refresh-token issuance so the MCP client can keep a session without re-prompting.\n    flows: [authorizationCode, refreshToken]\n    sources: [https://mcp.regal.ai/.well-known/oauth-authorization-server]\nresource:\n  resource: https://mcp.regal.ai/v1/external-mcp/mcp\n  authorization_servers: [https://mcp.regal.ai/]\n  bearer_methods_supported: [header]\n  source: https://mcp.regal.ai/.well-known/oauth-protected-resource/v1/external-mcp/mcp\nauthorization_model:\n  boundary: brand\n  detail: >-\n    Regal states every MCP tool is scoped to the authenticated brand and that no\n    cross-tenant\
  \ access is possible. Write tools additionally require explicit human\n    approval at the client and only save drafts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/scopes/regal-ai-scopes.yml
summary_line: 4 scopes · authorizationCode/refreshToken
tags:
- Artificial Intelligence
- AI Agents
- Voice AI
- Contact Center
- Outbound Calling
- Inbound Calling
- Phone Agents
- SMS
- Chat
- WebRTC
- Conversation Intelligence
- Journey Orchestration
- Branded Caller ID
- CCaaS
- CPaaS
- Sales Dialer
- Customer Engagement
token_urls:
- https://mcp.regal.ai/v1/external-mcp/token
---
