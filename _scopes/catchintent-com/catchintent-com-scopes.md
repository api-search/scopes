---
api_specs:
- filename: catchintent-com-discovery-api-openapi.yml
  format: yaml
  label: CatchIntent Discovery API
  slug: catchintent-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-discovery-api-openapi.yml
- filename: catchintent-com-health-api-openapi.yml
  format: yaml
  label: CatchIntent Health API
  slug: catchintent-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-health-api-openapi.yml
- filename: catchintent-com-mcp-api-openapi.yml
  format: yaml
  label: CatchIntent MCP API
  slug: catchintent-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-mcp-api-openapi.yml
- filename: catchintent-com-oauth-api-openapi.yml
  format: yaml
  label: CatchIntent OAuth API
  slug: catchintent-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-oauth-api-openapi.yml
authorization_urls:
- https://engine.catchintent.com/mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Catchintent Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CatchIntent publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CatchIntent API on a user''s behalf.


  Tokens are issued from https://engine.catchintent.com/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CatchIntent
provider_slug: catchintent-com
schemes:
- description: OAuth 2.1 with PKCE. Discover endpoints from https://engine.catchintent.com/.well-known/oauth-authorization-server. Request only the scopes needed for the MCP tools being called.
  flows:
  - authorizationUrl: https://engine.catchintent.com/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://engine.catchintent.com/mcp/token
  name: mcpOAuth
  source: openapi/catchintent-com-openapi.json
scope_count: 9
scope_names:
- read:agents
- read:leads
- read:outreach
- read:workspace
- write:agents
- write:crm
- write:leads
- write:outreach
- write:workspace
scopes:
- description: Read agents via agent_list, agent_get, agent_runs.
  flows:
  - authorizationCode
  scope: read:agents
- description: Read leads via lead_search, lead_get.
  flows:
  - authorizationCode
  scope: read:leads
- description: Read outreach engagements and unified inbox via engagement_list, engagement_get, inbox_list.
  flows:
  - authorizationCode
  scope: read:outreach
- description: Read workspace usage, ICP options, and product/brand context.
  flows:
  - authorizationCode
  scope: read:workspace
- description: Create, update, and change status of agents via agent_create, agent_update, agent_set_status.
  flows:
  - authorizationCode
  scope: write:agents
- description: Push qualified leads to connected CRMs via lead_push_to_crm.
  flows:
  - authorizationCode
  scope: write:crm
- description: Update lead status, trigger enrichment, and draft outreach via lead_update_status, lead_enrich, lead_draft_outreach.
  flows:
  - authorizationCode
  scope: write:leads
- description: Manage engagement lifecycle via engagement_enroll, engagement_reassign, engagement_pause, engagement_resume, engagement_mark_replied, engagement_exit.
  flows:
  - authorizationCode
  scope: write:outreach
- description: Create, update, and delete products (brands).
  flows:
  - authorizationCode
  scope: write:workspace
slug: catchintent-com-scopes
source_filename: catchintent-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/catchintent-com-openapi.json\nschemes:\n- name: mcpOAuth\n  source: openapi/catchintent-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://engine.catchintent.com/mcp/authorize\n    tokenUrl: https://engine.catchintent.com/mcp/token\n  description: OAuth 2.1 with PKCE. Discover endpoints from https://engine.catchintent.com/.well-known/oauth-authorization-server.\n    Request only the scopes needed for the MCP tools being called.\nscopes:\n- scope: read:agents\n  description: Read agents via agent_list, agent_get, agent_runs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: read:leads\n  description: Read leads via lead_search, lead_get.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: read:outreach\n  description: Read outreach engagements and unified inbox via engagement_list, engagement_get,\n\
  \    inbox_list.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: read:workspace\n  description: Read workspace usage, ICP options, and product/brand context.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: write:agents\n  description: Create, update, and change status of agents via agent_create, agent_update, agent_set_status.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: write:crm\n  description: Push qualified leads to connected CRMs via lead_push_to_crm.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: write:leads\n  description: Update lead status, trigger enrichment, and draft outreach via lead_update_status,\n    lead_enrich, lead_draft_outreach.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: write:outreach\n  description: Manage engagement\
  \ lifecycle via engagement_enroll, engagement_reassign, engagement_pause,\n    engagement_resume, engagement_mark_replied, engagement_exit.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n- scope: write:workspace\n  description: Create, update, and delete products (brands).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/catchintent-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/catchintent-com/scopes/catchintent-com-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- B2B
- Sales
- Intent Data
- Artificial Intelligence
- Outbound
token_bound: false
token_urls:
- https://engine.catchintent.com/mcp/token
---
