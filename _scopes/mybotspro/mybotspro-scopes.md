---
authorization_urls:
- https://auth.mybots.pro/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: probed
name: Mybotspro Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from `scopes_supported` in the provider's live OIDC discovery document. myBots publishes no scopes/permissions reference page, so there are no descriptions to enrich with — the descriptions below are the STANDARD OIDC/OAuth definitions of these registered scopes (RFC 6749 / OpenID Connect Core 1.0 §5.4), not claims about myBots-specific behavior. Every scope advertised is a standard one; myBots advertises NO product-specific scopes (nothing for agents, channels, conversations, contacts or billing), so an OAuth client cannot request least-privilege access to any myBots resource — only identity.
overview: 'Mybots.pro publishes 6 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mybots.pro API on a user''s behalf.


  Tokens are issued from https://auth.mybots.pro/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mybots.pro
provider_slug: mybotspro
schemes:
- flows:
  - authorizationUrl: https://auth.mybots.pro/connect/authorize
    flow: authorizationCode
    tokenUrl: https://auth.mybots.pro/connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.mybots.pro/connect/token
  - flow: password
    tokenUrl: https://auth.mybots.pro/connect/token
  name: OAuth2
  source: well-known/mybotspro-openid-configuration.json
scope_count: 6
scope_names:
- openid
- profile
- email
- phone
- offline_access
- roles
scopes:
- description: Standard OIDC scope requesting an ID token for the authenticated subject.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope for the end-user's default profile claims (name, family_name, picture, updated_at, and similar).
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope for the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC scope for the phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Standard OIDC scope requesting a refresh token so the client can obtain access tokens without the end-user present.
  flows:
  - authorizationCode
  scope: offline_access
- description: Role claims for the authenticated subject. Conventional in OpenIddict/ASP.NET Identity deployments; myBots publishes no enumeration of which roles exist.
  flows:
  - authorizationCode
  - clientCredentials
  scope: roles
slug: mybotspro-scopes
source_filename: mybotspro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://auth.mybots.pro/.well-known/openid-configuration\nnote: >-\n  Scopes are taken verbatim from `scopes_supported` in the provider's live OIDC discovery\n  document. myBots publishes no scopes/permissions reference page, so there are no\n  descriptions to enrich with — the descriptions below are the STANDARD OIDC/OAuth\n  definitions of these registered scopes (RFC 6749 / OpenID Connect Core 1.0 §5.4), not\n  claims about myBots-specific behavior. Every scope advertised is a standard one; myBots\n  advertises NO product-specific scopes (nothing for agents, channels, conversations,\n  contacts or billing), so an OAuth client cannot request least-privilege access to any\n  myBots resource — only identity.\ndocs: null\nschemes:\n- name: OAuth2\n  source: well-known/mybotspro-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mybots.pro/connect/authorize\n    tokenUrl: https://auth.mybots.pro/connect/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://auth.mybots.pro/connect/token\n  - flow: password\n    tokenUrl: https://auth.mybots.pro/connect/token\nscopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated subject.\n  standard: OpenID Connect Core 1.0\n  product_specific: false\n  flows: [authorizationCode]\n  sources: [well-known/mybotspro-openid-configuration.json]\n- scope: profile\n  description: >-\n    Standard OIDC scope for the end-user's default profile claims (name, family_name,\n    picture, updated_at, and similar).\n  standard: OpenID Connect Core 1.0 §5.4\n  product_specific: false\n  flows: [authorizationCode]\n  sources: [well-known/mybotspro-openid-configuration.json]\n- scope: email\n  description: Standard OIDC scope for the email and email_verified claims.\n  standard: OpenID Connect Core 1.0 §5.4\n  product_specific: false\n  flows: [authorizationCode]\n  sources: [well-known/mybotspro-openid-configuration.json]\n\
  - scope: phone\n  description: Standard OIDC scope for the phone_number and phone_number_verified claims.\n  standard: OpenID Connect Core 1.0 §5.4\n  product_specific: false\n  flows: [authorizationCode]\n  sources: [well-known/mybotspro-openid-configuration.json]\n- scope: offline_access\n  description: >-\n    Standard OIDC scope requesting a refresh token so the client can obtain access tokens\n    without the end-user present.\n  standard: OpenID Connect Core 1.0 §11\n  product_specific: false\n  flows: [authorizationCode]\n  sources: [well-known/mybotspro-openid-configuration.json]\n- scope: roles\n  description: >-\n    Role claims for the authenticated subject. Conventional in OpenIddict/ASP.NET Identity\n    deployments; myBots publishes no enumeration of which roles exist.\n  standard: null\n  product_specific: false\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/mybotspro-openid-configuration.json]\nclaims_supported: [aud, exp, iat, iss, sub]\nclaims_note:\
  \ >-\n  `claims_supported` lists only the five registered JWT claims. Despite advertising the\n  profile/email/phone scopes, the discovery document does not advertise the corresponding\n  claims (name, email, phone_number), so a client cannot tell from discovery what the\n  userinfo endpoint will actually return.\nsummary:\n  scope_count: 6\n  product_specific_scope_count: 0\n  standard_oidc_scope_count: 6\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mybotspro/refs/heads/main/scopes/mybotspro-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials/password
tags:
- Company
- AI Agents
- Conversational AI
- Messaging
- Chatbots
- Customer Support
- Sales Automation
- WhatsApp
- Telegram
- Instagram
- Omnichannel
- Lead Qualification
- OpenID Connect
token_urls:
- https://auth.mybots.pro/connect/token
---
