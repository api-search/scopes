---
authorization_urls: []
description: ''
docs: https://www.health-samurai.io/docs/aidbox/modules/security-and-access-control/auth/smart-on-fhir
flows:
- authorizationCode
- clientCredentials
- implicit
- password
kind: oauth-scopes
layout: scope
method: searched
name: Aidbox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aidbox publishes 12 OAuth 2.0 scopes via the authorizationCode, clientCredentials, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aidbox API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aidbox
provider_slug: aidbox
schemes:
- authorizationUrl: https://sandbox.aidbox.app/auth/authorize
  flows:
  - authorizationCode
  - clientCredentials
  - implicit
  - password
  name: SMART-on-FHIR / OAuth2
  tokenUrl: https://sandbox.aidbox.app/auth/token
scope_count: 12
scope_names:
- openid
- profile
- email
- groups
- fhirUser
- launch
- launch/patient
- offline_access
- online_access
- patient/*.cruds
- user/*.cruds
- system/*.cruds
scopes:
- description: OpenID Connect authentication; issue an id_token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email claim.
  flows: []
  scope: email
- description: Access to the user's group memberships.
  flows: []
  scope: groups
- description: Return a fhirUser claim identifying the current user as a FHIR resource.
  flows: []
  scope: fhirUser
- description: EHR launch context (requires an EHR launch).
  flows: []
  scope: launch
- description: Standalone launch requesting patient context selection.
  flows: []
  scope: launch/patient
- description: Issue a refresh token for long-lived access (permission-offline).
  flows: []
  scope: offline_access
- description: Refresh token valid only while the user's session is active.
  flows: []
  scope: online_access
- description: Patient-compartment access to all resource types (SMART v2 CRUDS = create, read, update, delete, search). Narrowable per resource, e.g. patient/Observation.rs.
  flows: []
  scope: patient/*.cruds
- description: User-level access to all resource types the user is permitted to see (SMART v2).
  flows: []
  scope: user/*.cruds
- description: System/backend-services access to all resource types (SMART Backend Services, v2).
  flows: []
  scope: system/*.cruds
slug: aidbox-scopes
source_filename: aidbox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: well-known/aidbox-smart-configuration.json (scopes_supported) + SMART App Launch scope syntax\ndocs: https://www.health-samurai.io/docs/aidbox/modules/security-and-access-control/auth/smart-on-fhir\nschemes:\n- name: SMART-on-FHIR / OAuth2\n  authorizationUrl: https://sandbox.aidbox.app/auth/authorize\n  tokenUrl: https://sandbox.aidbox.app/auth/token\n  flows: [authorizationCode, clientCredentials, implicit, password]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an id_token.\n- scope: profile\n  description: Access to the user's basic profile claims.\n- scope: email\n  description: Access to the user's email claim.\n- scope: groups\n  description: Access to the user's group memberships.\n- scope: fhirUser\n  description: Return a fhirUser claim identifying the current user as a FHIR resource.\n- scope: launch\n  description: EHR launch context (requires an EHR launch).\n- scope: launch/patient\n\
  \  description: Standalone launch requesting patient context selection.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access (permission-offline).\n- scope: online_access\n  description: Refresh token valid only while the user's session is active.\n- scope: patient/*.cruds\n  description: >-\n    Patient-compartment access to all resource types (SMART v2 CRUDS = create, read,\n    update, delete, search). Narrowable per resource, e.g. patient/Observation.rs.\n- scope: user/*.cruds\n  description: User-level access to all resource types the user is permitted to see (SMART v2).\n- scope: system/*.cruds\n  description: System/backend-services access to all resource types (SMART Backend Services, v2).\nsmart_scope_syntax:\n  versions: [v1, v2]\n  v1_examples: [patient/Observation.read, user/*.read, system/Patient.write]\n  v2_actions: c=create, r=read, u=update, d=delete, s=search\n  note: >-\n    Aidbox supports both SMART v1 (.read/.write/.*) and v2 (.cruds\
  \ granular) scope syntaxes;\n    scopes_supported in the sandbox smart-configuration advertises the wildcard *.cruds forms.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidbox/refs/heads/main/scopes/aidbox-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials/implicit/password
tags:
- Healthcare
- United States
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- EHR
- Health Data
- FHIR Server
- Bulk Data
- Terminology
- Digital Health
token_urls: []
---
