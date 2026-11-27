---
authorization_urls: []
description: ''
docs: https://configo.org/docs/dev/reference#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Configo Scopes
name_suffix: OAuth Scopes
note: All scopes required by an endpoint must be present on the token. Endpoints under /api/v1/projects/{project.uuid}/ require both projects and the resource scope. Scopes combine with per-project role permissions (e.g. can_view_all_orders).
overview: 'Configo publishes 17 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Configo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Configo
provider_slug: configo-org
schemes: []
scope_count: 17
scope_names:
- identify
- billing
- files
- projects
- members
- orders
- clients
- tasks
- reports
- materials
- configurators
- products
- warehouses
- wiki
- documents
- email_templates
- automations
scopes:
- description: The user's profile, connected accounts, referrals, locale and notifications
  flows: []
  scope: identify
- description: Subscription, plans, payments and balance
  flows: []
  scope: billing
- description: Uploading, retrieving and deleting files
  flows: []
  scope: files
- description: 'Projects and their settings: funnels, statuses, loss reasons, contact fields'
  flows: []
  scope: projects
- description: Project members, invitations and roles
  flows: []
  scope: members
- description: Orders
  flows: []
  scope: orders
- description: Contacts, companies and tags
  flows: []
  scope: clients
- description: Tasks
  flows: []
  scope: tasks
- description: Reports
  flows: []
  scope: reports
- description: Materials
  flows: []
  scope: materials
- description: Configurators and the public showcase
  flows: []
  scope: configurators
- description: Products
  flows: []
  scope: products
- description: Warehouses and stock
  flows: []
  scope: warehouses
- description: The wiki
  flows: []
  scope: wiki
- description: Document templates
  flows: []
  scope: documents
- description: Email templates and the mail sender
  flows: []
  scope: email_templates
- description: Automations
  flows: []
  scope: automations
slug: configo-org-scopes
source_filename: configo-org-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://configo.org/docs/dev/reference\ndocs: https://configo.org/docs/dev/reference#scopes\nnote: All scopes required by an endpoint must be present on the token. Endpoints under /api/v1/projects/{project.uuid}/ require\n  both projects and the resource scope. Scopes combine with per-project role permissions (e.g. can_view_all_orders).\nscopes:\n- name: identify\n  description: The user's profile, connected accounts, referrals, locale and notifications\n- name: billing\n  description: Subscription, plans, payments and balance\n- name: files\n  description: Uploading, retrieving and deleting files\n- name: projects\n  description: 'Projects and their settings: funnels, statuses, loss reasons, contact fields'\n- name: members\n  description: Project members, invitations and roles\n- name: orders\n  description: Orders\n- name: clients\n  description: Contacts, companies and tags\n- name: tasks\n  description: Tasks\n- name:\
  \ reports\n  description: Reports\n- name: materials\n  description: Materials\n- name: configurators\n  description: Configurators and the public showcase\n- name: products\n  description: Products\n- name: warehouses\n  description: Warehouses and stock\n- name: wiki\n  description: The wiki\n- name: documents\n  description: Document templates\n- name: email_templates\n  description: Email templates and the mail sender\n- name: automations\n  description: Automations\n"
source_yaml_url: https://artifacts.apis.io/configo-org/scopes/configo-org-scopes.yml
summary_line: 17 scopes
tags:
- Company
- CPQ
- Product Configurator
- Manufacturing
- Pricing
- CRM
- Inventory
- MCP
token_bound: false
token_urls: []
---
