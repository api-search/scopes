---
api_specs:
- filename: competitortracker-io-openapi-generated.yml
  format: yaml
  label: Competitor Tracker & Co. API
  slug: competitortracker-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/competitortracker-io/openapi/_ae-authored/competitortracker-io-openapi-generated.yml
authorization_urls: []
description: A read endpoint wants the matching :read scope, a write endpoint the matching :write. The required scope and required organization role for each endpoint are shown on its API reference page. Missing scope returns 403 InsufficientScope; too-low role returns 403 InsufficientRole.
docs: https://competitortracker.io/docs/scopes-and-permissions/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Competitor Tracker & Co. Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Competitor Tracker & Co. publishes 22 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Competitor Tracker & Co. API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Competitor Tracker & Co.
provider_slug: competitortracker-io
schemes: []
scope_count: 22
scope_names:
- openid
- email
- profile
- mcp
- competitors:read
- competitors:write
- labels:read
- labels:write
- snapshots:read
- pages:read
- changes:read
- account:read
- account:write
- billing:read
- org:read
- org:write
- members:read
- members:write
- invites:read
- invites:write
- dispatches:read
- dispatches:write
scopes:
- description: Sign-in. Issues an id_token.
  flows: []
  scope: openid
- description: Puts the user's email on the id_token.
  flows: []
  scope: email
- description: Puts the user's name on the id_token.
  flows: []
  scope: profile
- description: Lets an MCP client act on the user's behalf.
  flows: []
  scope: mcp
- description: Read the competitors you track.
  flows: []
  scope: competitors:read
- description: Add, change and remove tracked competitors.
  flows: []
  scope: competitors:write
- description: Read labels.
  flows: []
  scope: labels:read
- description: Create, change and delete labels.
  flows: []
  scope: labels:write
- description: Read snapshots.
  flows: []
  scope: snapshots:read
- description: Read tracked pages.
  flows: []
  scope: pages:read
- description: Read detected changes.
  flows: []
  scope: changes:read
- description: Read your own profile and account settings.
  flows: []
  scope: account:read
- description: Update your own profile and account settings.
  flows: []
  scope: account:write
- description: Read the coin balance and transaction history.
  flows: []
  scope: billing:read
- description: Read organization settings.
  flows: []
  scope: org:read
- description: 'Manage organization settings: rename, ownership, deletion.'
  flows: []
  scope: org:write
- description: Read members.
  flows: []
  scope: members:read
- description: Manage member roles.
  flows: []
  scope: members:write
- description: Read invitations.
  flows: []
  scope: invites:read
- description: Create and revoke invitations.
  flows: []
  scope: invites:write
- description: Read dispatch settings and delivery history.
  flows: []
  scope: dispatches:read
- description: Manage notifications, recipients and webhooks.
  flows: []
  scope: dispatches:write
slug: competitortracker-io-scopes
source_filename: competitortracker-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://competitortracker.io/docs/scopes-and-permissions/\ndocs: https://competitortracker.io/docs/scopes-and-permissions/\ndescription: >-\n  A read endpoint wants the matching :read scope, a write endpoint the matching :write. The required\n  scope and required organization role for each endpoint are shown on its API reference page. Missing\n  scope returns 403 InsufficientScope; too-low role returns 403 InsufficientRole.\nscopes:\n- {name: openid, group: sign-in (OAuth2 only), description: Sign-in. Issues an id_token.}\n- {name: email, group: sign-in (OAuth2 only), description: Puts the user's email on the id_token.}\n- {name: profile, group: sign-in (OAuth2 only), description: Puts the user's name on the id_token.}\n- {name: mcp, group: sign-in (OAuth2 only), description: Lets an MCP client act on the user's behalf.}\n- {name: 'competitors:read', group: tracked data, description: Read the competitors you track.}\n- {name:\
  \ 'competitors:write', group: tracked data, description: 'Add, change and remove tracked competitors.'}\n- {name: 'labels:read', group: tracked data, description: Read labels.}\n- {name: 'labels:write', group: tracked data, description: 'Create, change and delete labels.'}\n- {name: 'snapshots:read', group: tracked data, description: Read snapshots.}\n- {name: 'pages:read', group: tracked data, description: Read tracked pages.}\n- {name: 'changes:read', group: tracked data, description: Read detected changes.}\n- {name: 'account:read', group: your account, description: Read your own profile and account settings.}\n- {name: 'account:write', group: your account, description: Update your own profile and account settings.}\n- {name: 'billing:read', group: your account, description: Read the coin balance and transaction history.}\n- {name: 'org:read', group: organization administration, description: Read organization settings.}\n- {name: 'org:write', group: organization administration, description:\
  \ 'Manage organization settings: rename, ownership, deletion.', grantable_by: admin or owner}\n- {name: 'members:read', group: organization administration, description: Read members., grantable_by: admin or owner}\n- {name: 'members:write', group: organization administration, description: Manage member roles., grantable_by: admin or owner}\n- {name: 'invites:read', group: organization administration, description: Read invitations., grantable_by: admin or owner}\n- {name: 'invites:write', group: organization administration, description: Create and revoke invitations., grantable_by: admin or owner}\n- {name: 'dispatches:read', group: organization administration, description: Read dispatch settings and delivery history.}\n- {name: 'dispatches:write', group: organization administration, description: 'Manage notifications, recipients and webhooks.', grantable_by: admin or owner}\nroles:\n- {name: member, description: Day-to-day work on the organization's tracked data.}\n- {name: admin, description:\
  \ Everything a member can, plus operations that change organization configuration or destructively affect shared resources.}\n- {name: owner, description: 'Everything an admin can, plus organization-lifecycle operations: transferring ownership and deleting the organization.'}\n"
source_yaml_url: https://artifacts.apis.io/competitortracker-io/scopes/competitortracker-io-scopes.yml
summary_line: 22 scopes
tags:
- Company
- Competitive Intelligence
- Competitor Tracking
- Website Change Monitoring
- Price Monitoring
- Market Intelligence
- MCP
- AI Agents
token_bound: false
token_urls: []
---
