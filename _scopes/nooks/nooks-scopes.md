---
api_specs:
- filename: nooks-accounts-api-openapi.yml
  format: yaml
  label: Nooks Accounts API
  slug: nooks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-accounts-api-openapi.yml
- filename: nooks-calldispositions-api-openapi.yml
  format: yaml
  label: Nooks Call Dispositions API
  slug: nooks-calldispositions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calldispositions-api-openapi.yml
- filename: nooks-calls-api-openapi.yml
  format: yaml
  label: Nooks Calls API
  slug: nooks-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-calls-api-openapi.yml
- filename: nooks-emails-api-openapi.yml
  format: yaml
  label: Nooks Emails API
  slug: nooks-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emails-api-openapi.yml
- filename: nooks-emailtemplates-api-openapi.yml
  format: yaml
  label: Nooks Email Templates API
  slug: nooks-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-emailtemplates-api-openapi.yml
- filename: nooks-introspection-api-openapi.yml
  format: yaml
  label: Nooks Introspection API
  slug: nooks-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-introspection-api-openapi.yml
- filename: nooks-mailboxes-api-openapi.yml
  format: yaml
  label: Nooks Mailboxes API
  slug: nooks-mailboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-mailboxes-api-openapi.yml
- filename: nooks-nooks-sequencing-api-api-openapi.yml
  format: yaml
  label: Nooks Nooks Sequencing API
  slug: nooks-nooks-sequencing-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-nooks-sequencing-api-api-openapi.yml
- filename: nooks-notes-api-openapi.yml
  format: yaml
  label: Nooks Notes API
  slug: nooks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-notes-api-openapi.yml
- filename: nooks-prospects-api-openapi.yml
  format: yaml
  label: Nooks Prospects API
  slug: nooks-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-prospects-api-openapi.yml
- filename: nooks-sequences-api-openapi.yml
  format: yaml
  label: Nooks Sequences API
  slug: nooks-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequences-api-openapi.yml
- filename: nooks-sequencestates-api-openapi.yml
  format: yaml
  label: Nooks Sequence States API
  slug: nooks-sequencestates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencestates-api-openapi.yml
- filename: nooks-sequencesteps-api-openapi.yml
  format: yaml
  label: Nooks Sequence Steps API
  slug: nooks-sequencesteps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-sequencesteps-api-openapi.yml
- filename: nooks-tasks-api-openapi.yml
  format: yaml
  label: Nooks Tasks API
  slug: nooks-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-tasks-api-openapi.yml
- filename: nooks-users-api-openapi.yml
  format: yaml
  label: Nooks Users API
  slug: nooks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/openapi/nooks-users-api-openapi.yml
authorization_urls:
- https://oauth.nooks.in/oauth/authorize
description: ''
docs: https://developer.nooks.in/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nooks Scopes
name_suffix: OAuth Scopes
note: 'derive-oauth-scopes.py found NO scopes: Nooks declares only a single `BearerAuth` http/bearer securityScheme in its OpenAPI and never models the OAuth flow as an `oauth2` scheme, so the mechanical pass had nothing to read. The scopes below are searched, not derived — 24 scopes published verbatim in `scopes_supported` of the live RFC 8414 authorization-server metadata, with descriptions taken from the scope table in the OpenAPI `info.description` Authentication section. Nothing here is inferred.'
overview: 'Nooks publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nooks API on a user''s behalf.


  Tokens are issued from https://oauth.nooks.in/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nooks
provider_slug: nooks
schemes:
- flows:
  - authorizationUrl: https://oauth.nooks.in/oauth/authorize
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://oauth.nooks.in/oauth/revoke
    tokenUrl: https://oauth.nooks.in/oauth/token
  issuer: https://oauth.nooks.in
  name: NooksOAuth2
  source: https://oauth.nooks.in/.well-known/oauth-authorization-server
  spec: RFC 8414 OAuth 2.0 Authorization Server Metadata
scope_count: 24
scope_names:
- prospects:read
- prospects:write
- sequences:read
- sequences:write
- sequence-steps:read
- sequence-states:read
- sequence-states:write
- tasks:read
- tasks:write
- calls:read
- calls:write
- call-dispositions:read
- emails:read
- emails:write
- email-templates:read
- mailboxes:read
- users:read
- accounts:read
- notes:write
- opportunities:read
- search:read
- coaching:read
- teams:read
- desktop-notes:read
scopes:
- description: View your prospects
  flows:
  - authorizationCode
  scope: prospects:read
- description: Create and update prospects
  flows:
  - authorizationCode
  scope: prospects:write
- description: View your sequences
  flows:
  - authorizationCode
  scope: sequences:read
- description: Create and update sequences
  flows:
  - authorizationCode
  scope: sequences:write
- description: View sequence steps
  flows:
  - authorizationCode
  scope: sequence-steps:read
- description: View sequence enrollments
  flows:
  - authorizationCode
  scope: sequence-states:read
- description: Enroll prospects and manage enrollments
  flows:
  - authorizationCode
  scope: sequence-states:write
- description: View your tasks
  flows:
  - authorizationCode
  scope: tasks:read
- description: Create, update, complete, skip, and delete tasks
  flows:
  - authorizationCode
  scope: tasks:write
- description: View your calls
  flows:
  - authorizationCode
  scope: calls:read
- description: Create and update calls
  flows:
  - authorizationCode
  scope: calls:write
- description: View call dispositions
  flows:
  - authorizationCode
  scope: call-dispositions:read
- description: View your emails
  flows:
  - authorizationCode
  scope: emails:read
- description: Create and update emails
  flows:
  - authorizationCode
  scope: emails:write
- description: View email templates
  flows:
  - authorizationCode
  scope: email-templates:read
- description: View connected mailboxes
  flows:
  - authorizationCode
  scope: mailboxes:read
- description: View users in your workspace
  flows:
  - authorizationCode
  scope: users:read
- description: View accounts (companies) in your workspace
  flows:
  - authorizationCode
  scope: accounts:read
- description: Create notes on CRM-backed prospects and accounts
  flows:
  - authorizationCode
  scope: notes:write
- description: View opportunities (deals) in your workspace
  flows:
  - authorizationCode
  scope: opportunities:read
- description: Search across your prospects, accounts, and other records
  flows:
  - authorizationCode
  scope: search:read
- description: Published in the live authorization-server metadata `scopes_supported`. Not listed in the OpenAPI scope table and has no corresponding REST operation in the published spec — read access to AI Coaching data, reachable via the MCP server.
  flows:
  - authorizationCode
  scope: coaching:read
- description: Published in the live authorization-server metadata `scopes_supported`. Not listed in the OpenAPI scope table and has no corresponding REST operation in the published spec.
  flows:
  - authorizationCode
  scope: teams:read
- description: Published in the live authorization-server metadata `scopes_supported`. Not listed in the OpenAPI scope table and has no corresponding REST operation in the published spec.
  flows:
  - authorizationCode
  scope: desktop-notes:read
slug: nooks-scopes
source_filename: nooks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://oauth.nooks.in/.well-known/oauth-authorization-server\ndocs: https://developer.nooks.in/\nnote: >-\n  derive-oauth-scopes.py found NO scopes: Nooks declares only a single `BearerAuth` http/bearer\n  securityScheme in its OpenAPI and never models the OAuth flow as an `oauth2` scheme, so the\n  mechanical pass had nothing to read. The scopes below are searched, not derived — 24 scopes\n  published verbatim in `scopes_supported` of the live RFC 8414 authorization-server metadata,\n  with descriptions taken from the scope table in the OpenAPI `info.description` Authentication\n  section. Nothing here is inferred.\nschemes:\n- name: NooksOAuth2\n  source: https://oauth.nooks.in/.well-known/oauth-authorization-server\n  spec: RFC 8414 OAuth 2.0 Authorization Server Metadata\n  issuer: https://oauth.nooks.in\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.nooks.in/oauth/authorize\n    tokenUrl:\
  \ https://oauth.nooks.in/oauth/token\n    revocationUrl: https://oauth.nooks.in/oauth/revoke\n    pkce: S256\nscope_count: 24\nscopes:\n- scope: prospects:read\n  description: View your prospects\n  flows: [authorizationCode]\n- scope: prospects:write\n  description: Create and update prospects\n  flows: [authorizationCode]\n- scope: sequences:read\n  description: View your sequences\n  flows: [authorizationCode]\n- scope: sequences:write\n  description: Create and update sequences\n  flows: [authorizationCode]\n- scope: sequence-steps:read\n  description: View sequence steps\n  flows: [authorizationCode]\n- scope: sequence-states:read\n  description: View sequence enrollments\n  flows: [authorizationCode]\n- scope: sequence-states:write\n  description: Enroll prospects and manage enrollments\n  flows: [authorizationCode]\n- scope: tasks:read\n  description: View your tasks\n  flows: [authorizationCode]\n- scope: tasks:write\n  description: Create, update, complete, skip, and delete tasks\n\
  \  flows: [authorizationCode]\n- scope: calls:read\n  description: View your calls\n  flows: [authorizationCode]\n- scope: calls:write\n  description: Create and update calls\n  flows: [authorizationCode]\n- scope: call-dispositions:read\n  description: View call dispositions\n  flows: [authorizationCode]\n- scope: emails:read\n  description: View your emails\n  flows: [authorizationCode]\n- scope: emails:write\n  description: Create and update emails\n  flows: [authorizationCode]\n- scope: email-templates:read\n  description: View email templates\n  flows: [authorizationCode]\n- scope: mailboxes:read\n  description: View connected mailboxes\n  flows: [authorizationCode]\n- scope: users:read\n  description: View users in your workspace\n  flows: [authorizationCode]\n- scope: accounts:read\n  description: View accounts (companies) in your workspace\n  flows: [authorizationCode]\n- scope: notes:write\n  description: Create notes on CRM-backed prospects and accounts\n  flows: [authorizationCode]\n\
  - scope: opportunities:read\n  description: View opportunities (deals) in your workspace\n  flows: [authorizationCode]\n- scope: search:read\n  description: Search across your prospects, accounts, and other records\n  flows: [authorizationCode]\n- scope: coaching:read\n  description: >-\n    Published in the live authorization-server metadata `scopes_supported`. Not listed in the\n    OpenAPI scope table and has no corresponding REST operation in the published spec — read\n    access to AI Coaching data, reachable via the MCP server.\n  flows: [authorizationCode]\n- scope: teams:read\n  description: >-\n    Published in the live authorization-server metadata `scopes_supported`. Not listed in the\n    OpenAPI scope table and has no corresponding REST operation in the published spec.\n  flows: [authorizationCode]\n- scope: desktop-notes:read\n  description: >-\n    Published in the live authorization-server metadata `scopes_supported`. Not listed in the\n    OpenAPI scope table and has no\
  \ corresponding REST operation in the published spec.\n  flows: [authorizationCode]\ndivergence:\n  note: >-\n    The authorization server publishes 24 scopes; the OpenAPI scope table documents 21. The three\n    extras (coaching:read, teams:read, desktop-notes:read) are a real surface divergence — they\n    grant access that the published REST contract does not describe, and are the strongest hint\n    that the MCP server at mcp.nooks.in reaches capabilities the REST API does not expose.\n  metadata_only:\n  - coaching:read\n  - teams:read\n  - desktop-notes:read\nx-evidence:\n- url: https://oauth.nooks.in/.well-known/oauth-authorization-server\n  status: 200\n- url: https://mcp.nooks.in/.well-known/oauth-protected-resource\n  status: 200\n- url: https://developer.nooks.in/openapi.yml\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nooks/refs/heads/main/scopes/nooks-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Sales Engagement
- Sales Dialer
- AI SDR
- Outbound Sales
- Sales Coaching
- Revenue Operations
- Sales Sequencing
- CRM Integration
- Agents
- MCP
token_urls:
- https://oauth.nooks.in/oauth/token
---
