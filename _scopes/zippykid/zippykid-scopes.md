---
api_specs:
- filename: zippykid-pressable-openapi-original.json
  format: json
  label: Pressable API
  slug: pressable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zippykid/refs/heads/main/openapi/zippykid-pressable-openapi-original.json
authorization_urls:
- https://my.pressable.com/auth/authorize
description: ''
docs: https://my.pressable.com/documentation/api/v1
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zippykid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ZippyKid publishes 13 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ZippyKid API on a user''s behalf.


  Tokens are issued from https://my.pressable.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ZippyKid
provider_slug: zippykid
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://my.pressable.com/auth/token
  name: OAuth2ClientCredentials
  source: https://my.pressable.com/documentation/api/v1/authentication.md
- flows:
  - authorizationUrl: https://my.pressable.com/auth/authorize
    flow: authorizationCode
    tokenUrl: https://my.pressable.com/auth/token
  name: MCPOAuth
  source: https://my.pressable.com/.well-known/oauth-authorization-server
scope_count: 13
scope_names:
- Account (Read)
- Account (Edit)
- Sites (Read)
- Sites (Edit)
- Collaborators (Read)
- Collaborators (Edit)
- Domains (Read)
- Domains (Edit)
- Git (Read)
- Git (Edit)
- admin
- owner
- mcp
scopes:
- description: Read account profile, settings, add-ons, and activity logs.
  flows:
  - clientCredentials
  scope: Account (Read)
- description: Modify account defaults (PHP version, datacenter) and add-ons.
  flows:
  - clientCredentials
  scope: Account (Edit)
- description: List and read managed site details, backups, logs, plugins, and themes.
  flows:
  - clientCredentials
  scope: Sites (Read)
- description: Create, update, delete, clone, enable/disable sites and manage plugins/themes/cache.
  flows:
  - clientCredentials
  scope: Sites (Edit)
- description: List collaborators and their site access.
  flows:
  - clientCredentials
  scope: Collaborators (Read)
- description: Add/remove collaborators and manage account- and site-level access.
  flows:
  - clientCredentials
  scope: Collaborators (Edit)
- description: List site domains and DNS zones/records.
  flows:
  - clientCredentials
  scope: Domains (Read)
- description: Add/remove domains, set primary domain, manage DNS records and SSL.
  flows:
  - clientCredentials
  scope: Domains (Edit)
- description: Read git configuration, branches, and deploy history.
  flows:
  - clientCredentials
  scope: Git (Read)
- description: Connect/disconnect repositories, store tokens, and trigger deployments.
  flows:
  - clientCredentials
  scope: Git (Edit)
- description: Administrative access across account resources.
  flows:
  - clientCredentials
  scope: admin
- description: Full owner-level access to all account resources.
  flows:
  - clientCredentials
  scope: owner
- description: Scope advertised by the MCP OAuth authorization server for agent access.
  flows:
  - authorizationCode
  scope: mcp
slug: zippykid-scopes
source_filename: zippykid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://my.pressable.com/documentation/api/v1/authentication.md\ndocs: https://my.pressable.com/documentation/api/v1\nschemes:\n- name: OAuth2ClientCredentials\n  source: https://my.pressable.com/documentation/api/v1/authentication.md\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://my.pressable.com/auth/token\n- name: MCPOAuth\n  source: https://my.pressable.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://my.pressable.com/auth/authorize\n    tokenUrl: https://my.pressable.com/auth/token\nscopes:\n# Permission-based scopes configured per access token in the control panel.\n- scope: Account (Read)\n  description: Read account profile, settings, add-ons, and activity logs.\n  flows: [clientCredentials]\n- scope: Account (Edit)\n  description: Modify account defaults (PHP version, datacenter) and add-ons.\n  flows: [clientCredentials]\n- scope: Sites\
  \ (Read)\n  description: List and read managed site details, backups, logs, plugins, and themes.\n  flows: [clientCredentials]\n- scope: Sites (Edit)\n  description: Create, update, delete, clone, enable/disable sites and manage plugins/themes/cache.\n  flows: [clientCredentials]\n- scope: Collaborators (Read)\n  description: List collaborators and their site access.\n  flows: [clientCredentials]\n- scope: Collaborators (Edit)\n  description: Add/remove collaborators and manage account- and site-level access.\n  flows: [clientCredentials]\n- scope: Domains (Read)\n  description: List site domains and DNS zones/records.\n  flows: [clientCredentials]\n- scope: Domains (Edit)\n  description: Add/remove domains, set primary domain, manage DNS records and SSL.\n  flows: [clientCredentials]\n- scope: Git (Read)\n  description: Read git configuration, branches, and deploy history.\n  flows: [clientCredentials]\n- scope: Git (Edit)\n  description: Connect/disconnect repositories, store tokens,\
  \ and trigger deployments.\n  flows: [clientCredentials]\n- scope: admin\n  description: Administrative access across account resources.\n  flows: [clientCredentials]\n- scope: owner\n  description: Full owner-level access to all account resources.\n  flows: [clientCredentials]\n- scope: mcp\n  description: Scope advertised by the MCP OAuth authorization server for agent access.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zippykid/refs/heads/main/scopes/zippykid-scopes.yml
summary_line: 13 scopes · clientCredentials/authorizationCode
tags:
- Company
- WordPress
- Managed Hosting
- WordPress Hosting
- Web Hosting
- WP Cloud
- MCP
- DevOps
token_urls:
- https://my.pressable.com/auth/token
---
