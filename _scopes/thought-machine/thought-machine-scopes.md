---
authorization_urls:
- https://auth.thoughtmachine.net/application/o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Thought Machine Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Thought Machine publishes 5 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Thought Machine API on a user''s behalf.


  Tokens are issued from https://auth.thoughtmachine.net/application/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Thought Machine
provider_slug: thought-machine
schemes:
- flows:
  - authorizationUrl: https://auth.thoughtmachine.net/application/o/authorize/
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.thoughtmachine.net/application/o/token/
  - flow: clientCredentials
    tokenUrl: https://auth.thoughtmachine.net/application/o/token/
  - deviceAuthorizationUrl: https://auth.thoughtmachine.net/application/o/device/
    flow: deviceCode
    tokenUrl: https://auth.thoughtmachine.net/application/o/token/
  issuer: https://auth.thoughtmachine.net/application/o/vault-portal/
  name: vault-portal-oidc
  source: well-known/thought-machine-openid-configuration.json
scope_count: 5
scope_names:
- openid
- email
- profile
- entitlements
- role
scopes:
- description: OpenID Connect authentication; issues an ID token for the portal user.
  flows:
  - authorizationCode
  scope: openid
- description: Release the user's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Release profile claims (name, given_name, preferred_username, nickname, groups).
  flows:
  - authorizationCode
  scope: profile
- description: Release the entitlements claim used to authorise portal/documentation access.
  flows:
  - authorizationCode
  scope: entitlements
- description: Release the roles claim for the authenticated portal user.
  flows:
  - authorizationCode
  scope: role
slug: thought-machine-scopes
source_filename: thought-machine-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://auth.thoughtmachine.net/application/o/vault-portal/.well-known/openid-configuration\nx-scope-of-this-file: >-\n  These are the OAuth 2.0 / OIDC scopes advertised by the Thought Machine identity provider\n  (auth.thoughtmachine.net, Authentik) for the vault-portal client — the SSO in front of the\n  Vault documentation and enablement portals. They are NOT the authorization scopes of the\n  Vault Core or Vault Payments data APIs, which are documented behind the partner login and\n  were not anonymously observable. No scope list has been invented.\nschemes:\n- name: vault-portal-oidc\n  source: well-known/thought-machine-openid-configuration.json\n  issuer: https://auth.thoughtmachine.net/application/o/vault-portal/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.thoughtmachine.net/application/o/authorize/\n    tokenUrl: https://auth.thoughtmachine.net/application/o/token/\n    pkce: S256\n  -\
  \ flow: clientCredentials\n    tokenUrl: https://auth.thoughtmachine.net/application/o/token/\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.thoughtmachine.net/application/o/device/\n    tokenUrl: https://auth.thoughtmachine.net/application/o/token/\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token for the portal user.\n  flows: [authorizationCode]\n  sources: [well-known/thought-machine-openid-configuration.json]\n- scope: email\n  description: Release the user's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/thought-machine-openid-configuration.json]\n- scope: profile\n  description: Release profile claims (name, given_name, preferred_username, nickname, groups).\n  flows: [authorizationCode]\n  sources: [well-known/thought-machine-openid-configuration.json]\n- scope: entitlements\n  description: Release the entitlements claim used to authorise portal/documentation access.\n  flows:\
  \ [authorizationCode]\n  sources: [well-known/thought-machine-openid-configuration.json]\n- scope: role\n  description: Release the roles claim for the authenticated portal user.\n  flows: [authorizationCode]\n  sources: [well-known/thought-machine-openid-configuration.json]\nclaims_supported:\n- sub\n- iss\n- aud\n- exp\n- iat\n- auth_time\n- acr\n- amr\n- nonce\n- email\n- email_verified\n- entitlements\n- roles\n- name\n- given_name\n- preferred_username\n- nickname\n- groups\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thought-machine/refs/heads/main/scopes/thought-machine-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Banking
- Core Banking
- Financial-Services
- Payments
- Cloud-Native
- Smart Contracts
- ISO 20022
- Ledger
- Fintech
- United Kingdom
token_urls:
- https://auth.thoughtmachine.net/application/o/token/
---
