---
authorization_urls: []
description: ''
docs: https://cloudcrane.ai/docs/connect
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CloudCrane Scopes
name_suffix: OAuth Scopes
note: Scope names from scopes_supported in both discovery documents. The docs publish no per-scope reference; descriptions below are our reading of the scope names against what the docs say an assistant may do; they are not provider-published per-scope text. The troubleshooting page notes a read-only connection ("This connection can only read apps") is a legacy choice that must be reconnected.
overview: 'CloudCrane publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CloudCrane API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CloudCrane
provider_slug: cloudcrane-ai
schemes: []
scope_count: 2
scope_names:
- apps:read
- apps:write
scopes:
- description: Read the workspace's apps (list, code, blueprints, versions).
  flows: []
  scope: apps:read
- description: 'Make, change, roll back and delete the workspace''s apps (docs: "see, make, change, roll back and delete your apps").'
  flows: []
  scope: apps:write
slug: cloudcrane-ai-scopes
source_filename: cloudcrane-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource:\n- https://cloudcrane.ai/.well-known/oauth-protected-resource\n- https://cloudcrane.ai/.well-known/oauth-authorization-server\ndocs: https://cloudcrane.ai/docs/connect\nnote: Scope names from scopes_supported in both discovery documents. The docs publish no per-scope reference; descriptions below are our reading of the scope names against what the docs say an assistant may do; they are not provider-published per-scope text. The troubleshooting page notes a read-only connection (\"This connection can only read apps\") is a legacy choice that must be reconnected.\nscopes:\n- name: apps:read\n  description: Read the workspace's apps (list, code, blueprints, versions).\n- name: apps:write\n  description: 'Make, change, roll back and delete the workspace''s apps (docs: \"see, make, change, roll back and delete your apps\").'\n"
source_yaml_url: https://artifacts.apis.io/cloudcrane-ai/scopes/cloudcrane-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- AI Assistant
- MCP
- Mobile App
- No-Code
- App Builder
- Progressive Web Apps
token_bound: false
token_urls: []
---
