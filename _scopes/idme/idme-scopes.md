---
authorization_urls:
- https://api.id.me/oauth/authorize
description: ''
docs: https://docs.id.me/integrations/configurations/configuration-standards
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Idme Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ID.me publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ID.me API on a user''s behalf.


  Tokens are issued from https://api.id.me/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ID.me
provider_slug: idme
schemes:
- flows:
  - authorizationUrl: https://api.id.me/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.id.me/oauth/token
  name: OAuth2
  source: well-known/idme-openid-configuration.json
scope_count: 11
scope_names:
- openid
- military
- responder
- student
- teacher
- government
- employee
- hospital_employee
- alumni
- nurse
- medical
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Members and dependents of the uniformed services.
  flows: []
  scope: military
- description: Active and retired members of the first responder community.
  flows: []
  scope: responder
- description: Members actively enrolled in accredited public/private universities or colleges.
  flows: []
  scope: student
- description: Members of the teaching community.
  flows: []
  scope: teacher
- description: Members employed by federal, state, or local governments.
  flows: []
  scope: government
- description: Members employed by partnering companies.
  flows: []
  scope: employee
- description: Members employed by hospitals and healthcare systems.
  flows: []
  scope: hospital_employee
- description: Members with degrees from accredited institutions.
  flows: []
  scope: alumni
- description: Members of the nursing community.
  flows: []
  scope: nurse
- description: Members of the medical professional community.
  flows: []
  scope: medical
slug: idme-scopes
source_filename: idme-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.id.me/oidc/.well-known/openid-configuration\ndocs: https://docs.id.me/integrations/configurations/configuration-standards\nschemes:\n- name: OAuth2\n  source: well-known/idme-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.id.me/oauth/authorize\n    tokenUrl: https://api.id.me/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  sources: [well-known/idme-openid-configuration.json]\n# ID.me maps \"scope\" to a verification policy/community group. The discovery doc\n# advertises only `openid`; the following are the standard community/affiliation\n# scope values documented in the configuration standards reference.\n- scope: military\n  description: Members and dependents of the uniformed services.\n  group: community\n- scope: responder\n  description: Active and retired members of the first responder community.\n\
  \  group: community\n- scope: student\n  description: Members actively enrolled in accredited public/private universities or colleges.\n  group: community\n- scope: teacher\n  description: Members of the teaching community.\n  group: community\n- scope: government\n  description: Members employed by federal, state, or local governments.\n  group: community\n- scope: employee\n  description: Members employed by partnering companies.\n  group: community\n- scope: hospital_employee\n  description: Members employed by hospitals and healthcare systems.\n  group: community\n- scope: alumni\n  description: Members with degrees from accredited institutions.\n  group: community\n- scope: nurse\n  description: Members of the nursing community.\n  group: community\n- scope: medical\n  description: Members of the medical professional community.\n  group: community\nauthn_context:\n- value: mfa\n  description: Multi-factor authentication.\n- value: kba_replacement\n  description: Identity proofing\
  \ requiring one piece of evidence.\n- value: fortified_identity\n  description: Identity proofing requiring two pieces of evidence.\n- value: http://idmanagement.gov\n  description: NIST IAL2/AAL2 identity assurance.\nnotes: >-\n  Canadian community equivalents also exist (military_canada, responder_canada,\n  student_canada, teacher_canada, government_canada, nurse_canada, doctor_canada,\n  alumni_canada). Scopes resolve to policies configured per client application.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idme/refs/heads/main/scopes/idme-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Company
- Identity
- Identity Verification
- Authentication
- OpenID Connect
- OAuth 2.0
- SAML
- Single Sign-On
- Digital Identity
- KYC
- Fraud Prevention
- Government
token_urls:
- https://api.id.me/oauth/token
---
