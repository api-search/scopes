---
authorization_urls:
- https://auth.partner.iralogix.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Iralogix Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IRALOGIX publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the IRALOGIX API on a user''s behalf.


  Tokens are issued from https://auth.partner.iralogix.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IRALOGIX
provider_slug: iralogix
schemes:
- flows:
  - authorizationUrl: https://auth.partner.iralogix.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.partner.iralogix.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.partner.iralogix.com/oauth/token
  - deviceAuthorizationUrl: https://auth.partner.iralogix.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.partner.iralogix.com/oauth/token
  issuer: https://auth.partner.iralogix.com/
  name: IRALOGIX Partner OIDC
  source: well-known/iralogix-openid-configuration.json
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
- description: Request an ID token — the base OpenID Connect scope.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated partner user.
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
- description: When the user record was created in the tenant.
  flows: []
  scope: created_at
- description: The linked identity providers for the user.
  flows: []
  scope: identities
slug: iralogix-scopes
source_filename: iralogix-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://auth.partner.iralogix.com/.well-known/openid-configuration\ndocs: null\nnotes: 'These are the scopes the IRALOGIX partner authorization server advertises in\n  its OIDC discovery document. They are the standard OpenID Connect scopes and Auth0\n  claim-scopes only — no IRALOGIX business scopes (accounts, contributions, distributions,\n  rollovers, trading) are published anonymously. Partner-facing resource scopes, if\n  any exist, are behind the gated documentation at docs.iralogix.com and would require\n  authenticated discovery to enumerate. Nothing here is inferred; the list is verbatim\n  from scopes_supported.'\nschemes:\n- name: IRALOGIX Partner OIDC\n  source: well-known/iralogix-openid-configuration.json\n  issuer: https://auth.partner.iralogix.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.partner.iralogix.com/authorize\n    tokenUrl: https://auth.partner.iralogix.com/oauth/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://auth.partner.iralogix.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.partner.iralogix.com/oauth/device/code\n    tokenUrl: https://auth.partner.iralogix.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token — the base OpenID Connect scope.\n  kind: oidc-standard\n- scope: profile\n  description: Basic profile claims for the authenticated partner user.\n  kind: oidc-standard\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without user interaction.\n  kind: oidc-standard\n- scope: email\n  description: The user's email address.\n  kind: oidc-standard\n- scope: email_verified\n  description: Whether the user's email address has been verified.\n  kind: claim-scope\n- scope: name\n  description: The user's full name.\n  kind: claim-scope\n- scope: given_name\n  description: The user's given name.\n  kind: claim-scope\n- scope: family_name\n\
  \  description: The user's family name.\n  kind: claim-scope\n- scope: nickname\n  description: The user's nickname.\n  kind: claim-scope\n- scope: picture\n  description: URL of the user's profile picture.\n  kind: claim-scope\n- scope: phone\n  description: The user's phone number.\n  kind: oidc-standard\n- scope: address\n  description: The user's postal address.\n  kind: oidc-standard\n- scope: created_at\n  description: When the user record was created in the tenant.\n  kind: claim-scope\n- scope: identities\n  description: The linked identity providers for the user.\n  kind: claim-scope\ngaps:\n- id: no-resource-scopes\n  note: No business/resource scopes are published. For a platform that markets API-driven\n    partner connectivity, publishing a scope reference (read/write per IRA domain object)\n    would be the single largest authorization-transparency improvement.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://auth.partner.iralogix.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  field: scopes_supported\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iralogix/refs/heads/main/scopes/iralogix-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Financial-Services
- Retirement
- IRA
- Recordkeeping
- Wealth Management
- Fintech
- Compliance
- White Label
- Retirement Technology
token_urls:
- https://auth.partner.iralogix.com/oauth/token
---
