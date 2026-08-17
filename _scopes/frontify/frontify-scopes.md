---
authorization_urls: []
description: 'Frontify runs two distinct OAuth surfaces with two distinct scope vocabularies, and they must not be conflated: (1) FRONTIFY INSTANCE OAuth — the authorization-code flow against https://{instance}.frontify.com/api/oauth/authorize, used by the Frontify Authenticator, Finder, Brand SDK apps and any custom integration. Its scopes are the `basic:*` / `account:*` / `blocks:*` / `webhooks:*` family below. (2) MCP SERVER OAuth — the authorization server embedded in the hosted MCP server at mcp.frontify-integrations.com, whose own RFC 8414 metadata declares a single scope, `mcp:tools`. That token is what an MCP client obtains; the server then brokers to the instance under the pack''s Frontify scopes.'
docs: https://developer.frontify.com/d/wJcTnsuhwb6T/about-1
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Frontify Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Frontify publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Frontify API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Frontify
provider_slug: frontify
schemes:
- authorizationUrl: https://{instance}.frontify.com/api/oauth/authorize
  flow: authorizationCode
  name: Frontify instance OAuth 2.0
  note: Instance-scoped. Client ID / Client Secret are issued by creating an OAuth application in the Frontify instance's Developer settings. The exact scope set requested at app-creation time must match the set used at authorization time.
  type: oauth2
- authorizationUrl: https://mcp.frontify-integrations.com/oauth/authorize
  client_id_metadata_document_supported: true
  dynamic_client_registration: true
  flow: authorizationCode
  name: Frontify MCP Server authorization server
  pkce: S256
  registrationUrl: https://mcp.frontify-integrations.com/oauth/register
  source: well-known/frontify-oauth-authorization-server.json
  tokenUrl: https://mcp.frontify-integrations.com/oauth/token
  type: oauth2
scope_count: 8
scope_names:
- basic:read
- basic:write
- account:read
- blocks:read
- webhooks:read
- webhooks:write
- mcp:tools
- openid
scopes:
- description: Read access to core Frontify objects — brands, libraries, projects, folders, assets and their metadata. Always active; the minimum scope for any integration.
  flows: []
  scope: basic:read
- description: Write access to core Frontify objects — create/update assets, tags, custom metadata, collections, folders, comments and workflow tasks.
  flows: []
  scope: basic:write
- description: Read access to account-level information (account id, account settings, users).
  flows: []
  scope: account:read
- description: Read access to guideline content blocks — brand portals, guideline pages and the blocks/sections inside them.
  flows: []
  scope: blocks:read
- description: Read access to installed webhooks.
  flows: []
  scope: webhooks:read
- description: Install, configure and uninstall webhooks.
  flows: []
  scope: webhooks:write
- description: The single scope advertised by the hosted MCP server's authorization server and required on the bearer token an MCP client presents to https://mcp.frontify-integrations.com/mcp.
  flows: []
  scope: mcp:tools
- description: Advertised in the MCP authorization server's OIDC-shaped discovery document only.
  flows: []
  scope: openid
slug: frontify-scopes
source_filename: frontify-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://mcp.frontify-integrations.com/mcp/packs/admin (Frontify's own MCP pack pages\n  publish the exact Frontify OAuth scopes each pack requests) +\n  well-known/frontify-oauth-authorization-server.json +\n  well-known/frontify-oauth-protected-resource.json +\n  third-party integration docs that enumerate required Frontify scopes\n  (docs.elastic.io/components/frontify, docs.squiz.net Frontify connector)\ndocs: https://developer.frontify.com/d/wJcTnsuhwb6T/about-1\ndescription: >-\n  Frontify runs two distinct OAuth surfaces with two distinct scope vocabularies, and\n  they must not be conflated:\n  (1) FRONTIFY INSTANCE OAuth — the authorization-code flow against\n  https://{instance}.frontify.com/api/oauth/authorize, used by the Frontify\n  Authenticator, Finder, Brand SDK apps and any custom integration. Its scopes are the\n  `basic:*` / `account:*` / `blocks:*` / `webhooks:*` family below.\n  (2) MCP SERVER OAuth\
  \ — the authorization server embedded in the hosted MCP server at\n  mcp.frontify-integrations.com, whose own RFC 8414 metadata declares a single scope,\n  `mcp:tools`. That token is what an MCP client obtains; the server then brokers to the\n  instance under the pack's Frontify scopes.\nschemes:\n  - name: Frontify instance OAuth 2.0\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://{instance}.frontify.com/api/oauth/authorize\n    note: >-\n      Instance-scoped. Client ID / Client Secret are issued by creating an OAuth\n      application in the Frontify instance's Developer settings. The exact scope set\n      requested at app-creation time must match the set used at authorization time.\n  - name: Frontify MCP Server authorization server\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://mcp.frontify-integrations.com/oauth/authorize\n    tokenUrl: https://mcp.frontify-integrations.com/oauth/token\n    registrationUrl: https://mcp.frontify-integrations.com/oauth/register\n\
  \    pkce: S256\n    dynamic_client_registration: true\n    client_id_metadata_document_supported: true\n    source: well-known/frontify-oauth-authorization-server.json\nscopes:\n  - scope: basic:read\n    surface: frontify-instance\n    description: >-\n      Read access to core Frontify objects — brands, libraries, projects, folders,\n      assets and their metadata. Always active; the minimum scope for any integration.\n    evidence: requested by every MCP pack; documented as always-active / minimum by integration vendors\n  - scope: basic:write\n    surface: frontify-instance\n    description: >-\n      Write access to core Frontify objects — create/update assets, tags, custom\n      metadata, collections, folders, comments and workflow tasks.\n    evidence: requested by the admin, collaboration, asset-organization, asset-creation, creative-automation, workflow-automation, brand-admin and bulk-operations MCP packs\n  - scope: account:read\n    surface: frontify-instance\n    description:\
  \ Read access to account-level information (account id, account settings, users).\n    evidence: requested by the admin MCP pack\n  - scope: blocks:read\n    surface: frontify-instance\n    description: >-\n      Read access to guideline content blocks — brand portals, guideline pages and the\n      blocks/sections inside them.\n    evidence: requested by the admin, discovery and brand-portal MCP packs\n  - scope: webhooks:read\n    surface: frontify-instance\n    description: Read access to installed webhooks.\n    evidence: named as a required scope for Frontify webhook operations in third-party connector documentation\n    confidence: medium\n  - scope: webhooks:write\n    surface: frontify-instance\n    description: Install, configure and uninstall webhooks.\n    evidence: named as a required scope for Frontify webhook operations in third-party connector documentation\n    confidence: medium\n  - scope: mcp:tools\n    surface: frontify-mcp-server\n    description: >-\n      The single\
  \ scope advertised by the hosted MCP server's authorization server and\n      required on the bearer token an MCP client presents to\n      https://mcp.frontify-integrations.com/mcp.\n    evidence: >-\n      well-known/frontify-oauth-authorization-server.json scopes_supported;\n      well-known/frontify-oauth-protected-resource.json scopes_supported; and the\n      WWW-Authenticate challenge on an anonymous tools/list POST\n      (`Bearer resource_metadata=\"...\", scope=\"mcp:tools\"`)\n  - scope: openid\n    surface: frontify-mcp-server\n    description: Advertised in the MCP authorization server's OIDC-shaped discovery document only.\n    evidence: well-known/frontify-openid-configuration.json scopes_supported\nscope_to_pack:\n  admin: [basic:read, basic:write, account:read, blocks:read]\n  discovery: [basic:read, blocks:read]\n  collaboration: [basic:read, basic:write]\n  asset-organization: [basic:read, basic:write]\n  asset-creation: [basic:read, basic:write]\n  creative-automation:\
  \ [basic:read, basic:write]\n  workflow-automation: [basic:read, basic:write]\n  brand-admin: [basic:read, basic:write]\n  brand-portal: [basic:read, blocks:read]\n  bulk-operations: [basic:read, basic:write]\ngaps:\n  - >-\n    Frontify does not publish a single canonical scopes reference page on a readable\n    host — the developer portal is a JS-rendered SPA. The vocabulary above is assembled\n    from Frontify's own MCP pack pages (which print the scopes verbatim), Frontify's own\n    OAuth AS metadata, and third-party connector docs. Scope strings marked\n    confidence: medium were not observed on a Frontify-served surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frontify/refs/heads/main/scopes/frontify-scopes.yml
summary_line: 8 scopes
tags:
- Company
- Marketing
- Brand Management
- Digital Asset Management
- DAM
- Content
- GraphQL
- Creative Operations
token_urls: []
---
