---
api_specs:
- filename: ironfang-account-api-openapi.yml
  format: yaml
  label: Ironfang Account API
  slug: ironfang-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-account-api-openapi.yml
- filename: ironfang-batches-api-openapi.yml
  format: yaml
  label: Ironfang Batches API
  slug: ironfang-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-batches-api-openapi.yml
- filename: ironfang-destinations-api-openapi.yml
  format: yaml
  label: Ironfang Destinations API
  slug: ironfang-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-destinations-api-openapi.yml
- filename: ironfang-jobs-api-openapi.yml
  format: yaml
  label: Ironfang Jobs API
  slug: ironfang-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-jobs-api-openapi.yml
- filename: ironfang-render-api-openapi.yml
  format: yaml
  label: Ironfang Render API
  slug: ironfang-render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-render-api-openapi.yml
- filename: ironfang-signed-urls-api-openapi.yml
  format: yaml
  label: Ironfang Signed URLs API
  slug: ironfang-signed-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-signed-urls-api-openapi.yml
- filename: ironfang-templates-api-openapi.yml
  format: yaml
  label: Ironfang Templates API
  slug: ironfang-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/openapi/ironfang-templates-api-openapi.yml
authorization_urls: []
description: ''
docs:
- https://ironfang.uk/docs/mcp
- https://ironfang.uk/renderwolf/docs#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ironfang Scopes
name_suffix: OAuth Scopes
note: 'derive-oauth-scopes.py found no oauth2 securityScheme in the OpenAPI - the published contract declares only the apiKey bearer scheme, so nothing was derivable. Every scope below was read from Ironfang''s own published scope tables. Two scope systems share one vocabulary: API-key scopes chosen at key creation (REST), and OAuth scopes granted at MCP consent.'
overview: 'Ironfang uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ironfang
provider_slug: ironfang
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ironfang-scopes
source_filename: ironfang-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://ironfang.uk/docs/mcp\ndocs:\n  - https://ironfang.uk/docs/mcp\n  - https://ironfang.uk/renderwolf/docs#scopes\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme in the OpenAPI - the published contract\n  declares only the apiKey bearer scheme, so nothing was derivable. Every scope below was read\n  from Ironfang's own published scope tables. Two scope systems share one vocabulary: API-key\n  scopes chosen at key creation (REST), and OAuth scopes granted at MCP consent.\nauthorization_server: https://id.ironfang.uk\nadvertised_at:\n  - well-known/ironfang-oauth-authorization-server.json\n  - well-known/ironfang-oauth-protected-resource.json\nadvertised_scopes_note: >-\n  The two discovery documents advertise only three scopes (ironfang:mcp, renderwolf:render,\n  renderwolf:usage:read). The MCP reference documents six more that the metadata does not list.\nscopes:\n  - name: 'ironfang:mcp'\n    description:\
  \ Connect, list tools, and inspect this connection and its budgets.\n    requires_permission: membership\n    surfaces: [mcp]\n    advertised_in_metadata: true\n  - name: 'renderwolf:render'\n    description: >-\n      Create screenshots, PDFs, QR codes, template renders, clips and site previews; read or\n      cancel its own jobs.\n    requires_permission: render\n    surfaces: [rest, mcp]\n    advertised_in_metadata: true\n  - name: 'renderwolf:usage:read'\n    description: Read the period's credit usage.\n    requires_permission: usage.read\n    surfaces: [rest, mcp]\n    advertised_in_metadata: true\n  - name: 'renderwolf:sign'\n    description: Create signed render URLs. Through MCP they must expire within 24 hours.\n    requires_permission: render\n    surfaces: [rest, mcp]\n    advertised_in_metadata: false\n  - name: 'renderwolf:templates:read'\n    description: List templates and their variable names - never the stored markup.\n    requires_permission: templates.read\n    surfaces:\
  \ [rest, mcp]\n    advertised_in_metadata: false\n  - name: 'renderwolf:templates:write'\n    description: Create, edit and delete templates.\n    requires_permission: templates.write\n    surfaces: [rest]\n    advertised_in_metadata: false\n    note: REST API-key scope only; not exposed as an MCP tool scope.\n  - name: 'renderwolf:destinations'\n    description: >-\n      Register and test delivery destinations, and name a destination on a job or batch.\n      Storage destinations carrying credentials are registered in the portal, not by an agent.\n    requires_permission: destinations.manage\n    surfaces: [rest, mcp]\n    advertised_in_metadata: false\n  - name: 'auditwolf:read'\n    description: Read sites, audits, findings and rules.\n    requires_permission: auditwolf.read\n    surfaces: [mcp]\n    advertised_in_metadata: false\n    note: Sibling product (Auditwolf). Reserved - tools not yet available.\n  - name: 'auditwolf:run'\n    description: Start a manual audit of a site within\
  \ its page bound and the connection budget.\n    requires_permission: auditwolf.run\n    surfaces: [mcp]\n    advertised_in_metadata: false\n    note: Sibling product (Auditwolf). Reserved - tools not yet available.\n  - name: 'auditwolf:evidence'\n    description: See where an audit's signed evidence bundle is and how to verify it.\n    requires_permission: auditwolf.evidence\n    surfaces: [mcp]\n    advertised_in_metadata: false\n    note: Sibling product (Auditwolf). Reserved - tools not yet available.\nsemantics:\n  ungranted_tool_behavior: >-\n    A tool whose scope was not granted is still listed so a client can ask for it; the call\n    answers 403 with the complete scope set in the challenge, and the client re-runs the flow\n    for the extra scope.\n  api_key_scopes_immutable: >-\n    API-key scopes cannot be widened after creation - broader access requires a new key.\n  legacy_keys: Keys created before scopes existed carry no scopes and retain full access.\n  revocation: >-\n\
  \    Scopes are re-checked live against the organisation permission on every call; losing a\n    permission ends the access the same minute.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironfang/refs/heads/main/scopes/ironfang-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Developer Tools
- screenshot-api
- website screenshot
- HTML to PDF
- PDF API
- Image API
- OG Image API
- QR Code API
- Website-to-Video
- Rendering Infrastructure
- MCP
- UK-hosted
token_urls: []
---
