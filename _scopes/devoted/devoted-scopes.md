---
api_specs:
- filename: devoted-patient-access-openapi.json
  format: json
  label: Patient Access API
  slug: patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted/refs/heads/main/openapi/devoted-patient-access-openapi.json
authorization_urls: []
description: ''
docs: https://www.devoted.com/developers/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Devoted Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Devoted Health publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Devoted Health API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Devoted Health
provider_slug: devoted
schemes:
- authorizationUrl: https://login.devoted.com/authorize
  name: OpenIDConnect
  source: well-known/devoted-openid-configuration.json
  tokenUrl: https://login.devoted.com/oauth/token
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
- description: Authenticate the member and issue an ID token (OIDC core).
  flows: []
  scope: openid
- description: Access basic profile claims (name, nickname, picture, updated_at).
  flows: []
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Member's full name claim.
  flows: []
  scope: name
- description: Member's given (first) name claim.
  flows: []
  scope: given_name
- description: Member's family (last) name claim.
  flows: []
  scope: family_name
- description: Member's nickname claim.
  flows: []
  scope: nickname
- description: Member's email address claim.
  flows: []
  scope: email
- description: Whether the member's email address has been verified.
  flows: []
  scope: email_verified
- description: URL of the member's profile picture.
  flows: []
  scope: picture
- description: Timestamp the member's identity record was created.
  flows: []
  scope: created_at
- description: Linked identity provider records for the member.
  flows: []
  scope: identities
- description: Member's phone number claim.
  flows: []
  scope: phone
- description: Member's postal address claim.
  flows: []
  scope: address
slug: devoted-scopes
source_filename: devoted-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.devoted.com/.well-known/openid-configuration\ndocs: https://www.devoted.com/developers/\nnotes: >-\n  OpenID Connect scopes advertised by Devoted Health's Auth0 authorization\n  server (login.devoted.com), used for member authorization to the Patient Access\n  FHIR API. Scope list captured verbatim from the published discovery document\n  scopes_supported. Member authorization follows the OAuth 2.0 / OIDC pattern\n  required by the CMS Interoperability and Patient Access rule.\nschemes:\n- name: OpenIDConnect\n  source: well-known/devoted-openid-configuration.json\n  authorizationUrl: https://login.devoted.com/authorize\n  tokenUrl: https://login.devoted.com/oauth/token\nscopes:\n- scope: openid\n  description: Authenticate the member and issue an ID token (OIDC core).\n- scope: profile\n  description: Access basic profile claims (name, nickname, picture, updated_at).\n- scope: offline_access\n  description: Issue\
  \ a refresh token for long-lived access.\n- scope: name\n  description: Member's full name claim.\n- scope: given_name\n  description: Member's given (first) name claim.\n- scope: family_name\n  description: Member's family (last) name claim.\n- scope: nickname\n  description: Member's nickname claim.\n- scope: email\n  description: Member's email address claim.\n- scope: email_verified\n  description: Whether the member's email address has been verified.\n- scope: picture\n  description: URL of the member's profile picture.\n- scope: created_at\n  description: Timestamp the member's identity record was created.\n- scope: identities\n  description: Linked identity provider records for the member.\n- scope: phone\n  description: Member's phone number claim.\n- scope: address\n  description: Member's postal address claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devoted/refs/heads/main/scopes/devoted-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Healthcare
- Medicare Advantage
- Health Insurance
- FHIR
- Interoperability
- CMS Patient Access
- Payer
token_urls: []
---
