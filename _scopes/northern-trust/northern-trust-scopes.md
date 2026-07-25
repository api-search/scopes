---
authorization_urls:
- https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize
description: ''
docs: https://developer.ntrs.com/get-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Northern Trust Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Northern Trust publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Northern Trust API on a user''s behalf.


  Tokens are issued from https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Northern Trust
provider_slug: northern-trust
schemes:
- flows:
  - authorizationUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token
  name: NorthernTrustOIDC
  source: well-known/northern-trust-openid-configuration.json
scope_count: 10
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
- api.read
- aor.role
- interclient_access
scopes:
- description: OpenID Connect — issue an ID token identifying the authenticated principal.
  flows: []
  scope: openid
- description: Access to the principal's basic profile claims (name, etc.).
  flows: []
  scope: profile
- description: Access to the principal's email address claim.
  flows: []
  scope: email
- description: Access to the principal's address claim.
  flows: []
  scope: address
- description: Access to the principal's phone-number claim.
  flows: []
  scope: phone
- description: Issue a refresh token so the client can obtain new access tokens without re-prompting.
  flows: []
  scope: offline_access
- description: Okta device single-sign-on scope enabling native SSO across device apps.
  flows: []
  scope: device_sso
- description: Provider-defined. Read access to the Northern Trust API Store resources exposed through the enterprise gateway. (Inferred — no public gloss.)
  flows: []
  scope: api.read
- description: Provider-defined role/entitlement scope carried on the access token to convey the caller's authorized role for API-Store access. (Inferred — no public gloss.)
  flows: []
  scope: aor.role
- description: Provider-defined scope authorizing cross-client / delegated access between registered client applications. (Inferred — no public gloss.)
  flows: []
  scope: interclient_access
slug: northern-trust-scopes
source_filename: northern-trust-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/.well-known/openid-configuration\n  (scopes_supported, live Okta OIDC discovery)\ndocs: https://developer.ntrs.com/get-started\nnotes: >-\n  Scopes are read verbatim from the custom Okta authorization server's\n  scopes_supported. Northern Trust does not publish a public scope-reference page\n  (the developer portal is gated), so descriptions for the provider-defined\n  scopes are inferred conservatively and marked as such; the standard OIDC scopes\n  use their RFC-defined meaning. Okta platform scopes (okta.myAccount.*) are the\n  identity-provider's own account scopes, not API-Store product scopes, and are\n  omitted here.\nschemes:\n- name: NorthernTrustOIDC\n  source: well-known/northern-trust-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/authorize\n    tokenUrl: https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect — issue an ID token identifying the authenticated principal.\n  standard: true\n- scope: profile\n  description: Access to the principal's basic profile claims (name, etc.).\n  standard: true\n- scope: email\n  description: Access to the principal's email address claim.\n  standard: true\n- scope: address\n  description: Access to the principal's address claim.\n  standard: true\n- scope: phone\n  description: Access to the principal's phone-number claim.\n  standard: true\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without re-prompting.\n  standard: true\n- scope: device_sso\n  description: Okta device single-sign-on scope enabling native SSO across device apps.\n  standard: true\n- scope: api.read\n  description: >-\n    Provider-defined. Read access to the Northern Trust API Store resources\n    exposed through the enterprise gateway. (Inferred — no public gloss.)\n\
  \  standard: false\n- scope: aor.role\n  description: >-\n    Provider-defined role/entitlement scope carried on the access token to convey\n    the caller's authorized role for API-Store access. (Inferred — no public gloss.)\n  standard: false\n- scope: interclient_access\n  description: >-\n    Provider-defined scope authorizing cross-client / delegated access between\n    registered client applications. (Inferred — no public gloss.)\n  standard: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northern-trust/refs/heads/main/scopes/northern-trust-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Fortune 500
- Banking
- Wealth Management
- Asset Servicing
- Asset Management
- Financial Services
- United States
token_urls:
- https://login.ntrs.com/oauth2/aus1m4yuzpqNFht7o0h8/v1/token
---
