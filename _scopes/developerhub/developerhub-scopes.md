---
api_specs:
- filename: developerhub-documentation-api-openapi.yml
  format: yaml
  label: DeveloperHub Documentation API
  slug: developerhub-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-documentation-api-openapi.yml
- filename: developerhub-pages-api-openapi.yml
  format: yaml
  label: DeveloperHub Pages API
  slug: developerhub-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-pages-api-openapi.yml
- filename: developerhub-project-api-openapi.yml
  format: yaml
  label: DeveloperHub Project API
  slug: developerhub-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-project-api-openapi.yml
- filename: developerhub-reader-access-api-openapi.yml
  format: yaml
  label: DeveloperHub Reader Access API
  slug: developerhub-reader-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-reader-access-api-openapi.yml
- filename: developerhub-references-api-openapi.yml
  format: yaml
  label: DeveloperHub References API
  slug: developerhub-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-references-api-openapi.yml
- filename: developerhub-versions-api-openapi.yml
  format: yaml
  label: DeveloperHub Versions API
  slug: developerhub-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-versions-api-openapi.yml
- filename: developerhub-changelog-api-openapi.yml
  format: yaml
  label: DeveloperHub Changelog API
  slug: developerhub-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-changelog-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Developerhub Scopes
name_suffix: OAuth Scopes
note: 'The REST API declares no OAuth flows — it is X-Api-Key only. OAuth exists on exactly one surface: the hosted Editor MCP server at https://ai.developerhub.io/mcp, whose RFC 8414 / RFC 9728 discovery documents are served anonymously and declare a single scope. Alongside that, API keys carry a separate, finer-grained permission vocabulary that the OpenAPI names per operation; those are recorded here as api_key_permissions because they are not OAuth scopes.'
overview: 'DeveloperHub uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DeveloperHub
provider_slug: developerhub
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: developerhub-scopes
source_filename: developerhub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  https://ai.developerhub.io/.well-known/oauth-authorization-server and\n  https://ai.developerhub.io/.well-known/oauth-protected-resource , fetched 2026-09-06;\n  permission names read from https://docs.developerhub.io/api.md\nprovider: DeveloperHub\nproviderId: developerhub\nnote: >-\n  The REST API declares no OAuth flows — it is X-Api-Key only. OAuth exists on exactly one surface:\n  the hosted Editor MCP server at https://ai.developerhub.io/mcp, whose RFC 8414 / RFC 9728\n  discovery documents are served anonymously and declare a single scope. Alongside that, API keys\n  carry a separate, finer-grained permission vocabulary that the OpenAPI names per operation; those\n  are recorded here as api_key_permissions because they are not OAuth scopes.\nauthorization_server:\n  issuer: https://ai.developerhub.io/\n  authorization_endpoint: https://ai.developerhub.io/authorize\n  token_endpoint: https://ai.developerhub.io/token\n\
  \  registration_endpoint: https://ai.developerhub.io/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\n  dynamic_client_registration: true\n  document: well-known/developerhub-oauth-authorization-server.json\nprotected_resource:\n  resource: https://ai.developerhub.io/\n  resource_name: DeveloperHub\n  authorization_servers:\n  - https://ai.developerhub.io/\n  document: well-known/developerhub-oauth-protected-resource.json\nscope_count: 1\nscopes:\n- name: editor\n  description: >-\n    Act as the signed-in DeveloperHub editor on the Editor MCP server. The agent reaches only the\n    projects that person can already edit, and only those with the Editor MCP server turned on.\n  surface: https://ai.developerhub.io/mcp\n  source: oauth-authorization-server + oauth-protected-resource metadata\napi_key_permissions:\n\
  \  note: >-\n    Separate from OAuth. The OpenAPI names a permission on individual operations; only the changelog\n    operations state one explicitly, and no published permissions reference page enumerates the rest.\n  documented:\n  - name: changelog.edit\n    operations:\n    - create_changelog_post\n  - name: changelog.read\n    operations:\n    - list_changelog_posts\n  undocumented_note: >-\n    https://docs.developerhub.io/support-center/api-key says \"Each API Key can have different\n    permissions. Consult the API to know which permissions you need\", so the full permission\n    vocabulary is only visible in the key-creation UI.\n  docs: https://docs.developerhub.io/support-center/api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/scopes/developerhub-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Reference
- Developer Portals
- Documentation
- Knowledge Base
- OpenAPI
- Docs as Code
- Model Context Protocol
- Agent Skills
token_urls: []
---
