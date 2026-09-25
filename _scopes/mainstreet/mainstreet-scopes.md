---
authorization_urls:
- https://login.mainstreet.com/authorize
description: ''
docs: https://login.mainstreet.com/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Mainstreet Scopes
name_suffix: OAuth Scopes
note: These are the scopes the MainStreet identity host advertises in its OIDC discovery document (an Auth0 tenant). They are the standard OIDC scope set plus Auth0's per-claim scopes — MainStreet publishes no product-specific API scopes, because it publishes no public product API. Nothing below is inferred; every scope is transcribed verbatim from scopes_supported.
overview: 'MainStreet publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the MainStreet API on a user''s behalf.


  Tokens are issued from https://login.mainstreet.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MainStreet
provider_slug: mainstreet
schemes:
- flows:
  - authorizationUrl: https://login.mainstreet.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.mainstreet.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.mainstreet.com/oauth/token
  - authorizationUrl: https://login.mainstreet.com/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://login.mainstreet.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://login.mainstreet.com/oauth/token
  issuer: https://login.mainstreet.com/
  name: MainStreet OIDC (Auth0 tenant)
  source: well-known/mainstreet-openid-configuration.json
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
- description: Request an ID token — the base OpenID Connect scope.
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Issue a refresh token so the client can act after the access token expires.
  flows: []
  scope: offline_access
- description: The end user's full name claim.
  flows: []
  scope: name
- description: The end user's given name claim.
  flows: []
  scope: given_name
- description: The end user's family name claim.
  flows: []
  scope: family_name
- description: The end user's nickname claim.
  flows: []
  scope: nickname
- description: The end user's email address claim.
  flows: []
  scope: email
- description: Whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: The end user's profile picture URL claim.
  flows: []
  scope: picture
- description: When the end user's identity record was created.
  flows: []
  scope: created_at
- description: The linked identity providers on the end user's account.
  flows: []
  scope: identities
- description: The end user's phone number claim.
  flows: []
  scope: phone
- description: The end user's address claim.
  flows: []
  scope: address
slug: mainstreet-scopes
source_filename: mainstreet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://login.mainstreet.com/.well-known/openid-configuration\ndocs: https://login.mainstreet.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes the MainStreet identity host advertises in its OIDC\n  discovery document (an Auth0 tenant). They are the standard OIDC scope set plus\n  Auth0's per-claim scopes — MainStreet publishes no product-specific API scopes,\n  because it publishes no public product API. Nothing below is inferred; every\n  scope is transcribed verbatim from scopes_supported.\nschemes:\n- name: MainStreet OIDC (Auth0 tenant)\n  source: well-known/mainstreet-openid-configuration.json\n  issuer: https://login.mainstreet.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.mainstreet.com/authorize\n    tokenUrl: https://login.mainstreet.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.mainstreet.com/oauth/token\n  - flow: implicit\n    authorizationUrl:\
  \ https://login.mainstreet.com/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.mainstreet.com/oauth/device/code\n    tokenUrl: https://login.mainstreet.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token — the base OpenID Connect scope.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: profile\n  description: Access the end user's default profile claims.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can act after the access token expires.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: name\n  description: The end user's full name claim.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: given_name\n  description: The end user's given name claim.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: family_name\n  description: The end user's family name claim.\n\
  \  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: nickname\n  description: The end user's nickname claim.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: email\n  description: The end user's email address claim.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: email_verified\n  description: Whether the end user's email address has been verified.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: picture\n  description: The end user's profile picture URL claim.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: created_at\n  description: When the end user's identity record was created.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: identities\n  description: The linked identity providers on the end user's account.\n  sources: [well-known/mainstreet-openid-configuration.json]\n- scope: phone\n  description: The end user's phone number claim.\n  sources:\
  \ [well-known/mainstreet-openid-configuration.json]\n- scope: address\n  description: The end user's address claim.\n  sources: [well-known/mainstreet-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://login.mainstreet.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mainstreet/refs/heads/main/scopes/mainstreet-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/implicit/deviceCode
tags:
- Company
- Tax
- Tax Credits
- Accounting
- Financial Services
- Small Business
- Fintech
- Bookkeeping
- Compliance
- Payroll
token_urls:
- https://login.mainstreet.com/oauth/token
---
