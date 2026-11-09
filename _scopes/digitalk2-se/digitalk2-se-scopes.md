---
authorization_urls: []
description: ''
docs: https://www.digitalk2.se/mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Digitalk2 Se Scopes
name_suffix: OAuth Scopes
note: The docs name two user-chosen permissions at consent time; the literal OAuth scope strings are not published, so names below are the documented permission labels, not verified scope tokens.
overview: 'DigitalK2 publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DigitalK2 API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DigitalK2
provider_slug: digitalk2-se
schemes: []
scope_count: 2
scope_names:
- Read
- Prepare
scopes:
- description: See drafts, figures, tax calculation (the 7 read-only MCP tools).
  flows: []
  scope: Read
- description: Fill in and change drafts in steps 1 to 6. Never payment, signing or filing with Bolagsverket.
  flows: []
  scope: Prepare
slug: digitalk2-se-scopes
source_filename: digitalk2-se-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://raw.githubusercontent.com/digitalk2se/digitalk2-plugin/main/README.md\ndocs: https://www.digitalk2.se/mcp\nname: DigitalK2 OAuth permissions\nnote: The docs name two user-chosen permissions at consent time; the literal OAuth scope strings are not published, so names below are the documented permission labels, not verified scope tokens.\nscopes:\n- name: Read\n  description: See drafts, figures, tax calculation (the 7 read-only MCP tools).\n  quote: \"You choose the permissions: **Read** (see drafts, figures, tax calculation) and **Prepare** (fill in and change drafts in steps 1 to 6).\"\n- name: Prepare\n  description: Fill in and change drafts in steps 1 to 6. Never payment, signing or filing with Bolagsverket.\n"
source_yaml_url: https://artifacts.apis.io/digitalk2-se/scopes/digitalk2-se-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Accounting
- Annual Reports
- Bolagsverket
- Sweden
- SIE
- Small Business
- Tax
- MCP
token_bound: false
token_urls: []
---
