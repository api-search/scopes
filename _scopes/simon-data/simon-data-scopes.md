---
api_specs:
- filename: simon-data-audience-api-openapi.yml
  format: yaml
  label: Simon Data Audience API
  slug: simon-data-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-audience-api-openapi.yml
- filename: simon-data-event-ingestion-openapi.yml
  format: yaml
  label: Simon Data Event Ingestion API
  slug: simon-data-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/openapi/simon-data-event-ingestion-openapi.yml
authorization_urls:
- https://app.simondata.com/mcp/oauth/authorize
description: ''
docs: https://docs.simondata.com/reference/getting-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Simon Data Scopes
name_suffix: OAuth Scopes
note: Simon Data publishes no OAuth scope vocabulary. The Audience API uses opaque bearer tokens issued by a Client Solutions Manager, and the Event Ingestion API uses a shared partnerSecret in the payload — neither has a scope surface. The one OAuth authorization server Simon does publish, the MCP metadata document at https://app.simondata.com/.well-known/oauth-authorization-server, omits scopes_supported entirely. Recorded as a real zero, not a gap.
overview: 'Simon Data uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app.simondata.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Simon Data
provider_slug: simon-data
schemes:
- description: MCP authorization server; scopes_supported is absent from the published metadata.
  flows:
  - authorizationUrl: https://app.simondata.com/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.simondata.com/mcp/oauth/token
  name: mcp-oauth
  source: well-known/simon-data-oauth-authorization-server.json
scope_count: 0
scope_names: []
scopes: []
slug: simon-data-scopes
source_filename: simon-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.simondata.com/reference/getting-started\ndocs: https://docs.simondata.com/reference/getting-started\nnote: >-\n  Simon Data publishes no OAuth scope vocabulary. The Audience API uses opaque bearer tokens issued by a Client\n  Solutions Manager, and the Event Ingestion API uses a shared partnerSecret in the payload — neither has a scope\n  surface. The one OAuth authorization server Simon does publish, the MCP metadata document at\n  https://app.simondata.com/.well-known/oauth-authorization-server, omits scopes_supported entirely. Recorded as a real\n  zero, not a gap.\nschemes:\n- name: mcp-oauth\n  source: well-known/simon-data-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.simondata.com/mcp/oauth/authorize\n    tokenUrl: https://app.simondata.com/mcp/oauth/token\n  description: MCP authorization server; scopes_supported is absent from the published metadata.\n\
  scopes: []\nscope_count: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simon-data/refs/heads/main/scopes/simon-data-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Customer Data Platform
- CDP
- Marketing Automation
- Audience Segmentation
- Event Tracking
- Data Ingestion
- Personalization
- Marketing Technology
- Identity Resolution
- Customer Profiles
- Journey Orchestration
- Snowflake
token_urls:
- https://app.simondata.com/mcp/oauth/token
---
