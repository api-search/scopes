---
authorization_urls:
- https://apis.vitality.co.uk/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Vitality Uk Scopes
name_suffix: OAuth Scopes
note: Only the OpenID Connect standard scopes are advertised in Vitality's public discovery document. Any business scopes on the partner APIs behind the apis.vitality.co.uk gateway (WSO2 API Manager scopes are bound per-API in the publisher) are not published anonymously and cannot be enumerated without partner-issued credentials. The list below is exactly what the provider publishes — it is not a complete picture of the partner authorization surface.
overview: 'Vitality publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vitality API on a user''s behalf.


  Tokens are issued from https://apis.vitality.co.uk/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vitality
provider_slug: vitality-uk
schemes:
- flows:
  - authorizationUrl: https://apis.vitality.co.uk/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://apis.vitality.co.uk/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://apis.vitality.co.uk/oauth2/token
  issuer: https://apis.vitality.co.uk/oauth2/token
  name: WSO2 API Manager OAuth2
  source: https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration
scope_count: 5
scope_names:
- openid
- profile
- email
- phone
- address
scopes:
- description: Request an OpenID Connect ID token alongside the access token. This is the scope Vitality's own first-party Workplace Connect adviser application requests.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC profile claims (name, given_name, family_name, preferred_username, picture, locale, updated_at and related).
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Standard OIDC phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Standard OIDC address claim (formatted, street_address, locality, region, postal_code, country).
  flows:
  - authorizationCode
  scope: address
slug: vitality-uk-scopes
source_filename: vitality-uk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Only the OpenID Connect standard scopes are advertised in Vitality's public\n  discovery document. Any business scopes on the partner APIs behind the\n  apis.vitality.co.uk gateway (WSO2 API Manager scopes are bound per-API in the\n  publisher) are not published anonymously and cannot be enumerated without\n  partner-issued credentials. The list below is exactly what the provider\n  publishes — it is not a complete picture of the partner authorization surface.\nschemes:\n- name: WSO2 API Manager OAuth2\n  source: https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration\n  issuer: https://apis.vitality.co.uk/oauth2/token\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apis.vitality.co.uk/oauth2/authorize\n    tokenUrl: https://apis.vitality.co.uk/oauth2/token\n  - flow: clientCredentials\n\
  \    tokenUrl: https://apis.vitality.co.uk/oauth2/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token alongside the access token. This\n    is the scope Vitality's own first-party Workplace Connect adviser application\n    requests.\n  flows: [authorizationCode]\n  sources: [https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration]\n- scope: profile\n  description: Standard OIDC profile claims (name, given_name, family_name,\n    preferred_username, picture, locale, updated_at and related).\n  flows: [authorizationCode]\n  sources: [https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration]\n- scope: email\n  description: Standard OIDC email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration]\n- scope: phone\n  description: Standard OIDC phone_number and phone_number_verified claims.\n  flows: [authorizationCode]\n  sources: [https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration]\n\
  - scope: address\n  description: Standard OIDC address claim (formatted, street_address, locality,\n    region, postal_code, country).\n  flows: [authorizationCode]\n  sources: [https://apis.vitality.co.uk/oauth2/token/.well-known/openid-configuration]\nnot_published:\n  business_scopes: true\n  note: No member, policy, quote, claim or benefit scope is advertised publicly.\n    Vitality-specific identity claims (memberID, entityID, partyID, roles, groups)\n    appear in claims_supported, implying member-level authorization exists behind\n    the gate, but the scopes that gate it are partner-issued.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitality-uk/refs/heads/main/scopes/vitality-uk-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Insurance
- United Kingdom
- Health Insurance
- Life Insurance
- Employee Benefits
- Carrier
- Policy Administration
- Underwriting
- Partner Gated
token_urls:
- https://apis.vitality.co.uk/oauth2/token
---
