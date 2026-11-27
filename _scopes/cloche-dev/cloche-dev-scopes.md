---
authorization_urls: []
description: ''
docs: https://cloche.dev/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cloche Scopes
name_suffix: OAuth Scopes
note: Cloche's auth.md defers scopes to the authorization-server metadata ("the metadata is the truth"). Only standard OIDC scopes are advertised; no Cloche-specific resource scopes are published.
overview: 'Cloche publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloche API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloche
provider_slug: cloche-dev
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in.
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Issue a refresh token.
  flows: []
  scope: offline_access
slug: cloche-dev-scopes
source_filename: cloche-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://sleek-marigold-65.authkit.app/.well-known/oauth-authorization-server\ndocs: https://cloche.dev/auth.md\nname: Cloche OAuth scopes\nnote: Cloche's auth.md defers scopes to the authorization-server metadata (\"the metadata is the truth\"). Only standard OIDC scopes are advertised; no Cloche-specific resource scopes are published.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in.\n- name: profile\n  description: Basic profile claims.\n- name: email\n  description: Email address claim.\n- name: offline_access\n  description: Issue a refresh token.\n"
source_yaml_url: https://artifacts.apis.io/cloche-dev/scopes/cloche-dev-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Artificial Intelligence
- MCP
- Ai Apps
- Governance
- Low-Code
- Internal Tools
- Agents
token_bound: false
token_urls: []
---
