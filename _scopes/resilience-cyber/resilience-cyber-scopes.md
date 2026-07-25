---
authorization_urls:
- https://auth.cyberresilience.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Resilience Cyber Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes the Auth0 tenant advertises in its discovery document and the scopes the portal actually requests on /authorize. They are OpenID Connect standard scopes and Auth0 profile-claim scopes — NOT product scopes. No insurance-domain scope surface (policy, quote, bind, claim, submission, portfolio) is published anywhere on the Resilience estate, and there is no scopes/permissions reference page to search: cyberresilience.com soft-404s every developer path. Absence of a domain scope model is the finding, not a gap in this harvest.'
overview: 'Resilience publishes 14 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Resilience API on a user''s behalf.


  Tokens are issued from https://auth.cyberresilience.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Resilience
provider_slug: resilience-cyber
schemes:
- flows:
  - authorizationUrl: https://auth.cyberresilience.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.cyberresilience.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.cyberresilience.com/oauth/token
  name: Auth0OIDC
  source: well-known/resilience-cyber-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Issue an ID token — required for OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Access the end user's email address.
  flows: []
  scope: email
- description: Access the end user's email verification status.
  flows: []
  scope: email_verified
- description: Issue a refresh token so the portal session can be renewed.
  flows: []
  scope: offline_access
- description: Access the end user's full name claim.
  flows: []
  scope: name
- description: Access the end user's given-name claim.
  flows: []
  scope: given_name
- description: Access the end user's family-name claim.
  flows: []
  scope: family_name
- description: Access the end user's nickname claim.
  flows: []
  scope: nickname
- description: Access the end user's profile picture claim.
  flows: []
  scope: picture
- description: Access the end user's account creation timestamp.
  flows: []
  scope: created_at
- description: Access the end user's linked identity providers.
  flows: []
  scope: identities
- description: Access the end user's phone number claim.
  flows: []
  scope: phone
- description: Access the end user's address claim.
  flows: []
  scope: address
slug: resilience-cyber-scopes
source_filename: resilience-cyber-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.cyberresilience.com/.well-known/openid-configuration\nlocal_copy: well-known/resilience-cyber-openid-configuration.json\nnote: >-\n  These are the scopes the Auth0 tenant advertises in its discovery document and\n  the scopes the portal actually requests on /authorize. They are OpenID Connect\n  standard scopes and Auth0 profile-claim scopes — NOT product scopes. No\n  insurance-domain scope surface (policy, quote, bind, claim, submission,\n  portfolio) is published anywhere on the Resilience estate, and there is no\n  scopes/permissions reference page to search: cyberresilience.com soft-404s\n  every developer path. Absence of a domain scope model is the finding, not a\n  gap in this harvest.\nschemes:\n- name: Auth0OIDC\n  source: well-known/resilience-cyber-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cyberresilience.com/authorize\n    tokenUrl: https://auth.cyberresilience.com/oauth/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://auth.cyberresilience.com/oauth/token\nrequested_by_portal:\n- openid\n- profile\n- email\n- offline_access\nscopes:\n- scope: openid\n  description: Issue an ID token — required for OpenID Connect authentication.\n  kind: oidc-standard\n  requested_by_portal: true\n- scope: profile\n  description: Access the end user's default profile claims.\n  kind: oidc-standard\n  requested_by_portal: true\n- scope: email\n  description: Access the end user's email address.\n  kind: oidc-standard\n  requested_by_portal: true\n- scope: email_verified\n  description: Access the end user's email verification status.\n  kind: auth0-claim\n- scope: offline_access\n  description: Issue a refresh token so the portal session can be renewed.\n  kind: oidc-standard\n  requested_by_portal: true\n- scope: name\n  description: Access the end user's full name claim.\n  kind: auth0-claim\n- scope: given_name\n  description: Access the end user's given-name claim.\n\
  \  kind: auth0-claim\n- scope: family_name\n  description: Access the end user's family-name claim.\n  kind: auth0-claim\n- scope: nickname\n  description: Access the end user's nickname claim.\n  kind: auth0-claim\n- scope: picture\n  description: Access the end user's profile picture claim.\n  kind: auth0-claim\n- scope: created_at\n  description: Access the end user's account creation timestamp.\n  kind: auth0-claim\n- scope: identities\n  description: Access the end user's linked identity providers.\n  kind: auth0-claim\n- scope: phone\n  description: Access the end user's phone number claim.\n  kind: oidc-standard\n- scope: address\n  description: Access the end user's address claim.\n  kind: oidc-standard\nproduct_scopes:\n  published: false\n  audience: https://api.prod.resilienceinsurance.app\n  note: >-\n    Any product-level scopes on the private audience would only be visible to an\n    authenticated broker or policyholder client. They cannot be enumerated\n    anonymously and\
  \ are not documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resilience-cyber/refs/heads/main/scopes/resilience-cyber-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials
tags:
- Insurance
- United States
- Cyber Insurance
- Property and Casualty
- Insurtech
- Underwriting
- Claims
- Risk Data
- Technology Errors and Omissions
- Broker
- Specialty Insurance
token_urls:
- https://auth.cyberresilience.com/oauth/token
---
