---
authorization_urls: []
description: ''
docs: https://www.onescreen.ai/mcp/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Onescreen Ai Scopes
name_suffix: OAuth Scopes
note: 'Not derived from an OpenAPI — OneScreen publishes no REST contract. These scopes are read verbatim from the two anonymous OAuth discovery documents the MCP host serves: the RFC 8414 authorization-server metadata (22 scopes) and the RFC 9728 protected-resource metadata for https://mcp.onescreen.ai/mcp (18 scopes). Descriptions are ours, inferred from the scope name and the provider''s published product description; the scope STRINGS are the provider''s.'
overview: 'OneScreen AI publishes 22 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the OneScreen AI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OneScreen AI
provider_slug: onescreen-ai
schemes: []
scope_count: 22
scope_names:
- mcp::server:connect
- mcp::audiences:read
- mcp::audiences:write
- mcp::personas.source:read
- mcp::markets:read
- mcp::inventories:read
- mcp::inventories.pricing:read
- mcp::inventories.owner_vendor:read
- mcp::pois:read
- mcp::vendors:read
- mcp::vendors.contacts:read
- mcp::plans:read
- mcp::plans:write
- mcp::rfps:read
- mcp::rfps:write
- mcp::messages:send
- mcp::customers:read
- mcp::customers:write
- mcp::read:pricing
- mcp::read:owner_vendors
- mcp::read:vendor_contacts
- mcp::read:persona_source
scopes:
- description: Establish an MCP session with the server. The baseline scope; everything else gates data.
  flows: []
  scope: mcp::server:connect
- description: Read behavioral OOH audience personas and audience segments.
  flows: []
  scope: mcp::audiences:read
- description: Create or update audience segments.
  flows: []
  scope: mcp::audiences:write
- description: Read the underlying source/provenance detail behind a persona.
  flows: []
  scope: mcp::personas.source:read
- description: Read audience-based market rankings and market recommendations.
  flows: []
  scope: mcp::markets:read
- description: Search and read OOH inventory listings (placements/units).
  flows: []
  scope: mcp::inventories:read
- description: Read pricing and availability for inventory. Separately scoped from inventories:read — this is the permission-based pricing intelligence the provider reserves for the Planner closed beta.
  flows: []
  scope: mcp::inventories.pricing:read
- description: Read the media owner / vendor that owns a given inventory unit.
  flows: []
  scope: mcp::inventories.owner_vendor:read
- description: Read points of interest used for geospatial and audience-density overlays.
  flows: []
  scope: mcp::pois:read
- description: Read media owner / vendor records.
  flows: []
  scope: mcp::vendors:read
- description: Read vendor contact records (reps). Separately scoped — contact data is PII.
  flows: []
  scope: mcp::vendors.contacts:read
- description: Read media plans / campaigns.
  flows: []
  scope: mcp::plans:read
- description: Create or modify a media plan / campaign.
  flows: []
  scope: mcp::plans:write
- description: Read requests for proposal.
  flows: []
  scope: mcp::rfps:read
- description: Draft or update a request for proposal against shortlisted inventory.
  flows: []
  scope: mcp::rfps:write
- description: Send a message into the marketplace workflow (e.g. RFP or quote outreach to a vendor).
  flows: []
  scope: mcp::messages:send
- description: Read customer / tenant records.
  flows: []
  scope: mcp::customers:read
- description: Create or update customer / tenant records.
  flows: []
  scope: mcp::customers:write
- description: Legacy form of mcp::inventories.pricing:read.
  flows: []
  scope: mcp::read:pricing
- description: Legacy form of mcp::inventories.owner_vendor:read.
  flows: []
  scope: mcp::read:owner_vendors
- description: Legacy form of mcp::vendors.contacts:read.
  flows: []
  scope: mcp::read:vendor_contacts
- description: Legacy form of mcp::personas.source:read.
  flows: []
  scope: mcp::read:persona_source
slug: onescreen-ai-scopes
source_filename: onescreen-ai-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.onescreen.ai/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.onescreen.ai/.well-known/oauth-authorization-server\ndocs: https://www.onescreen.ai/mcp/\nnote: >-\n  Not derived from an OpenAPI — OneScreen publishes no REST contract. These scopes are read\n  verbatim from the two anonymous OAuth discovery documents the MCP host serves: the RFC 8414\n  authorization-server metadata (22 scopes) and the RFC 9728 protected-resource metadata for\n  https://mcp.onescreen.ai/mcp (18 scopes). Descriptions are ours, inferred from the scope\n  name and the provider's published product description; the scope STRINGS are the provider's.\nauthorization_server: https://auth.onescreen.ai/oauth/2.1\nresource: https://mcp.onescreen.ai/mcp\nscope_count: 22\nresource_scope_count: 18\nnaming:\n  pattern: 'mcp::<resource>[.<sub-resource>]:<action>'\n  actions:\n  - read\n  - write\n  - send\n  - connect\n  note: >-\n    Two generations of naming coexist in the authorization-server metadata. The current\
  \ form\n    puts the action last (mcp::inventories.pricing:read); four legacy scopes put it first\n    (mcp::read:pricing). The legacy four are absent from the protected-resource metadata,\n    which is the narrower and more current of the two documents.\nscopes:\n- scope: mcp::server:connect\n  description: Establish an MCP session with the server. The baseline scope; everything else gates data.\n  in_resource_metadata: true\n- scope: mcp::audiences:read\n  description: Read behavioral OOH audience personas and audience segments.\n  in_resource_metadata: true\n- scope: mcp::audiences:write\n  description: Create or update audience segments.\n  in_resource_metadata: true\n- scope: mcp::personas.source:read\n  description: Read the underlying source/provenance detail behind a persona.\n  in_resource_metadata: true\n- scope: mcp::markets:read\n  description: Read audience-based market rankings and market recommendations.\n  in_resource_metadata: true\n- scope: mcp::inventories:read\n  description:\
  \ Search and read OOH inventory listings (placements/units).\n  in_resource_metadata: true\n- scope: mcp::inventories.pricing:read\n  description: >-\n    Read pricing and availability for inventory. Separately scoped from inventories:read —\n    this is the permission-based pricing intelligence the provider reserves for the Planner\n    closed beta.\n  in_resource_metadata: true\n- scope: mcp::inventories.owner_vendor:read\n  description: Read the media owner / vendor that owns a given inventory unit.\n  in_resource_metadata: true\n- scope: mcp::pois:read\n  description: Read points of interest used for geospatial and audience-density overlays.\n  in_resource_metadata: true\n- scope: mcp::vendors:read\n  description: Read media owner / vendor records.\n  in_resource_metadata: true\n- scope: mcp::vendors.contacts:read\n  description: Read vendor contact records (reps). Separately scoped — contact data is PII.\n  in_resource_metadata: true\n- scope: mcp::plans:read\n  description: Read\
  \ media plans / campaigns.\n  in_resource_metadata: true\n- scope: mcp::plans:write\n  description: Create or modify a media plan / campaign.\n  in_resource_metadata: true\n- scope: mcp::rfps:read\n  description: Read requests for proposal.\n  in_resource_metadata: true\n- scope: mcp::rfps:write\n  description: Draft or update a request for proposal against shortlisted inventory.\n  in_resource_metadata: true\n- scope: mcp::messages:send\n  description: Send a message into the marketplace workflow (e.g. RFP or quote outreach to a vendor).\n  in_resource_metadata: true\n- scope: mcp::customers:read\n  description: Read customer / tenant records.\n  in_resource_metadata: true\n- scope: mcp::customers:write\n  description: Create or update customer / tenant records.\n  in_resource_metadata: true\n- scope: mcp::read:pricing\n  description: Legacy form of mcp::inventories.pricing:read.\n  in_resource_metadata: false\n  status: legacy\n- scope: mcp::read:owner_vendors\n  description: Legacy\
  \ form of mcp::inventories.owner_vendor:read.\n  in_resource_metadata: false\n  status: legacy\n- scope: mcp::read:vendor_contacts\n  description: Legacy form of mcp::vendors.contacts:read.\n  in_resource_metadata: false\n  status: legacy\n- scope: mcp::read:persona_source\n  description: Legacy form of mcp::personas.source:read.\n  in_resource_metadata: false\n  status: legacy\nsources:\n- https://mcp.onescreen.ai/.well-known/oauth-authorization-server\n- https://mcp.onescreen.ai/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onescreen-ai/refs/heads/main/scopes/onescreen-ai-scopes.yml
summary_line: 22 scopes
tags:
- Company
- Advertising
- Out-of-Home
- DOOH
- Advertising Technology
- Marketing
- Media
- AI Agents
- MCP
- Authentication
- Agent Readiness
token_urls: []
---
