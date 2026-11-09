---
authorization_urls: []
description: ''
docs: https://docs.demiton.io/registers/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Demiton Io Scopes
name_suffix: OAuth Scopes
note: These are Demiton's documented data-read permissions, enforced per register at query time across API, MCP and Studio. The docs do not say whether they are issued as OAuth scope strings on MCP tokens; they are recorded as documented permissions, not as observed token scopes.
overview: 'Demiton publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Demiton API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Demiton
provider_slug: demiton-io
schemes: []
scope_count: 3
scope_names:
- data:read_operations
- data:read_financials
- data:read_payroll
scopes:
- description: Read operations-domain registers (project activity, forms, allocations, plant movements, site records).
  flows: []
  scope: data:read_operations
- description: Read financials-domain registers (cost codes, rates, budget variance, contract financials). Name follows the documented data:read_<scope> pattern for the financials domain.
  flows: []
  scope: data:read_financials
- description: Read payroll-domain registers (pay runs, pay rates, leave, timesheets) - most restricted.
  flows: []
  scope: data:read_payroll
slug: demiton-io-scopes
source_filename: demiton-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://docs.demiton.io/registers/\ndocs: https://docs.demiton.io/registers/\nnote: These are Demiton's documented data-read permissions, enforced per register at query time across API, MCP and Studio. The docs do not say whether they are issued as OAuth scope strings on MCP tokens; they are recorded as documented permissions, not as observed token scopes.\nscopes:\n- name: data:read_operations\n  description: Read operations-domain registers (project activity, forms, allocations, plant movements, site records).\n- name: data:read_financials\n  description: Read financials-domain registers (cost codes, rates, budget variance, contract financials). Name follows the documented data:read_<scope> pattern for the financials domain.\n- name: data:read_payroll\n  description: Read payroll-domain registers (pay runs, pay rates, leave, timesheets) - most restricted.\n"
source_yaml_url: https://artifacts.apis.io/demiton-io/scopes/demiton-io-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Construction
- Civil Engineering
- Project Management
- Compliance
- MCP
- Artificial Intelligence
- Open Contracting
token_bound: false
token_urls: []
---
