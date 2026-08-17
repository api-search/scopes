---
authorization_urls:
- https://crawler-api-auth.onclusive.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Airpr Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes the Onclusive developer-portal authorization server actually advertises in its OIDC discovery document. They are the four standard OpenID Connect scopes and nothing more — Onclusive has defined no custom resource-server scopes on this user pool, or has not exposed them in discovery. NOT derived from an OpenAPI: Onclusive publishes none. No API-permission or scope reference page exists on any public Onclusive URL, so there is no richer `docs:` to point at.'
overview: 'AirPR publishes 4 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AirPR API on a user''s behalf.


  Tokens are issued from https://crawler-api-auth.onclusive.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AirPR
provider_slug: airpr
schemes:
- flows:
  - authorizationUrl: https://crawler-api-auth.onclusive.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://crawler-api-auth.onclusive.com/oauth2/token
  - authorizationUrl: https://crawler-api-auth.onclusive.com/oauth2/authorize
    flow: implicit
  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T
  name: OnclusiveDeveloperPortalOIDC
  source: well-known/airpr-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: Standard OpenID Connect scope; requests an ID token identifying the authenticated developer-portal user.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Releases the user's email address and email_verified claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Releases the user's phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Releases the user's basic profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: profile
slug: airpr-scopes
source_filename: airpr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/openid-configuration\nnote: >-\n  These are the scopes the Onclusive developer-portal authorization server\n  actually advertises in its OIDC discovery document. They are the four standard\n  OpenID Connect scopes and nothing more — Onclusive has defined no custom\n  resource-server scopes on this user pool, or has not exposed them in\n  discovery. NOT derived from an OpenAPI: Onclusive publishes none. No\n  API-permission or scope reference page exists on any public Onclusive URL, so\n  there is no richer `docs:` to point at.\nschemes:\n- name: OnclusiveDeveloperPortalOIDC\n  type: openIdConnect\n  source: well-known/airpr-openid-configuration.json\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://crawler-api-auth.onclusive.com/oauth2/authorize\n    tokenUrl:\
  \ https://crawler-api-auth.onclusive.com/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://crawler-api-auth.onclusive.com/oauth2/authorize\nscopes:\n- scope: openid\n  description: >-\n    Standard OpenID Connect scope; requests an ID token identifying the\n    authenticated developer-portal user.\n  standard: true\n  flows: [authorizationCode, implicit]\n  sources: [well-known/airpr-openid-configuration.json]\n- scope: email\n  description: Releases the user's email address and email_verified claim.\n  standard: true\n  flows: [authorizationCode, implicit]\n  sources: [well-known/airpr-openid-configuration.json]\n- scope: phone\n  description: Releases the user's phone_number and phone_number_verified claims.\n  standard: true\n  flows: [authorizationCode, implicit]\n  sources: [well-known/airpr-openid-configuration.json]\n- scope: profile\n  description: Releases the user's basic profile claims.\n  standard: true\n  flows: [authorizationCode, implicit]\n  sources: [well-known/airpr-openid-configuration.json]\n\
  scope_count: 4\ncustom_scope_count: 0\nx-evidence:\n- url: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_F0XmSWr9T/.well-known/openid-configuration\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airpr/refs/heads/main/scopes/airpr-scopes.yml
summary_line: 4 scopes · authorizationCode/implicit
tags:
- Company
- Public Relations
- Media Intelligence
- Media Monitoring
- Analytics
- Communications
- Marketing
- PR Measurement
- Onclusive
token_urls:
- https://crawler-api-auth.onclusive.com/oauth2/token
---
