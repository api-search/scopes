---
api_specs:
- filename: devoted-health-patient-access-openapi-original.json
  format: json
  label: Devoted Health Patient Access API
  slug: devoted-health-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted-health/refs/heads/main/openapi/devoted-health-patient-access-openapi-original.json
- filename: devoted-health-provider-directory-openapi-original.yml
  format: yaml
  label: Devoted Health Provider Directory & Formulary API
  slug: devoted-health-provider-directory-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devoted-health/refs/heads/main/openapi/devoted-health-provider-directory-openapi-original.yml
authorization_urls: []
description: ''
docs: https://www.devoted.com/developers/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Devoted Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Devoted Health publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Devoted Health API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Devoted Health
provider_slug: devoted-health
schemes:
- authorizationUrl: https://login.devoted.com/authorize
  issuer: https://login.devoted.com/
  name: OpenID Connect
  source: well-known/devoted-health-openid-configuration.json
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
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Access to the end user's default profile claims.
  flows: []
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: End user's full name.
  flows: []
  scope: name
- description: End user's given (first) name.
  flows: []
  scope: given_name
- description: End user's family (last) name.
  flows: []
  scope: family_name
- description: End user's nickname.
  flows: []
  scope: nickname
- description: End user's email address.
  flows: []
  scope: email
- description: Whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: End user's profile picture URL.
  flows: []
  scope: picture
- description: Account creation timestamp.
  flows: []
  scope: created_at
- description: End user's linked identities.
  flows: []
  scope: identities
- description: End user's phone number.
  flows: []
  scope: phone
- description: End user's postal address.
  flows: []
  scope: address
slug: devoted-health-scopes
source_filename: devoted-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.devoted.com/.well-known/openid-configuration\ndocs: https://www.devoted.com/developers/\nnotes: >-\n  Devoted Health authorizes FHIR access with OAuth 2.0 / OpenID Connect using\n  SMART-on-FHIR. The OpenID Connect discovery document publishes the OIDC\n  scopes_supported below. The Patient Access API is patient-authorized and,\n  per SMART-on-FHIR / CMS Patient Access conventions, is accessed with\n  patient-scoped clinical scopes (e.g. patient/Patient.read); those clinical\n  scopes are not enumerated in the discovery document, so only the OIDC scopes\n  Devoted actually publishes are asserted here as searched, with the expected\n  SMART clinical-scope pattern noted as convention.\nschemes:\n- name: OpenID Connect\n  issuer: https://login.devoted.com/\n  authorizationUrl: https://login.devoted.com/authorize\n  tokenUrl: https://login.devoted.com/oauth/token\n  source: well-known/devoted-health-openid-configuration.json\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n- scope: profile\n  description: Access to the end user's default profile claims.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n- scope: name\n  description: End user's full name.\n- scope: given_name\n  description: End user's given (first) name.\n- scope: family_name\n  description: End user's family (last) name.\n- scope: nickname\n  description: End user's nickname.\n- scope: email\n  description: End user's email address.\n- scope: email_verified\n  description: Whether the end user's email address has been verified.\n- scope: picture\n  description: End user's profile picture URL.\n- scope: created_at\n  description: Account creation timestamp.\n- scope: identities\n  description: End user's linked identities.\n- scope: phone\n  description: End user's phone number.\n- scope: address\n  description: End user's postal address.\nsmart_clinical_scope_convention:\n\
  \  note: >-\n    Per SMART-on-FHIR / CMS Patient Access, member-authorized reads use\n    patient-context clinical scopes of the form patient/<Resource>.read for the\n    resources the Patient Access API exposes. These are governed by Devoted's\n    consent flow and are not enumerated in the OIDC discovery document.\n  expected_patterns:\n  - patient/Patient.read\n  - patient/Condition.read\n  - patient/Encounter.read\n  - patient/Medication.read\n  - patient/ExplanationOfBenefit.read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devoted-health/refs/heads/main/scopes/devoted-health-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Patient Access
- Provider Directory
- Drug Formulary
- CMS
- HL7
- SMART on FHIR
token_urls: []
---
