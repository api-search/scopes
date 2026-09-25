---
authorization_urls:
- https://www.sidecare.com/accounts/oauth/authorizations
description: ''
docs: https://www.sidecare.com/connexion-hub
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sidecare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SideCare publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SideCare API on a user''s behalf.


  Tokens are issued from https://www.sidecare.com/accounts/oauth/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SideCare
provider_slug: sidecare
schemes:
- flows:
  - authorizationUrl: https://www.sidecare.com/accounts/oauth/authorizations
    flow: authorizationCode
    tokenUrl: https://www.sidecare.com/accounts/oauth/tokens
  name: sidecare-oidc
  source: well-known/sidecare-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- profile
- email
- address
scopes:
- description: Required OpenID Connect scope; returns the subject identifier and an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the end-user's profile claims (name, given_name, family_name, birthdate, phone_number).
  flows:
  - authorizationCode
  scope: profile
- description: Access to the end-user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Access to the end-user's postal address claim.
  flows:
  - authorizationCode
  scope: address
slug: sidecare-scopes
source_filename: sidecare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.sidecare.com/.well-known/openid-configuration\ndocs: https://www.sidecare.com/connexion-hub\nschemes:\n- name: sidecare-oidc\n  type: openIdConnect\n  source: well-known/sidecare-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.sidecare.com/accounts/oauth/authorizations\n    tokenUrl: https://www.sidecare.com/accounts/oauth/tokens\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; returns the subject identifier and an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/sidecare-openid-configuration.json]\n- scope: profile\n  description: Access to the end-user's profile claims (name, given_name, family_name, birthdate, phone_number).\n  flows: [authorizationCode]\n  sources: [well-known/sidecare-openid-configuration.json]\n- scope: email\n  description: Access to the end-user's email and email_verified claims.\n  flows: [authorizationCode]\n\
  \  sources: [well-known/sidecare-openid-configuration.json]\n- scope: address\n  description: Access to the end-user's postal address claim.\n  flows: [authorizationCode]\n  sources: [well-known/sidecare-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidecare/refs/heads/main/scopes/sidecare-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Financial Services
- Insurance
- Insurtech
- Health Insurance
- Employee Benefits
- Human Resources
- HRIS
- France
- OpenID Connect
token_urls:
- https://www.sidecare.com/accounts/oauth/tokens
---
