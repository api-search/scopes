---
api_specs:
- filename: planable-campaigns-api-openapi.yml
  format: yaml
  label: Planable Campaigns API
  slug: planable-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-campaigns-api-openapi.yml
- filename: planable-competitors-api-openapi.yml
  format: yaml
  label: Planable Competitors API
  slug: planable-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-competitors-api-openapi.yml
- filename: planable-labels-api-openapi.yml
  format: yaml
  label: Planable Labels API
  slug: planable-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-labels-api-openapi.yml
- filename: planable-media-api-openapi.yml
  format: yaml
  label: Planable Media API
  slug: planable-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-media-api-openapi.yml
- filename: planable-members-api-openapi.yml
  format: yaml
  label: Planable Members API
  slug: planable-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-members-api-openapi.yml
- filename: planable-pages-api-openapi.yml
  format: yaml
  label: Planable Pages API
  slug: planable-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-pages-api-openapi.yml
- filename: planable-posts-api-openapi.yml
  format: yaml
  label: Planable Posts API
  slug: planable-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-posts-api-openapi.yml
- filename: planable-social-listening-api-openapi.yml
  format: yaml
  label: Planable Social Listening API
  slug: planable-social-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-social-listening-api-openapi.yml
- filename: planable-stories-api-openapi.yml
  format: yaml
  label: Planable Stories API
  slug: planable-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-stories-api-openapi.yml
- filename: planable-system-api-openapi.yml
  format: yaml
  label: Planable System API
  slug: planable-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-system-api-openapi.yml
- filename: planable-workspaces-api-openapi.yml
  format: yaml
  label: Planable Workspaces API
  slug: planable-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/openapi/planable-workspaces-api-openapi.yml
authorization_urls: []
description: ''
docs: https://planable.io/guides/planable-public-api/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Planable Scopes
name_suffix: OAuth Scopes
note: Planable runs TWO distinct authorization models and they do not share a scope vocabulary. The REST Public API uses opaque `pln_` bearer tokens with a two-value scope (read / write) chosen in the UI at token-creation time — no OAuth flow, no scope parameter, so derive-oauth-scopes.py correctly found no oauth2 securityScheme in the OpenAPI. The MCP server is a real OAuth 2.0 protected resource and publishes six scopes in its RFC 8414 metadata. Both are recorded below.
overview: 'Planable uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Planable
provider_slug: planable
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: planable-scopes
source_filename: planable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.planable.io/.well-known/oauth-authorization-server\ndocs: https://planable.io/guides/planable-public-api/\nnote: >-\n  Planable runs TWO distinct authorization models and they do not share a scope vocabulary.\n  The REST Public API uses opaque `pln_` bearer tokens with a two-value scope (read / write) chosen\n  in the UI at token-creation time — no OAuth flow, no scope parameter, so derive-oauth-scopes.py\n  correctly found no oauth2 securityScheme in the OpenAPI. The MCP server is a real OAuth 2.0\n  protected resource and publishes six scopes in its RFC 8414 metadata. Both are recorded below.\n\nsurfaces:\n  - surface: mcp\n    model: oauth2\n    issuer: https://mcp.planable.io/\n    resource: https://mcp.planable.io/mcp\n    metadata_file: well-known/planable-oauth-authorization-server.json\n    protected_resource_file: well-known/planable-oauth-protected-resource.json\n    grant_types: [authorization_code, refresh_token]\n\
  \    pkce: S256\n    dynamic_client_registration: https://mcp.planable.io/oauth/register\n    scopes:\n      - name: read\n        description: >-\n          Read account structure and content — companies, workspaces, connected pages, members,\n          labels, posts, comments and media. (Description derived from Planable's published MCP\n          capability map; the metadata document lists scope names only.)\n        published_description: false\n      - name: approve\n        description: Act on the approval workflow — approve, reject and disapprove posts, including multi-level flows.\n        published_description: false\n      - name: edit\n        description: Create and update draft content — posts, grouped posts, labels, internal notes, comments.\n        published_description: false\n      - name: publish\n        description: >-\n          Publishing-adjacent actions. Planable states plainly that agent-created content always\n          lands as a draft and cannot bypass the\
  \ approval and scheduling flow, so this scope does\n          not grant direct publication.\n        published_description: false\n      - name: analyze\n        description: Pull page-level and post-level metrics and trigger metric refreshes. Requires the workspace Analytics add-on.\n        published_description: false\n      - name: engage\n        description: Comment and inbox-side engagement surfaces. Requires the workspace Social Inbox add-on.\n        published_description: false\n  - surface: rest\n    model: bearer-token\n    token_prefix: pln_\n    header: 'Authorization: Bearer pln_...'\n    scopes:\n      - name: read\n        description: Fetch workspaces, pages, posts, media, labels and analytics. Cannot create or modify anything.\n        published_description: true\n      - name: write\n        description: Create and update content. Write implies read.\n        published_description: true\n    additional_access_dimension:\n      name: workspace access\n      description:\
  \ >-\n        Independent of scope, a token is scoped to all company workspaces or to an explicit subset\n        chosen at creation. Planable frames this as blast-radius control.\n    token_policy:\n      who_can_create: Company Owners and Administrators only (not delegatable)\n      max_active_tokens_per_company: 10\n      expiry_options: [30 days, 60 days, 90 days, 6 months, 1 year, Never]\n      rotation: manual — generate new, update the tool, revoke the old; no automated rotation in v1\n      revocation: immediate; revoked tokens are removed and cannot be restored\n      visibility: all Owners/Admins see all company tokens; there is no per-user token isolation\n\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n    - url: https://api.planable.io/.well-known/oauth-authorization-server\n      http_status: 200\n    - url: https://api.planable.io/.well-known/oauth-protected-resource/mcp\n      http_status: 200\n    - url: https://planable.io/guides/planable-public-api/\n      http_status:\
  \ 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planable/refs/heads/main/scopes/planable-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Social-Media
- Content Collaboration
- Approval Workflows
- Social Media Management
- Content Publishing
- Marketing
- Social Media Analytics
- Social Listening
- MCP
- AI Agents
- Agent Skills
token_urls: []
---
