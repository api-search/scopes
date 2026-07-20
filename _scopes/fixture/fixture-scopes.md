---
api_specs:
- filename: fixture-v1-openapi.json
  format: json
  label: Fixture API v1
  slug: fixture-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/openapi/fixture-v1-openapi.json
authorization_urls: []
description: ''
docs: https://fixture.app/docs/authentication/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fixture Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fixture uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fixture
provider_slug: fixture
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fixture-scopes
source_filename: fixture-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://fixture.app/docs/authentication/scopes, https://beta-api.fixture.app/.well-known/oauth-authorization-server,\n  https://beta-api.fixture.app/.well-known/oauth-protected-resource\ndocs: https://fixture.app/docs/authentication/scopes\nsummary: Fixture runs two related scope vocabularies. API keys carry fine-grained resource\n  scopes (contacts:read, deals:write, ...) chosen explicitly at key creation. Fixture OAuth\n  access tokens — used by the CLI, the in-app Agent, and remote MCP clients — carry coarser\n  scopes (crm:read, crm:write, tasks:read, tasks:write, users:read) that map onto the same\n  API key scope requirements. Write implies read; there is no implicit full-access default.\nrules:\n- Write implies read. A key with contacts:write can also read Contacts.\n- The wildcard scope (*) satisfies any scope requirement. Intended for development keys.\n- A missing scope fails the request with 403 forbidden and a message\
  \ naming the scope.\n- Some operations require multiple scopes because they create resources across entities.\nscope_sets:\n- name: api-key\n  description: Fine-grained scopes assigned to a workspace API key at creation time.\n  source: https://fixture.app/docs/authentication/scopes\n  scopes:\n  - scope: contacts:read\n    description: View Contacts and their details\n  - scope: contacts:write\n    description: Create, update, and delete Contacts\n  - scope: accounts:read\n    description: View Accounts and their details\n  - scope: accounts:write\n    description: Create, update, and delete Accounts\n  - scope: deals:read\n    description: View Deals and their details\n  - scope: deals:write\n    description: Create, update, and delete Deals\n  - scope: users:read\n    description: View Team Users that can own Accounts and Deals\n  - scope: pipelines:read\n    description: View Pipelines and their Stages\n  - scope: leads:read\n    description: View Leads and their details\n  - scope:\
  \ leads:write\n    description: Create, update, and delete Leads\n  - scope: activities:read\n    description: View Activities and interaction history\n  - scope: activities:write\n    description: Create custom Activities\n  - scope: '*'\n    description: Full access to all resources\n- name: oauth\n  description: Scopes advertised by the Fixture Authorization Server metadata and required\n    by the remote MCP endpoint. Granted CRM and task scopes map onto the API key scope requirements.\n  issuer: https://beta-api.fixture.app\n  source: https://beta-api.fixture.app/.well-known/oauth-authorization-server\n  scopes:\n  - scope: crm:read\n    description: Read CRM records (Accounts, Contacts, Deals, Leads, Activities, Pipelines)\n  - scope: crm:write\n    description: Create and update CRM records\n  - scope: tasks:read\n    description: Read Tasks and Task Statuses\n  - scope: tasks:write\n    description: Create, update, and complete Tasks\n  - scope: users:read\n    description: Read\
  \ team Users\ncompound_requirements:\n- operation: convertLead\n  path: POST /api/v1/leads/{id}/convert\n  requires:\n  - scope: leads:write\n    always: true\n  - scope: accounts:write\n    always: true\n  - scope: contacts:write\n    always: true\n  - scope: deals:write\n    always: false\n    condition: only when create_deal is true\nmissing_scope_response:\n  status: 403\n  body:\n    error:\n      code: forbidden\n      message: 'Missing required scope: contacts:write'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixture/refs/heads/main/scopes/fixture-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- CRM
- Sales
- B2B
- Artificial Intelligence
- Agents
- MCP
- Customer Relationship Management
token_urls: []
---
