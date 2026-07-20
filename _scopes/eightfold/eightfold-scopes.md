---
api_specs:
- filename: llms.txt
  format: yaml
  label: Eightfold API v2
  slug: eightfold-api-v2
  spec_type: OpenAPI
  url: https://apidocs.eightfold.ai/llms.txt
authorization_urls: []
description: ''
docs: https://apidocs.eightfold.ai/docs/eightfold-api-authorization-guide
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Eightfold Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Eightfold uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eightfold
provider_slug: eightfold
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: eightfold-scopes
source_filename: eightfold-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://apidocs.eightfold.ai/docs/eightfold-api-authorization-guide\ndocs: https://apidocs.eightfold.ai/docs/eightfold-api-authorization-guide\nmodel: >-\n  Eightfold uses a permission-based authorization system. Each API key is assigned\n  specific permissions in the Admin Console. Permissions follow a hierarchical structure:\n  logical_entity[:logical_subentity]:SCOPE, where SCOPE is READ or WRITE. A request is\n  allowed only when the calling key holds the required entity permission for that\n  endpoint. Global READ / global WRITE toggles grant all read or all write endpoints.\nscope_grammar: 'logical_entity[:logical_subentity]:SCOPE   # SCOPE in {READ, WRITE}'\nscope_types: [READ, WRITE]\nexample_scopes:\n- scope: ats_position:READ\n  description: Read ATS positions (Get, List)\n- scope: ats_position:WRITE\n  description: Create/Update/Patch ATS positions\n- scope: profile:READ\n  description: Read candidate/employee profiles\n\
  - scope: profile:WRITE\n  description: Create/Update/Patch/Delete profiles\n- scope: profile:skills:READ\n  description: Read the skills sub-entity of a profile (sub-entity example)\n- scope: position:READ\n  description: Read positions\n- scope: position:WRITE\n  description: Create/Update/Patch positions\n- scope: demand:READ\n  description: Read demands\n- scope: demand:WRITE\n  description: Create/Update/Patch/Delete demands\n- scope: booking:READ\n  description: Read bookings (resource management)\n- scope: booking:WRITE\n  description: Create/Update/Patch/Delete bookings\nnotes: >-\n  The concrete entity list is enumerated in the Admin Console permission UI and the\n  authorization guide's endpoint/permission reference table; scopes above are\n  representative examples of the entity:SCOPE grammar, not the exhaustive registry.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eightfold/refs/heads/main/scopes/eightfold-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Talent Intelligence
- Talent Acquisition
- Talent Management
- Recruiting
- Human Resources
- Workforce Planning
- HRIS
- ATS
- Artificial Intelligence
- SCIM
- REST
token_urls: []
---
