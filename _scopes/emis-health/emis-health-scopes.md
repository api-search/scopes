---
api_specs:
- filename: emis-health-partner-api-openapi.json
  format: json
  label: EMIS Partner API (PAPI)
  slug: emis-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emis-health/refs/heads/main/openapi/emis-health-partner-api-openapi.json
authorization_urls:
- https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/authorize
description: ''
docs: https://docs.partner.emis-x.uk/auth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Emis Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EMIS Health publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the EMIS Health API on a user''s behalf.


  Tokens are issued from https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EMIS Health
provider_slug: emis-health
schemes:
- flows:
  - authorizationUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/token
  name: OAuth2CodeEMIS-X-GP-PAPI
  source: openapi/emis-health-partner-api-openapi.json
  type: oauth2
scope_count: 7
scope_names:
- papi-appt.read
- papi-appt.write
- papi-cr.read
- papi-cr.write
- papi-subjects.read
- papi-config.read
- papi-searches.read
scopes:
- description: Read Appointments
  flows:
  - authorizationCode
  scope: papi-appt.read
- description: Write Appointments
  flows:
  - authorizationCode
  scope: papi-appt.write
- description: Read Clinical Record
  flows:
  - authorizationCode
  scope: papi-cr.read
- description: Write Clinical Record
  flows:
  - authorizationCode
  scope: papi-cr.write
- description: Read Subjects (patient demographics, matching, sequence)
  flows:
  - authorizationCode
  scope: papi-subjects.read
- description: Read Config (organisation lookup, user details)
  flows:
  - authorizationCode
  scope: papi-config.read
- description: Read Searches (population/clinical searches)
  flows:
  - authorizationCode
  scope: papi-searches.read
slug: emis-health-scopes
source_filename: emis-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/emis-health-partner-api-openapi.json\ndocs: https://docs.partner.emis-x.uk/auth/\nnotes: >-\n  Two scope surfaces exist. (1) The OAuth2 authorizationCode flow declared in the\n  PAPI OpenAPI enumerates seven papi-* scopes below. (2) The EMIS-X access token\n  additionally carries an \"authorizations\" JWT claim array of ERN-granted\n  clinical/agreement scopes (clinical-cr.*, agmt-agmt.read, doc-app.*,\n  term-prep.read) documented on the auth page; these govern EMIS-X clinical\n  record access and are granted per partner agreement, not requested in the\n  OAuth flow. Both are recorded verbatim from the spec and docs.\nschemes:\n- name: OAuth2CodeEMIS-X-GP-PAPI\n  source: openapi/emis-health-partner-api-openapi.json\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/authorize\n    tokenUrl:\
  \ https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/token\nscopes:\n- scope: papi-appt.read\n  description: Read Appointments\n  flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- scope: papi-appt.write\n  description: Write Appointments\n  flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- scope: papi-cr.read\n  description: Read Clinical Record\n  flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- scope: papi-cr.write\n  description: Write Clinical Record\n  flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- scope: papi-subjects.read\n  description: Read Subjects (patient demographics, matching, sequence)\n  flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- scope: papi-config.read\n  description: Read Config (organisation lookup, user details)\n \
  \ flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\n- scope: papi-searches.read\n  description: Read Searches (population/clinical searches)\n  flows: [authorizationCode]\n  sources: [openapi/emis-health-partner-api-openapi.json]\nauthorizations_claim_scopes:\n- scope: clinical-cr.read\n  description: Read the EMIS-X clinical record (authorizations JWT claim)\n  source: https://docs.partner.emis-x.uk/auth/\n- scope: clinical-cr.write\n  description: Write to the EMIS-X clinical record (authorizations JWT claim)\n  source: https://docs.partner.emis-x.uk/auth/\n- scope: agmt-agmt.read\n  description: Read partner agreement context (authorizations JWT claim)\n  source: https://docs.partner.emis-x.uk/auth/\n- scope: doc-app.addcode\n  description: Add a clinical code via a document/app context (authorizations JWT claim)\n  source: https://docs.partner.emis-x.uk/auth/\n- scope: doc-app.create\n  description: Create a document/app record (authorizations JWT\
  \ claim)\n  source: https://docs.partner.emis-x.uk/auth/\n- scope: term-prep.read\n  description: Read terminology preparation data (authorizations JWT claim)\n  source: https://docs.partner.emis-x.uk/auth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emis-health/refs/heads/main/scopes/emis-health-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Healthcare
- United Kingdom
- EHR
- EMR
- Interoperability
- HL7
- FHIR
- Primary Care
- NHS
- Clinical Data
- Electronic Patient Record
token_urls:
- https://identity.stg.emis-x.uk/b205162c-c95a-4639-8076-bb1fcb152d2b/b2c_1a_clientcredentials/oauth2/token
---
