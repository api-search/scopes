---
authorization_urls: []
description: OAuth 2.0 scope model for the Employment Hero API. Scopes are selected by the developer at application-registration time and consented by the organisation admin during the authorization-code (PKCE) flow; the public docs describe scope selection and give organisation/employee read examples rather than an exhaustive machine-readable scope registry. Captured verbatim from the docs; the full enumerated scope list is not published publicly.
docs: https://developer.employmenthero.com/api-references
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Humica Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'humi.ca publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the humi.ca API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: humi.ca
provider_slug: humica
schemes:
- authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize
  flow: authorizationCode
  name: OAuth2
  tokenUrl: https://oauth.employmenthero.com/oauth2/token
scope_count: 2
scope_names:
- organisation:read
- employee:read
scopes:
- description: Read access to organisation-level data (documented as an example scope).
  flows:
  - authorizationCode
  scope: organisation:read
- description: Read access to employee data (documented as an example scope).
  flows:
  - authorizationCode
  scope: employee:read
slug: humica-scopes
source_filename: humica-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.employmenthero.com/api-references\ndocs: https://developer.employmenthero.com/api-references\ndescription: >-\n  OAuth 2.0 scope model for the Employment Hero API. Scopes are selected by the\n  developer at application-registration time and consented by the organisation\n  admin during the authorization-code (PKCE) flow; the public docs describe\n  scope selection and give organisation/employee read examples rather than an\n  exhaustive machine-readable scope registry. Captured verbatim from the docs;\n  the full enumerated scope list is not published publicly.\nschemes:\n  - name: OAuth2\n    flow: authorizationCode\n    authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize\n    tokenUrl: https://oauth.employmenthero.com/oauth2/token\nscopes:\n  - scope: organisation:read\n    description: Read access to organisation-level data (documented as an example scope).\n    flows: [authorizationCode]\n\
  \    note: example scope named in the docs; exact scope string is developer-selected at app registration.\n  - scope: employee:read\n    description: Read access to employee data (documented as an example scope).\n    flows: [authorizationCode]\n    note: example scope named in the docs; exact scope string is developer-selected at app registration.\nscope_selection: >-\n  Scopes are chosen per application at registration and granted by the\n  organisation admin during consent. Employment Hero does not publish a full\n  enumerated scope reference, so only the documented example scopes are recorded\n  here (no fabrication of unlisted scopes).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humica/refs/heads/main/scopes/humica-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Human Resources
- Payroll
- HR Tech
- Benefits
- Applicant Tracking
- Employer of Record
- Canada
- SaaS
token_urls: []
---
