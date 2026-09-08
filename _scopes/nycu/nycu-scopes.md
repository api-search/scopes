---
api_specs:
- filename: nycu-oauth-api-openapi.yml
  format: yaml
  label: NYCU OAuth API
  slug: oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nycu/refs/heads/main/openapi/nycu-oauth-api-openapi.yml
authorization_urls: []
description: 'The three scopes published by the NYCU OAuth service. NYCU splits them into non-sensitive (非機敏) and sensitive (機敏): any registered developer may request `profile`, while `name` and `status` must be justified on an in-console application form and approved by the Information Technology Service Center. The terms of service state that, in principle, only systems developed or operated by the university are granted the sensitive scopes.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Nycu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'National Yang Ming Chiao Tung University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: National Yang Ming Chiao Tung University
provider_slug: nycu
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: nycu-scopes
source_filename: nycu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: National Yang Ming Chiao Tung University\nproviderId: nycu\ngenerated: '2026-09-01'\nmethod: searched\nsource: https://id.nycu.edu.tw/docs/\nx-operator: institution\ndescription: >-\n  The three scopes published by the NYCU OAuth service. NYCU splits them into non-sensitive\n  (非機敏) and sensitive (機敏): any registered developer may request `profile`, while `name`\n  and `status` must be justified on an in-console application form and approved by the\n  Information Technology Service Center. The terms of service state that, in principle, only\n  systems developed or operated by the university are granted the sensitive scopes.\nscopes:\n  - name: profile\n    resource: Email, account name\n    endpoint: https://id.nycu.edu.tw/api/profile/\n    sensitivity: non-sensitive\n    approval_required: false\n  - name: name\n    resource: User's personal name, account name\n    endpoint: https://id.nycu.edu.tw/api/name/\n\
  \    sensitivity: sensitive\n    approval_required: true\n  - name: status\n    resource: Enrollment/employment status, account name\n    endpoint: https://id.nycu.edu.tw/api/status/\n    sensitivity: sensitive\n    approval_required: true\napproval:\n  process_url: https://id.nycu.edu.tw/apply/app\n  authority: NYCU Information Technology Service Center (資訊技術服務中心)\n  description: >-\n    Requested on the application's management page, stating the fields needed, the purpose, the\n    responsible unit and a contact. NYCU reserves the right to revoke, suspend or terminate a\n    client on security or misuse grounds.\nevidence:\n  - url: https://id.nycu.edu.tw/docs/\n    status: 200\n  - url: https://id.nycu.edu.tw/policy/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nycu/refs/heads/main/scopes/nycu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Taiwan
- Identity
- Authentication
- Single Sign-On
- Research Data
- Institutional Repository
- Library
- Metadata
token_urls: []
---
