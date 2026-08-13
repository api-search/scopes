---
authorization_urls: []
description: The OAuth 2.0 scopes involve.me publishes for its Model Context Protocol server. These are read straight off RFC 8414 authorization-server metadata, so they are the provider's own values — but note that no human-readable scope reference page exists anywhere on involve.me, help.involve.me, or any developer site. The descriptions below are marked derived and are inferred from Statamic CMS resource naming; they are NOT provider-authored text.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Involve Me Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'involve.me publishes 21 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the involve.me API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: involve.me
provider_slug: involve-me
schemes: []
scope_count: 21
scope_names:
- '*'
- content:read
- content:write
- entries:read
- entries:write
- structures:read
- structures:write
- assets:read
- assets:write
- users:read
- users:write
- system:read
- system:write
- blueprints:read
- blueprints:write
- terms:read
- terms:write
- globals:read
- globals:write
- content-facade:read
- content-facade:write
scopes:
- description: Wildcard — full access to every resource family below.
  flows: []
  scope: '*'
- description: Read CMS content across all content types.
  flows: []
  scope: content:read
- description: Create, update and delete CMS content.
  flows: []
  scope: content:write
- description: Read Statamic entries (individual pages, blog posts, templates).
  flows: []
  scope: entries:read
- description: Create, update and delete Statamic entries.
  flows: []
  scope: entries:write
- description: Read navigation structures and content trees.
  flows: []
  scope: structures:read
- description: Modify navigation structures and content trees.
  flows: []
  scope: structures:write
- description: Read media assets and asset containers.
  flows: []
  scope: assets:read
- description: Upload, replace and delete media assets.
  flows: []
  scope: assets:write
- description: Read CMS user accounts and roles.
  flows: []
  scope: users:read
- description: Create, update and delete CMS user accounts.
  flows: []
  scope: users:write
- description: Read CMS system configuration and site settings.
  flows: []
  scope: system:read
- description: Modify CMS system configuration and site settings.
  flows: []
  scope: system:write
- description: Read Statamic blueprints and fieldsets (the content schema).
  flows: []
  scope: blueprints:read
- description: Modify Statamic blueprints and fieldsets.
  flows: []
  scope: blueprints:write
- description: Read taxonomy terms.
  flows: []
  scope: terms:read
- description: Create, update and delete taxonomy terms.
  flows: []
  scope: terms:write
- description: Read global content sets shared across the site.
  flows: []
  scope: globals:read
- description: Modify global content sets.
  flows: []
  scope: globals:write
- description: Read content through the Statamic content facade abstraction.
  flows: []
  scope: content-facade:read
- description: Write content through the Statamic content facade abstraction.
  flows: []
  scope: content-facade:write
slug: involve-me-scopes
source_filename: involve-me-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://www.involve.me/.well-known/oauth-authorization-server (HTTP 200,\n  application/json) — scopes_supported, read verbatim. Corroborated by\n  https://www.involve.me/.well-known/oauth-protected-resource (HTTP 200), which\n  publishes the identical list for the protected resource\n  https://www-cdn.involve.me/mcp/statamic.\ndescription: >-\n  The OAuth 2.0 scopes involve.me publishes for its Model Context Protocol server.\n  These are read straight off RFC 8414 authorization-server metadata, so they are\n  the provider's own values — but note that no human-readable scope reference page\n  exists anywhere on involve.me, help.involve.me, or any developer site. The\n  descriptions below are marked derived and are inferred from Statamic CMS resource\n  naming; they are NOT provider-authored text.\n\nauthorization_server: https://www-cdn.involve.me\nprotected_resource: https://www-cdn.involve.me/mcp/statamic\ndocs: null\n\
  docs_note: >-\n  involve.me publishes no scopes/permissions reference. There is no developer\n  portal (developers.involve.me and docs.involve.me both 302 to the marketing\n  homepage). The only public record of these scopes is the .well-known metadata\n  document itself.\n\npkce_required: S256\ngrant_types: [authorization_code, refresh_token]\nscope_count: 20\n\nscopes:\n  - scope: '*'\n    description_method: provider\n    description: Wildcard — full access to every resource family below.\n    risk: high\n\n  - scope: content:read\n    description_method: derived\n    description: Read CMS content across all content types.\n  - scope: content:write\n    description_method: derived\n    description: Create, update and delete CMS content.\n\n  - scope: entries:read\n    description_method: derived\n    description: Read Statamic entries (individual pages, blog posts, templates).\n  - scope: entries:write\n    description_method: derived\n    description: Create, update and delete Statamic\
  \ entries.\n\n  - scope: structures:read\n    description_method: derived\n    description: Read navigation structures and content trees.\n  - scope: structures:write\n    description_method: derived\n    description: Modify navigation structures and content trees.\n\n  - scope: assets:read\n    description_method: derived\n    description: Read media assets and asset containers.\n  - scope: assets:write\n    description_method: derived\n    description: Upload, replace and delete media assets.\n\n  - scope: users:read\n    description_method: derived\n    description: Read CMS user accounts and roles.\n    risk: high\n  - scope: users:write\n    description_method: derived\n    description: Create, update and delete CMS user accounts.\n    risk: high\n\n  - scope: system:read\n    description_method: derived\n    description: Read CMS system configuration and site settings.\n  - scope: system:write\n    description_method: derived\n    description: Modify CMS system configuration and\
  \ site settings.\n    risk: high\n\n  - scope: blueprints:read\n    description_method: derived\n    description: Read Statamic blueprints and fieldsets (the content schema).\n  - scope: blueprints:write\n    description_method: derived\n    description: Modify Statamic blueprints and fieldsets.\n\n  - scope: terms:read\n    description_method: derived\n    description: Read taxonomy terms.\n  - scope: terms:write\n    description_method: derived\n    description: Create, update and delete taxonomy terms.\n\n  - scope: globals:read\n    description_method: derived\n    description: Read global content sets shared across the site.\n  - scope: globals:write\n    description_method: derived\n    description: Modify global content sets.\n\n  - scope: content-facade:read\n    description_method: derived\n    description: Read content through the Statamic content facade abstraction.\n  - scope: content-facade:write\n    description_method: derived\n    description: Write content through the\
  \ Statamic content facade abstraction.\n\nfindings:\n  - >-\n    A wildcard '*' scope is offered alongside the granular pairs. An agent that\n    requests '*' receives write access to users and system configuration; there is\n    no published guidance steering integrators toward least privilege.\n  - >-\n    Every family is offered as a read/write pair with no finer granularity, so\n    there is no way to grant, for example, publish-without-delete.\n  - >-\n    These scopes govern the marketing website's CMS only. No OAuth scope surface\n    exists for the involve.me funnel product's own data (funnels, submissions,\n    participants, contacts).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/involve-me/refs/heads/main/scopes/involve-me-scopes.yml
summary_line: 21 scopes
tags:
- Company
- Marketing
- Lead Generation
- Forms
- Surveys
- Quizzes
- No-Code
- Email Marketing
- CRM
- Webhooks
- Model Context Protocol
- Austria
token_urls: []
---
