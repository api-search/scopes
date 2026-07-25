---
authorization_urls:
- https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/authorize
description: ''
docs: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/v2.0/.well-known/openid-configuration
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Caa Insurance Scopes
name_suffix: OAuth Scopes
note: CAA Insurance exposes no API and therefore no API authorization scopes. The only scope surface observable anywhere in the estate is the standard OpenID Connect scope set advertised by the Microsoft Entra External ID (CIAM) tenant that authenticates the CAA Broker Portal and CAA Club Group sign-in. These are identity scopes for signing a human in, not delegated permissions over insurance data — no quote, policy, billing, or claims scope exists publicly.
overview: 'CAA Insurance publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CAA Insurance API on a user''s behalf.


  Tokens are issued from https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CAA Insurance
provider_slug: caa-insurance
schemes:
- flows:
  - authorizationUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token
  - deviceAuthorizationUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/devicecode
    flow: deviceCode
    tokenUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token
  name: EntraExternalIdCIAM
  source: well-known/caa-insurance-openid-configuration.json
  type: openIdConnect
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Sign the user in and issue an ID token.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims (name, preferred_username).
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: The user's email claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token so the session can be renewed without re-prompting.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: caa-insurance-scopes
source_filename: caa-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: well-known/caa-insurance-openid-configuration.json\ndocs: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/v2.0/.well-known/openid-configuration\nnote: >-\n  CAA Insurance exposes no API and therefore no API authorization scopes. The\n  only scope surface observable anywhere in the estate is the standard OpenID\n  Connect scope set advertised by the Microsoft Entra External ID (CIAM) tenant\n  that authenticates the CAA Broker Portal and CAA Club Group sign-in. These are\n  identity scopes for signing a human in, not delegated permissions over\n  insurance data — no quote, policy, billing, or claims scope exists publicly.\nsurface: identity-provider\nschemes:\n- name: EntraExternalIdCIAM\n  type: openIdConnect\n  source: well-known/caa-insurance-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/authorize\n\
  \    tokenUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/devicecode\n    tokenUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token\nscopes:\n- scope: openid\n  description: Sign the user in and issue an ID token.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/caa-insurance-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims (name, preferred_username).\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/caa-insurance-openid-configuration.json]\n- scope: email\n  description: The user's email claim.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/caa-insurance-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the session can be renewed without\
  \ re-prompting.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/caa-insurance-openid-configuration.json]\nbusiness_scopes:\n  published: false\n  note: No quote, bind, policy, billing, or claims scope is published by CAA Insurance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caa-insurance/refs/heads/main/scopes/caa-insurance-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Insurance
- Canada
- Property and Casualty
- Auto Insurance
- Home Insurance
- Carrier
- Broker
- Personal Lines
- Telematics
- Partner Gated
- No Public API
token_urls:
- https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token
---
