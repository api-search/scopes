---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clepit Scopes
name_suffix: OAuth Scopes
note: No scopes/permissions reference page is published in the clepit.com docs.
overview: 'Clepit publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clepit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clepit
provider_slug: clepit-com
schemes: []
scope_count: 3
scope_names:
- openid
- email
- urn:zitadel:iam:org:project:id:377023715914839692:aud
scopes:
- description: OpenID Connect sign-in (listed in scopes_supported of the MCP protected-resource metadata).
  flows: []
  scope: openid
- description: Email claim (listed in scopes_supported).
  flows: []
  scope: email
- description: Audience scope for the Bomdisoft identity project (listed in scopes_supported).
  flows: []
  scope: urn:zitadel:iam:org:project:id:377023715914839692:aud
slug: clepit-com-scopes
source_filename: clepit-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://api.clepit.com/.well-known/oauth-protected-resource\nscopes:\n- name: openid\n  description: OpenID Connect sign-in (listed in scopes_supported of the MCP protected-resource metadata).\n- name: email\n  description: Email claim (listed in scopes_supported).\n- name: 'urn:zitadel:iam:org:project:id:377023715914839692:aud'\n  description: Audience scope for the Bomdisoft identity project (listed in scopes_supported).\nnote: No scopes/permissions reference page is published in the clepit.com docs.\n"
source_yaml_url: https://artifacts.apis.io/clepit-com/scopes/clepit-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Block Editor
- Rich Text Editor
- Knowledge Base
- Open Source
- TypeScript
- JSON
- Collaboration
- Wiki
token_bound: false
token_urls: []
---
