---
authorization_urls:
- https://auth.artificialos.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Artificial Labs Scopes
name_suffix: OAuth Scopes
note: These are the scopes the Artificial Labs Auth0 tenant advertises in its anonymous discovery document — standard OpenID Connect scopes and claim-scopes only. No product or insurance-domain scopes (underwriting, placement, contract, submission, quote, bind) are published anywhere public; any API-level authorization model for Smart Underwriting, Smart Placement or Contract Builder lives behind the partner contract and cannot be harvested. The documentation client observed in the wild (docs.artificial.io via oauth2-proxy) requests only "openid profile email".
overview: 'Artificial Labs publishes 14 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Artificial Labs API on a user''s behalf.


  Tokens are issued from https://auth.artificialos.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Artificial Labs
provider_slug: artificial-labs
schemes:
- flows:
  - authorizationUrl: https://auth.artificialos.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.artificialos.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.artificialos.com/oauth/token
  issuer: https://auth.artificialos.com/
  name: Auth0 OpenID Connect
  source: well-known/artificial-labs-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- email
- offline_access
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token / OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture, created_at).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token.
  flows:
  - authorizationCode
  scope: offline_access
- description: name claim.
  flows: []
  scope: name
- description: given_name claim.
  flows: []
  scope: given_name
- description: family_name claim.
  flows: []
  scope: family_name
- description: nickname claim.
  flows: []
  scope: nickname
- description: email_verified claim.
  flows: []
  scope: email_verified
- description: picture claim.
  flows: []
  scope: picture
- description: created_at claim.
  flows: []
  scope: created_at
- description: Linked identity providers for the user.
  flows: []
  scope: identities
- description: phone_number claim.
  flows: []
  scope: phone
- description: address claim.
  flows: []
  scope: address
slug: artificial-labs-scopes
source_filename: artificial-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://auth.artificialos.com/.well-known/openid-configuration\nnote: |\n  These are the scopes the Artificial Labs Auth0 tenant advertises in its\n  anonymous discovery document — standard OpenID Connect scopes and claim-scopes\n  only. No product or insurance-domain scopes (underwriting, placement, contract,\n  submission, quote, bind) are published anywhere public; any API-level\n  authorization model for Smart Underwriting, Smart Placement or Contract Builder\n  lives behind the partner contract and cannot be harvested. The documentation\n  client observed in the wild (docs.artificial.io via oauth2-proxy) requests only\n  \"openid profile email\".\nschemes:\n- name: Auth0 OpenID Connect\n  source: well-known/artificial-labs-openid-configuration.json\n  issuer: https://auth.artificialos.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.artificialos.com/authorize\n    tokenUrl: https://auth.artificialos.com/oauth/token\n\
  \  - flow: clientCredentials\n    tokenUrl: https://auth.artificialos.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token / OpenID Connect authentication.\n  flows: [authorizationCode]\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture,\n    created_at).\n  flows: [authorizationCode]\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: email\n  description: Email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token.\n  flows: [authorizationCode]\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: name\n  description: name claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: given_name\n  description: given_name claim.\n  sources:\
  \ [well-known/artificial-labs-openid-configuration.json]\n- scope: family_name\n  description: family_name claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: nickname\n  description: nickname claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: email_verified\n  description: email_verified claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: picture\n  description: picture claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: created_at\n  description: created_at claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: identities\n  description: Linked identity providers for the user.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: phone\n  description: phone_number claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n- scope: address\n  description: address claim.\n  sources: [well-known/artificial-labs-openid-configuration.json]\n\
  observed_in_use:\n- client: docs.artificial.io oauth2-proxy\n  scope: openid profile email\ndomain_scopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artificial-labs/refs/heads/main/scopes/artificial-labs-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials
tags:
- Insurance
- United Kingdom
- Insurtech
- Underwriting
- Reinsurance
- Specialty Insurance
- London Market
- Lloyd's of London
- Brokers
- Policy Administration
- ACORD
- Algorithmic Underwriting
token_urls:
- https://auth.artificialos.com/oauth/token
---
