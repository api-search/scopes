---
authorization_urls: []
description: ''
docs: https://www.cuevr.com/getting-started/integrations
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cuevr Scopes
name_suffix: OAuth Scopes
note: These are permissions on API access keys (not OAuth 2.0 scopes); Cuevr documents no OAuth flow.
overview: 'Cuevr publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cuevr API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cuevr
provider_slug: cuevr-com
schemes: []
scope_count: 7
scope_names:
- clients:read
- clients:write
- proposals:read
- proposals:write
- qualification:read
- qualification:write
- webhooks:manage
scopes:
- description: View clients.
  flows: []
  scope: clients:read
- description: Create, rename or link a client to your CRM.
  flows: []
  scope: clients:write
- description: View proposals.
  flows: []
  scope: proposals:read
- description: Create a proposal from a deal, close or reopen the deal.
  flows: []
  scope: proposals:write
- description: View a proposal's qualification.
  flows: []
  scope: qualification:read
- description: Add the deal's notes to the qualification at creation.
  flows: []
  scope: qualification:write
- description: Manage destinations and how they operate.
  flows: []
  scope: webhooks:manage
slug: cuevr-com-scopes
source_filename: cuevr-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Cuevr access key permissions\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://www.cuevr.com/getting-started/integrations\ndocs: https://www.cuevr.com/getting-started/integrations\nnote: These are permissions on API access keys (not OAuth 2.0 scopes); Cuevr documents no OAuth flow.\nscopes:\n- name: clients:read\n  label: Read clients\n  description: View clients.\n- name: clients:write\n  label: Create and edit clients\n  description: Create, rename or link a client to your CRM.\n- name: proposals:read\n  label: Read proposals\n  description: View proposals.\n- name: proposals:write\n  label: Create and edit proposals\n  description: Create a proposal from a deal, close or reopen the deal.\n- name: qualification:read\n  label: Read qualifications\n  description: View a proposal's qualification.\n- name: qualification:write\n  label: Write in qualifications\n  description: Add the deal's notes to the qualification at creation.\n- name: webhooks:manage\n  label:\
  \ Manage delivery destinations\n  description: Manage destinations and how they operate.\nrules:\n- To receive a family of events, the key that subscribes a destination must also have read permission for that family.\n"
source_yaml_url: https://artifacts.apis.io/cuevr-com/scopes/cuevr-com-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Sales Proposals
- E-Signature
- RFP
- Sales Enablement
- Artificial Intelligence
- MCP
- Webhook
token_bound: false
token_urls: []
---
