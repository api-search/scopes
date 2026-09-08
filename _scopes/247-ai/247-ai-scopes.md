---
authorization_urls:
- https://login.247.ai/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 247 Ai Scopes
name_suffix: OAuth Scopes
note: '[24]7.ai publishes no OpenAPI and no public scopes/permissions reference page. These scopes were read from the live discovery documents served by login.247.ai, the Okta-hosted [24]7 Engagement Cloud SSO tenant. IMPORTANT PROVENANCE CAVEAT: the org authorization server additionally advertises 80 `okta.*` scopes. Those belong to Okta''s own Management API running on the tenant — they are Okta''s product surface, not a [24]7.ai product API scope catalog — and are therefore recorded below as a counted, attributed block rather than listed as [24]7.ai scopes. Only the standard OIDC scopes are attributable to the [24]7.ai sign-in surface itself.'
overview: '[24]7.ai publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the [24]7.ai API on a user''s behalf.


  Tokens are issued from https://login.247.ai/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: '[24]7.ai'
provider_slug: 247-ai
schemes:
- flows:
  - authorizationUrl: https://login.247.ai/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.247.ai/oauth2/v1/token
  issuer: https://login.247.ai
  name: '[24]7 Engagement Cloud SSO'
  source: well-known/247-ai-openid-configuration.json
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- groups
- offline_access
scopes:
- description: OpenID Connect sign-in; issues an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, preferred_username, locale, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: address claim.
  flows:
  - authorizationCode
  scope: address
- description: phone_number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Group memberships of the signed-in user.
  flows:
  - authorizationCode
  scope: groups
- description: Issues a refresh token.
  flows:
  - authorizationCode
  scope: offline_access
slug: 247-ai-scopes
source_filename: 247-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://login.247.ai/.well-known/oauth-authorization-server\nnote: >-\n  [24]7.ai publishes no OpenAPI and no public scopes/permissions reference page. These scopes\n  were read from the live discovery documents served by login.247.ai, the Okta-hosted [24]7\n  Engagement Cloud SSO tenant. IMPORTANT PROVENANCE CAVEAT: the org authorization server\n  additionally advertises 80 `okta.*` scopes. Those belong to Okta's own Management API\n  running on the tenant — they are Okta's product surface, not a [24]7.ai product API scope\n  catalog — and are therefore recorded below as a counted, attributed block rather than\n  listed as [24]7.ai scopes. Only the standard OIDC scopes are attributable to the [24]7.ai\n  sign-in surface itself.\nschemes:\n- name: '[24]7 Engagement Cloud SSO'\n  source: well-known/247-ai-openid-configuration.json\n  issuer: https://login.247.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.247.ai/oauth2/v1/authorize\n\
  \    tokenUrl: https://login.247.ai/oauth2/v1/token\nscopes:\n- {scope: openid, description: 'OpenID Connect sign-in; issues an ID token.', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\n- {scope: profile, description: 'Basic profile claims (name, preferred_username, locale, updated_at).', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\n- {scope: email, description: 'email and email_verified claims.', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\n- {scope: address, description: 'address claim.', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\n- {scope: phone, description: 'phone_number claim.', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\n- {scope: groups, description: 'Group memberships of the signed-in user.', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\n-\
  \ {scope: offline_access, description: 'Issues a refresh token.', flows: [authorizationCode], sources: [well-known/247-ai-openid-configuration.json]}\nnot_attributed_to_provider:\n  count: 80\n  prefix: 'okta.*'\n  owner: Okta\n  reason: >-\n    Okta Management API scopes (okta.users.*, okta.apps.*, okta.logs.read, …) advertised by\n    the tenant's org authorization server. They govern administration of the Okta tenant, not\n    a [24]7.ai product API, and are not counted as [24]7.ai scopes.\n  source: well-known/247-ai-oauth-authorization-server.json\nx-evidence:\n- {url: 'https://login.247.ai/.well-known/oauth-authorization-server', http_status: 200, fetched: '2026-09-05'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/247-ai/refs/heads/main/scopes/247-ai-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Customer Experience
- Conversational AI
- Contact Center
- Customer Service
- Chatbots
- CCaaS
- Artificial Intelligence
- Interaction Analytics
- Business Process Outsourcing
token_urls:
- https://login.247.ai/oauth2/v1/token
---
