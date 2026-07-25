---
authorization_urls:
- https://auth.honeyinsurance.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Honey Insurance Scopes
name_suffix: OAuth Scopes
note: These are the scopes advertised by Honey Insurance's Auth0 custom-domain tenant, harvested anonymously from OIDC discovery on 2026-07-25. They are the stock OpenID Connect profile claims that Auth0 ships by default — there is no insurance-domain scope (no quote, bind, policy, claim or document scope), no published API audience to request an access token for, and no developer credential path. Treat this as consumer account sign-in, not an API authorization surface. Nothing here was derived from an OpenAPI definition, because Honey publishes none.
overview: 'Honey Insurance publishes 14 OAuth 2.0 scopes via the authorizationCode, implicit, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Honey Insurance API on a user''s behalf.


  Tokens are issued from https://auth.honeyinsurance.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Honey Insurance
provider_slug: honey-insurance
schemes:
- flows:
  - authorizationUrl: https://auth.honeyinsurance.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.honeyinsurance.com/oauth/token
  - authorizationUrl: https://auth.honeyinsurance.com/authorize
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://auth.honeyinsurance.com/oauth/token
  - deviceAuthorizationUrl: https://auth.honeyinsurance.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.honeyinsurance.com/oauth/token
  issuer: https://auth.honeyinsurance.com/
  name: Auth0OIDC
  source: well-known/honey-insurance-openid-configuration.json
  type: openIdConnect
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- email_verified
- address
- phone
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
scopes:
- description: Request an ID token — the base OpenID Connect scope.
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Request a refresh token for long-lived sessions.
  flows: []
  scope: offline_access
- description: Access the end user's email address.
  flows: []
  scope: email
- description: Access whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: Access the end user's postal address claim.
  flows: []
  scope: address
- description: Access the end user's phone number claim.
  flows: []
  scope: phone
- description: Access the end user's full name.
  flows: []
  scope: name
- description: Access the end user's given name.
  flows: []
  scope: given_name
- description: Access the end user's family name.
  flows: []
  scope: family_name
- description: Access the end user's nickname.
  flows: []
  scope: nickname
- description: Access the end user's profile picture URL.
  flows: []
  scope: picture
- description: Access the account creation timestamp.
  flows: []
  scope: created_at
- description: Access the linked identity providers on the Auth0 user record.
  flows: []
  scope: identities
slug: honey-insurance-scopes
source_filename: honey-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.honeyinsurance.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes advertised by Honey Insurance's Auth0 custom-domain\n  tenant, harvested anonymously from OIDC discovery on 2026-07-25. They are the\n  stock OpenID Connect profile claims that Auth0 ships by default — there is no\n  insurance-domain scope (no quote, bind, policy, claim or document scope), no\n  published API audience to request an access token for, and no developer\n  credential path. Treat this as consumer account sign-in, not an API\n  authorization surface. Nothing here was derived from an OpenAPI definition,\n  because Honey publishes none.\nschemes:\n- name: Auth0OIDC\n  type: openIdConnect\n  source: well-known/honey-insurance-openid-configuration.json\n  issuer: https://auth.honeyinsurance.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.honeyinsurance.com/authorize\n    tokenUrl:\
  \ https://auth.honeyinsurance.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://auth.honeyinsurance.com/authorize\n  - flow: clientCredentials\n    tokenUrl: https://auth.honeyinsurance.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.honeyinsurance.com/oauth/device/code\n    tokenUrl: https://auth.honeyinsurance.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token — the base OpenID Connect scope.\n  kind: oidc-standard\n- scope: profile\n  description: Access the end user's default profile claims.\n  kind: oidc-standard\n- scope: offline_access\n  description: Request a refresh token for long-lived sessions.\n  kind: oidc-standard\n- scope: email\n  description: Access the end user's email address.\n  kind: oidc-standard\n- scope: email_verified\n  description: Access whether the end user's email address has been verified.\n  kind: oidc-standard\n- scope: address\n  description: Access the end user's postal address\
  \ claim.\n  kind: oidc-standard\n- scope: phone\n  description: Access the end user's phone number claim.\n  kind: oidc-standard\n- scope: name\n  description: Access the end user's full name.\n  kind: profile-claim\n- scope: given_name\n  description: Access the end user's given name.\n  kind: profile-claim\n- scope: family_name\n  description: Access the end user's family name.\n  kind: profile-claim\n- scope: nickname\n  description: Access the end user's nickname.\n  kind: profile-claim\n- scope: picture\n  description: Access the end user's profile picture URL.\n  kind: profile-claim\n- scope: created_at\n  description: Access the account creation timestamp.\n  kind: auth0-extension\n- scope: identities\n  description: Access the linked identity providers on the Auth0 user record.\n  kind: auth0-extension\ndomain_scopes:\n  present: false\n  note: >-\n    No quote, bind, issue, policy, claim (FNOL), document or payment scope is\n    published. The four insurance verbs exist only as\
  \ consumer web and telephone\n    journeys — see review.yml findings.insuranceVerbs.\nrelated:\n  authentication: authentication/honey-insurance-authentication.yml\n  well_known: well-known/honey-insurance-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honey-insurance/refs/heads/main/scopes/honey-insurance-scopes.yml
summary_line: 14 scopes · authorizationCode/implicit/clientCredentials/deviceCode
tags:
- Insurance
- Australia
- Insurtech
- Home Insurance
- Property and Casualty
- Personal Lines
- Direct to Consumer
- Embedded Insurance
- Smart Home
- Claims
- Underwriting
token_urls:
- https://auth.honeyinsurance.com/oauth/token
---
