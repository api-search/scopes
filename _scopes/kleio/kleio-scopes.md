---
authorization_urls:
- https://auth.kleio.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Kleio Scopes
name_suffix: OAuth Scopes
note: 'Kleio publishes no scopes or permissions reference. The scopes below are the scopes_supported array from the OpenID Connect discovery document served by Kleio''s Auth0 tenant — captured because it is the only published scope surface, but read it for what it is: these are the standard OIDC identity scopes an Auth0 tenant advertises by default, not Kleio product scopes. No scope governing the Kleio platform API itself (catalog, knowledge engine, agents, quoting, CRM write-back) is publicly named anywhere. Kleio''s own API gateway metadata at api.kleio.ai omits scopes_supported entirely.'
overview: 'Kleio publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kleio API on a user''s behalf.


  Tokens are issued from https://auth.kleio.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kleio
provider_slug: kleio
schemes:
- flows:
  - authorizationUrl: https://auth.kleio.ai/authorize
    flow: authorizationCode
    tokenUrl: https://auth.kleio.ai/oauth/token
  issuer: https://auth.kleio.ai/
  name: KleioOIDC
  source: https://auth.kleio.ai/.well-known/openid-configuration
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
- description: Request an ID token and authenticate the end user.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Issue a refresh token so the client can renew access without user interaction.
  flows: []
  scope: offline_access
- description: The user's email address.
  flows: []
  scope: email
- description: Whether the user's email address has been verified.
  flows: []
  scope: email_verified
- description: The user's full name.
  flows: []
  scope: name
- description: The user's given name.
  flows: []
  scope: given_name
- description: The user's family name.
  flows: []
  scope: family_name
- description: The user's nickname.
  flows: []
  scope: nickname
- description: URL of the user's profile picture.
  flows: []
  scope: picture
- description: The user's phone number.
  flows: []
  scope: phone
- description: The user's postal address.
  flows: []
  scope: address
- description: When the user record was created.
  flows: []
  scope: created_at
- description: Linked identity-provider records for the user.
  flows: []
  scope: identities
slug: kleio-scopes
source_filename: kleio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://auth.kleio.ai/.well-known/openid-configuration\nnote: 'Kleio publishes no scopes or permissions reference. The scopes below are the scopes_supported\n  array from the OpenID Connect discovery document served by Kleio''s Auth0 tenant — captured because it\n  is the only published scope surface, but read it for what it is: these are the standard OIDC identity\n  scopes an Auth0 tenant advertises by default, not Kleio product scopes. No scope governing the Kleio\n  platform API itself (catalog, knowledge engine, agents, quoting, CRM write-back) is publicly named\n  anywhere. Kleio''s own API gateway metadata at api.kleio.ai omits scopes_supported entirely.'\nschemes:\n- name: KleioOIDC\n  issuer: https://auth.kleio.ai/\n  source: https://auth.kleio.ai/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.kleio.ai/authorize\n    tokenUrl: https://auth.kleio.ai/oauth/token\n\
  scope_class: oidc-identity-only\nscopes:\n- scope: openid\n  description: Request an ID token and authenticate the end user.\n  standard: OpenID Connect Core 1.0\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  standard: OpenID Connect Core 1.0\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without user interaction.\n  standard: OpenID Connect Core 1.0\n- scope: email\n  description: The user's email address.\n  standard: OpenID Connect Core 1.0\n- scope: email_verified\n  description: Whether the user's email address has been verified.\n- scope: name\n  description: The user's full name.\n- scope: given_name\n  description: The user's given name.\n- scope: family_name\n  description: The user's family name.\n- scope: nickname\n  description: The user's nickname.\n- scope: picture\n  description: URL of the user's profile picture.\n- scope: phone\n  description: The user's phone number.\n- scope: address\n\
  \  description: The user's postal address.\n- scope: created_at\n  description: When the user record was created.\n- scope: identities\n  description: Linked identity-provider records for the user.\ngaps:\n- 'No product scopes published. A customer integrating the Kleio platform API cannot learn from any\n  public source what authorization a token carries or how least-privilege access would be requested.'\n- 'The api.kleio.ai RFC 8414 metadata declares no scopes_supported, so the resource server publishes no\n  scope vocabulary of its own.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kleio/refs/heads/main/scopes/kleio-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Company
- Ai Data
- Agentic Commerce
- AI Agents
- Enterprise Sales
- Conversational AI
- Knowledge Engine
- MCP
- Agent To Agent
- Retail
- Travel
- Real-Estate
- Automotive
- France
token_urls:
- https://auth.kleio.ai/oauth/token
---
