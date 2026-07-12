---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Roivant Sciences Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Roivant Sciences publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Roivant Sciences API on a user''s behalf.


  Tokens are issued from https://api.healthjump.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Roivant Sciences
provider_slug: roivant-sciences
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.healthjump.com/oauth/token
  name: OAuth2
  source: openapi/datavant-healthjump-ehr-openapi.yml
scope_count: 3
scope_names:
- read:clinical
- read:financial
- read:patients
scopes:
- description: Read all clinical resources (encounters, vitals, labs, etc.).
  flows:
  - clientCredentials
  scope: read:clinical
- description: Read financial and billing-related fields.
  flows:
  - clientCredentials
  scope: read:financial
- description: Read patient demographic and clinical records.
  flows:
  - clientCredentials
  scope: read:patients
slug: roivant-sciences-scopes
source_filename: roivant-sciences-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datavant-healthjump-ehr-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/datavant-healthjump-ehr-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.healthjump.com/oauth/token\nscopes:\n- scope: read:clinical\n  description: Read all clinical resources (encounters, vitals, labs, etc.).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/datavant-healthjump-ehr-openapi.yml\n- scope: read:financial\n  description: Read financial and billing-related fields.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/datavant-healthjump-ehr-openapi.yml\n- scope: read:patients\n  description: Read patient demographic and clinical records.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/datavant-healthjump-ehr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roivant-sciences/refs/heads/main/scopes/roivant-sciences-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Biotech
- Pharmaceutical
- Drug Development
- Clinical Trials
- Health Data
- Tokenization
- Electronic Health Records
- Real World Evidence
- Holding Company
- Healthcare
token_urls:
- https://api.healthjump.com/oauth/token
---
