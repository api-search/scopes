---
authorization_urls:
- https://clerk.voiceops.com/oauth/authorize
description: ''
docs: https://clerk.com/docs/oauth/scoped-access
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Voiceops Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VoiceOps publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the VoiceOps API on a user''s behalf.


  Tokens are issued from https://clerk.voiceops.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VoiceOps
provider_slug: voiceops
schemes:
- flows:
  - authorizationUrl: https://clerk.voiceops.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.voiceops.com/oauth/token
  issuer: https://clerk.voiceops.com
  name: clerkOAuth2
  source: well-known/voiceops-oauth-authorization-server.json
scope_count: 6
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
scopes:
- description: Issue an OpenID Connect ID token for the signed-in user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, picture, preferred_username).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Read the user's public metadata held by the identity provider.
  flows:
  - authorizationCode
  scope: public_metadata
- description: Read the user's private metadata held by the identity provider.
  flows:
  - authorizationCode
  scope: private_metadata
- description: Issue a refresh token so the client can act without the user present.
  flows:
  - authorizationCode
  scope: offline_access
slug: voiceops-scopes
source_filename: voiceops-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://clerk.voiceops.com/.well-known/oauth-authorization-server\ndocs: https://clerk.com/docs/oauth/scoped-access\ndocs_note: >-\n  The service_documentation URL in the authorization-server metadata points at\n  Clerk's own documentation, not at a VoiceOps-authored scope reference —\n  VoiceOps publishes none.\nscope_source_caveat: >-\n  IMPORTANT: these are the scopes advertised by the OpenID Connect / OAuth 2.0\n  provider that signs users in to the VoiceOps application\n  (clerk.voiceops.com, issuer https://clerk.voiceops.com, CNAME to\n  frontend-api.clerk.services). They are Clerk's platform scoped-access\n  vocabulary. They are NOT scopes on a VoiceOps business API, and they do NOT\n  govern the remote MCP server at mcp.voiceops.com, which uses an API key with\n  no scope surface at all.\nschemes:\n  - name: clerkOAuth2\n    source: well-known/voiceops-oauth-authorization-server.json\n    issuer: https://clerk.voiceops.com\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.voiceops.com/oauth/authorize\n        tokenUrl: https://clerk.voiceops.com/oauth/token\nscopes:\n  - scope: openid\n    description: Issue an OpenID Connect ID token for the signed-in user.\n    flows: [authorizationCode]\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n  - scope: profile\n    description: Basic profile claims (name, given_name, family_name, picture, preferred_username).\n    flows: [authorizationCode]\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n  - scope: email\n    description: Email address and email_verified claim.\n    flows: [authorizationCode]\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n  - scope: public_metadata\n    description: Read the user's public metadata held by the identity provider.\n    flows: [authorizationCode]\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n  - scope: private_metadata\n\
  \    description: Read the user's private metadata held by the identity provider.\n    flows: [authorizationCode]\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Issue a refresh token so the client can act without the user present.\n    flows: [authorizationCode]\n    sources: [well-known/voiceops-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voiceops/refs/heads/main/scopes/voiceops-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Ai Apps
- Conversation Intelligence
- Call Centers
- Sales Coaching
- Customer Experience
- Artificial Intelligence
- Speech Analytics
- Model Context Protocol
- Agents
token_urls:
- https://clerk.voiceops.com/oauth/token
---
