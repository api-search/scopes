---
authorization_urls: []
description: ''
docs: https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Innovaccer Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Innovaccer publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Innovaccer API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Innovaccer
provider_slug: innovaccer
schemes: []
scope_count: 9
scope_names:
- hmcp:access
- hmcp:read
- hmcp:write
- patient/hmcp:read
- patient/hmcp:write
- openid
- profile
- launch/patient
- offline_access
scopes:
- description: Basic access to HMCP services.
  flows: []
  scope: hmcp:access
- description: Read access to HMCP resources.
  flows: []
  scope: hmcp:read
- description: Write access to HMCP resources.
  flows: []
  scope: hmcp:write
- description: Read access limited to the current patient context.
  flows: []
  scope: patient/hmcp:read
- description: Write access limited to the current patient context.
  flows: []
  scope: patient/hmcp:write
- description: Authentication using OpenID Connect; returns an ID token.
  flows: []
  scope: openid
- description: Access to basic user profile information.
  flows: []
  scope: profile
- description: Request patient context at launch time; token response includes a `patient` parameter.
  flows: []
  scope: launch/patient
- description: Request a refresh token for offline access.
  flows: []
  scope: offline_access
slug: innovaccer-scopes
source_filename: innovaccer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/auth.md\ndocs: https://github.com/innovaccer/Healthcare-MCP/blob/main/docs/specification/auth.md\napplies_to:\n  api: Healthcare Model Context Protocol (HMCP)\n  repository: https://github.com/innovaccer/Healthcare-MCP\nnotes: >-\n  Scopes published verbatim in the HMCP specification's \"Standard Scopes\" table.\n  These govern access to an HMCP server, Innovaccer's open-source healthcare\n  extension of MCP — not the gated Nucleus / Datashop platform API, for which no\n  scope reference is published anonymously. Derived from documentation, not from a\n  machine-readable securitySchemes block (Innovaccer publishes no OpenAPI).\nframework: SMART on FHIR\nformat:\n  pattern: \"[patient/][(read|write)].[resource]\"\n  description: >-\n    Optional `patient/` prefix restricts access to resources associated with the\n    current patient context; `read`/`write`\
  \ sets permission level; the resource\n    segment names the resource type or action.\nscope_count: 9\nscopes:\n- name: hmcp:access\n  description: Basic access to HMCP services.\n- name: hmcp:read\n  description: Read access to HMCP resources.\n- name: hmcp:write\n  description: Write access to HMCP resources.\n- name: patient/hmcp:read\n  description: Read access limited to the current patient context.\n  patient_scoped: true\n- name: patient/hmcp:write\n  description: Write access limited to the current patient context.\n  patient_scoped: true\n- name: openid\n  description: Authentication using OpenID Connect; returns an ID token.\n- name: profile\n  description: Access to basic user profile information.\n- name: launch/patient\n  description: Request patient context at launch time; token response includes a `patient` parameter.\n- name: offline_access\n  description: Request a refresh token for offline access.\npatient_context_flow:\n- Client requests the resource scope with the `patient/`\
  \ prefix together with `launch/patient`.\n- Authorization server returns a `patient` parameter in the token response containing the patient ID.\n- All operations using that token are automatically restricted to that patient.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovaccer/refs/heads/main/scopes/innovaccer-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Healthcare
- Health Data
- FHIR
- Interoperability
- Population Health
- Artificial Intelligence
- Data Platform
- Design Systems
- MCP
token_bound: false
token_urls: []
---
