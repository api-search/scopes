---
authorization_urls: []
description: ''
docs: https://login.meetelise.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Eliseai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EliseAI publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the EliseAI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EliseAI
provider_slug: eliseai
schemes:
- authorizationUrl: https://login.meetelise.com/authorize
  issuer: https://login.meetelise.com/
  name: OAuth2
  source: well-known/eliseai-openid-configuration.json
  tokenUrl: https://login.meetelise.com/oauth/token
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: OpenID Connect authentication (subject identifier)
  flows: []
  scope: openid
- description: Access to the user's default profile claims
  flows: []
  scope: profile
- description: Issue a refresh token for long-lived access
  flows: []
  scope: offline_access
- description: User's full name
  flows: []
  scope: name
- description: User's given (first) name
  flows: []
  scope: given_name
- description: User's family (last) name
  flows: []
  scope: family_name
- description: User's nickname
  flows: []
  scope: nickname
- description: User's email address
  flows: []
  scope: email
- description: Whether the user's email is verified
  flows: []
  scope: email_verified
- description: User's profile picture URL
  flows: []
  scope: picture
- description: Account creation timestamp
  flows: []
  scope: created_at
- description: Linked identity provider identities
  flows: []
  scope: identities
- description: User's phone number
  flows: []
  scope: phone
- description: User's address
  flows: []
  scope: address
slug: eliseai-scopes
source_filename: eliseai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://login.meetelise.com/.well-known/openid-configuration\ndocs: https://login.meetelise.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: well-known/eliseai-openid-configuration.json\n  issuer: https://login.meetelise.com/\n  authorizationUrl: https://login.meetelise.com/authorize\n  tokenUrl: https://login.meetelise.com/oauth/token\nscopes:\n- {scope: openid, description: OpenID Connect authentication (subject identifier)}\n- {scope: profile, description: Access to the user's default profile claims}\n- {scope: offline_access, description: Issue a refresh token for long-lived access}\n- {scope: name, description: User's full name}\n- {scope: given_name, description: User's given (first) name}\n- {scope: family_name, description: User's family (last) name}\n- {scope: nickname, description: User's nickname}\n- {scope: email, description: User's email address}\n- {scope: email_verified, description:\
  \ Whether the user's email is verified}\n- {scope: picture, description: User's profile picture URL}\n- {scope: created_at, description: Account creation timestamp}\n- {scope: identities, description: Linked identity provider identities}\n- {scope: phone, description: User's phone number}\n- {scope: address, description: User's address}\nnotes: >-\n  Standard OIDC scopes advertised by EliseAI's Auth0 tenant (scopes_supported in\n  the discovery document). These are the identity/login scopes; product/API\n  permission scopes for partner integrations are not published on a public surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliseai/refs/heads/main/scopes/eliseai-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Property Management
- Real Estate
- Healthcare
- Leasing
- Voice AI
- Automation
- CRM
token_urls: []
---
