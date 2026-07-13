---
api_specs:
- filename: cerner-oracle-health-fhir-r4-api-openapi.yml
  format: yaml
  label: Oracle Health Millennium Platform FHIR R4 API
  slug: oracle-health-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/openapi/cerner-oracle-health-fhir-r4-api-openapi.yml
authorization_urls:
- https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/patient/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cerner Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cerner (Oracle Health) publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cerner (Oracle Health) API on a user''s behalf.


  Tokens are issued from https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cerner (Oracle Health)
provider_slug: cerner
schemes:
- description: SMART on FHIR OAuth 2.0 with patient, user, and system scopes.
  flows:
  - authorizationUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/patient/authorize
    flow: authorizationCode
    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token
  - flow: clientCredentials
    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token
  name: oauth2
  source: openapi/cerner-oracle-health-fhir-r4-api-openapi.yml
scope_count: 4
scope_names:
- patient/*.read
- system/*.read
- system/*.write
- user/*.read
scopes:
- description: Read all patient-scoped resources.
  flows:
  - authorizationCode
  scope: patient/*.read
- description: System-level read access.
  flows:
  - authorizationCode
  - clientCredentials
  scope: system/*.read
- description: System-level write access.
  flows:
  - clientCredentials
  scope: system/*.write
- description: Read all user-scoped resources.
  flows:
  - authorizationCode
  scope: user/*.read
slug: cerner-scopes
source_filename: cerner-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/personas/patient/authorize\n    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token\n  - flow: clientCredentials\n    tokenUrl: https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token\n  description: SMART on FHIR OAuth 2.0 with patient, user, and system scopes.\nscopes:\n- scope: patient/*.read\n  description: Read all patient-scoped resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\n- scope: system/*.read\n  description: System-level read access.\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\n- scope: system/*.write\n  description: System-level write access.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\n- scope: user/*.read\n  description: Read all user-scoped resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cerner-oracle-health-fhir-r4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerner/refs/heads/main/scopes/cerner-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Cerner Millennium
- Code Console
- EHR
- Electronic Health Records
- FHIR
- HL7
- Healthcare
- Interoperability
- OAuth 2.0
- Oracle Health
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 1000
token_urls:
- https://authorization.cerner.com/tenants/{tenant}/protocols/oauth2/profiles/smart-v1/token
---
