---
authorization_urls:
- https://id.nib.com.au/authorize
- https://id.nib.co.nz/authorize
description: ''
docs: https://id.nib.com.au/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Nib Health Funds Scopes
name_suffix: OAuth Scopes
note: 'Not derived from an OpenAPI — nib publishes none. These are the scopes_supported values read verbatim from the anonymously-readable OpenID Connect discovery documents of nib''s Auth0 member identity tenants. Both the Australian (id.nib.com.au) and New Zealand (id.nib.co.nz) tenants advertise the identical set. Every scope below is a standard OIDC / Auth0 identity scope. nib publishes NO product scopes — nothing for policies, claims, quotes, members, providers, or partner data. That is the honest shape of this provider''s OAuth surface: a consumer sign-in tenant, not a partner API authorization server.'
overview: 'nib publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the nib API on a user''s behalf.


  Tokens are issued from https://id.nib.com.au/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: nib
provider_slug: nib-health-funds
schemes:
- flows:
  - authorizationUrl: https://id.nib.com.au/authorize
    flow: authorizationCode
    tokenUrl: https://id.nib.com.au/oauth/token
  - flow: clientCredentials
    tokenUrl: https://id.nib.com.au/oauth/token
  - authorizationUrl: https://id.nib.com.au/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://id.nib.com.au/oauth/device/code
    flow: deviceCode
    tokenUrl: https://id.nib.com.au/oauth/token
  issuer: https://id.nib.com.au/
  name: nib Australia member identity (Auth0 OIDC)
  source: well-known/nib-health-funds-openid-configuration.json
- flows:
  - authorizationUrl: https://id.nib.co.nz/authorize
    flow: authorizationCode
    tokenUrl: https://id.nib.co.nz/oauth/token
  issuer: https://id.nib.co.nz/
  name: nib New Zealand member identity (Auth0 OIDC)
  source: well-known/nib-health-funds-nz-openid-configuration.json
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
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows: []
  scope: profile
- description: Issue a refresh token so the client can renew access without the member re-authenticating.
  flows: []
  scope: offline_access
- description: The member's full name claim.
  flows: []
  scope: name
- description: The member's given name claim.
  flows: []
  scope: given_name
- description: The member's family name claim.
  flows: []
  scope: family_name
- description: The member's nickname claim.
  flows: []
  scope: nickname
- description: The member's email address claim.
  flows: []
  scope: email
- description: Whether the member's email address has been verified.
  flows: []
  scope: email_verified
- description: The member's profile picture claim.
  flows: []
  scope: picture
- description: When the member's identity record was created.
  flows: []
  scope: created_at
- description: Linked identity provider connections for the member (Auth0 identities array).
  flows: []
  scope: identities
- description: The member's phone number claim.
  flows: []
  scope: phone
- description: The member's address claim.
  flows: []
  scope: address
slug: nib-health-funds-scopes
source_filename: nib-health-funds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://id.nib.com.au/.well-known/openid-configuration\ndocs: https://id.nib.com.au/.well-known/openid-configuration\nnote: |\n  Not derived from an OpenAPI — nib publishes none. These are the\n  scopes_supported values read verbatim from the anonymously-readable OpenID\n  Connect discovery documents of nib's Auth0 member identity tenants. Both the\n  Australian (id.nib.com.au) and New Zealand (id.nib.co.nz) tenants advertise\n  the identical set.\n\n  Every scope below is a standard OIDC / Auth0 identity scope. nib publishes NO\n  product scopes — nothing for policies, claims, quotes, members, providers, or\n  partner data. That is the honest shape of this provider's OAuth surface: a\n  consumer sign-in tenant, not a partner API authorization server.\nschemes:\n- name: nib Australia member identity (Auth0 OIDC)\n  source: well-known/nib-health-funds-openid-configuration.json\n  issuer: https://id.nib.com.au/\n  flows:\n  -\
  \ flow: authorizationCode\n    authorizationUrl: https://id.nib.com.au/authorize\n    tokenUrl: https://id.nib.com.au/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://id.nib.com.au/oauth/token\n  - flow: implicit\n    authorizationUrl: https://id.nib.com.au/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://id.nib.com.au/oauth/device/code\n    tokenUrl: https://id.nib.com.au/oauth/token\n- name: nib New Zealand member identity (Auth0 OIDC)\n  source: well-known/nib-health-funds-nz-openid-configuration.json\n  issuer: https://id.nib.co.nz/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.nib.co.nz/authorize\n    tokenUrl: https://id.nib.co.nz/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token — the base OpenID Connect scope.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: profile\n  description: Basic\
  \ profile claims (name, given_name, family_name, nickname, picture).\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without the member\n    re-authenticating.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: name\n  description: The member's full name claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: given_name\n  description: The member's given name claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: family_name\n  description: The member's family name claim.\n \
  \ category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: nickname\n  description: The member's nickname claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: email\n  description: The member's email address claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: email_verified\n  description: Whether the member's email address has been verified.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: picture\n  description: The member's profile picture claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n\
  - scope: created_at\n  description: When the member's identity record was created.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: identities\n  description: Linked identity provider connections for the member (Auth0 identities\n    array).\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: phone\n  description: The member's phone number claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\n- scope: address\n  description: The member's address claim.\n  category: identity\n  sources: [well-known/nib-health-funds-openid-configuration.json, well-known/nib-health-funds-nz-openid-configuration.json]\nproduct_scopes:\n  published: false\n  note: No policy, claims, quote, member-data,\
  \ provider, or partner scopes are published\n    by nib on any anonymously reachable surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nib-health-funds/refs/heads/main/scopes/nib-health-funds-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/implicit/deviceCode
tags:
- Insurance
- Australia
- Health Insurance
- Carrier
- Claims
- Private Health Insurance
- Travel Insurance
- New Zealand
- NDIS
- Partner Gated
token_urls:
- https://id.nib.com.au/oauth/token
- https://id.nib.co.nz/oauth/token
---
