---
authorization_urls:
- https://auth.cytora.com/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cytora Scopes
name_suffix: OAuth Scopes
note: Every scope below is a stock OpenID Connect / Auth0 identity scope advertised by the tenant's discovery document. Cytora publishes NO product- or resource-level scopes anonymously (nothing of the form risk:read, submission:write, claim:create). Machine-to-machine access to api.cytora.com uses the client_credentials grant against an API audience that is provisioned per customer contract and is not disclosed publicly, so the real authorization surface cannot be enumerated without provisioned credentials.
overview: 'Cytora publishes 14 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cytora API on a user''s behalf.


  Tokens are issued from https://auth.cytora.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cytora
provider_slug: cytora
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.cytora.com/oauth/token
  - authorizationUrl: https://auth.cytora.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.cytora.com/oauth/token
  issuer: https://auth.cytora.com/
  name: CytoraOAuth2
  source: well-known/cytora-openid-configuration.json
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
- description: Request an ID token (OpenID Connect)
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Full name claim
  flows:
  - authorizationCode
  scope: name
- description: Given name claim
  flows:
  - authorizationCode
  scope: given_name
- description: Family name claim
  flows:
  - authorizationCode
  scope: family_name
- description: Nickname claim
  flows:
  - authorizationCode
  scope: nickname
- description: Email address claim
  flows:
  - authorizationCode
  scope: email
- description: Email verification state claim
  flows:
  - authorizationCode
  scope: email_verified
- description: Profile picture claim
  flows:
  - authorizationCode
  scope: picture
- description: Account creation timestamp claim
  flows:
  - authorizationCode
  scope: created_at
- description: Linked identity provider records claim
  flows:
  - authorizationCode
  scope: identities
- description: Phone number claim
  flows:
  - authorizationCode
  scope: phone
- description: Address claim
  flows:
  - authorizationCode
  scope: address
slug: cytora-scopes
source_filename: cytora-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.cytora.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Every scope below is a stock OpenID Connect / Auth0 identity scope advertised\n  by the tenant's discovery document. Cytora publishes NO product- or\n  resource-level scopes anonymously (nothing of the form risk:read,\n  submission:write, claim:create). Machine-to-machine access to api.cytora.com\n  uses the client_credentials grant against an API audience that is provisioned\n  per customer contract and is not disclosed publicly, so the real authorization\n  surface cannot be enumerated without provisioned credentials.\nschemes:\n- name: CytoraOAuth2\n  source: well-known/cytora-openid-configuration.json\n  issuer: https://auth.cytora.com/\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cytora.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cytora.com/authorize\n    tokenUrl: https://auth.cytora.com/oauth/token\n\
  scopes:\n- scope: openid\n  description: Request an ID token (OpenID Connect)\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: name\n  description: Full name claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: given_name\n  description: Given name claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: family_name\n  description: Family name claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: nickname\n  description: Nickname claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n\
  - scope: email\n  description: Email address claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: email_verified\n  description: Email verification state claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: picture\n  description: Profile picture claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: created_at\n  description: Account creation timestamp claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: identities\n  description: Linked identity provider records claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: phone\n  description: Phone number claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n- scope: address\n  description: Address claim\n  flows: [authorizationCode]\n  sources: [well-known/cytora-openid-configuration.json]\n\
  product_scopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cytora/refs/heads/main/scopes/cytora-scopes.yml
summary_line: 14 scopes · clientCredentials/authorizationCode
tags:
- Insurance
- United Kingdom
- Insurtech
- Commercial Insurance
- Underwriting
- Claims
- Risk Data
- Property and Casualty
- Reinsurance
- Broker
- Submission Intake
- Document AI
token_urls:
- https://auth.cytora.com/oauth/token
---
