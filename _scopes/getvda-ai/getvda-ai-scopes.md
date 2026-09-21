---
api_specs:
- filename: getvda-ai-witness-openapi.json
  format: json
  label: VDA Witness API
  slug: vda-witness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-witness-openapi.json
- filename: getvda-ai-hitl-openapi.json
  format: json
  label: VDA HITL API
  slug: vda-hitl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-hitl-openapi.json
- filename: getvda-ai-acp-openapi.json
  format: json
  label: VDA ACP API
  slug: vda-acp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-acp-openapi.json
- filename: getvda-ai-c2md-edge-openapi.json
  format: json
  label: C2MD Compliance Agent
  slug: c2md-compliance-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-c2md-edge-openapi.json
- filename: getvda-ai-gosce-router-openapi.json
  format: json
  label: GOSCE Agent Portfolio and Router
  slug: gosce-agent-portfolio-and-router
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/openapi/getvda-ai-gosce-router-openapi.json
authorization_urls: []
description: ''
docs: https://c2md.getvda.ai/llms.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Getvda Ai Scopes
name_suffix: OAuth Scopes
note: 'The OAuth scopes live in the served C2MD agent card''s securitySchemes, not in any OpenAPI (the C2MD OpenAPI is an edge-proxy shell with no securitySchemes, so derive-oauth-scopes.py has nothing to read). The same five c2md:* scopes are declared identically under google_oauth2 and microsoft_oauth2 authorizationCode flows, plus one Microsoft clientCredentials scope for pre-registered service principals. The witness_bearer scheme maps a Witness ACCOUNT tier to the same access ladder without OAuth: SEALED -> assess-tier skills, ANCHORED -> generate_starter and above. Witness''s own whoami returns scopes ["seal","read"] for a key; those are account-level grants, not OAuth scopes, and are listed under witness_account_scopes.'
overview: 'Verified Digital Agents (VDA) uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Verified Digital Agents (VDA)
provider_slug: getvda-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: getvda-ai-scopes
source_filename: getvda-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://c2md.getvda.ai/.well-known/agent-card.json\ndocs: https://c2md.getvda.ai/llms.txt\nderived_from: a2a/getvda-ai-c2md-agent-card.json\nnote: >-\n  The OAuth scopes live in the served C2MD agent card's securitySchemes, not in any OpenAPI (the C2MD OpenAPI is\n  an edge-proxy shell with no securitySchemes, so derive-oauth-scopes.py has nothing to read). The same five\n  c2md:* scopes are declared identically under google_oauth2 and microsoft_oauth2 authorizationCode flows, plus\n  one Microsoft clientCredentials scope for pre-registered service principals. The witness_bearer scheme maps a\n  Witness ACCOUNT tier to the same access ladder without OAuth: SEALED -> assess-tier skills, ANCHORED ->\n  generate_starter and above. Witness's own whoami returns scopes [\"seal\",\"read\"] for a key; those are\n  account-level grants, not OAuth scopes, and are listed under witness_account_scopes.\nauthorization_servers:\n- name: Google\n\
  \  authorization_url: https://accounts.google.com/o/oauth2/v2/auth\n  token_url: https://oauth2.googleapis.com/token\n  flows: [authorizationCode]\n  audience: Workspace and personal Google accounts; token validated via Google's JWKS\n- name: Microsoft Entra ID (organizations)\n  authorization_url: https://login.microsoftonline.com/organizations/oauth2/v2.0/authorize\n  token_url: https://login.microsoftonline.com/organizations/oauth2/v2.0/token\n  flows: [authorizationCode, clientCredentials]\n  audience: work and school accounts only; personal Microsoft accounts not supported\nscopes:\n- name: c2md:assess\n  description: Risk assessment and framework translation. Free tier. Rate-limited per account.\n  tier: free\n  skills: [assess_agent_risk, translate_control, list_supported_frameworks, generate_evidence_readiness_report, extract_governance_inputs]\n- name: c2md:generate_starter\n  description: Single-jurisdiction, single-framework-stack bundle. Watermarked. Non-commercial licence.\n\
  \  tier: starter\n  skills: [generate_compliance_bundle]\n- name: c2md:generate_pro\n  description: Multi-jurisdiction, full-framework-stack bundle. Includes DPIA / FRIA scaffolding. Commercial deployment licence.\n  tier: pro\n  skills: [generate_compliance_bundle, generate_dpia_fria_scaffold]\n- name: c2md:generate_journey\n  description: Full VDA-MD two-axis library for a given industry. Journey tier subscription.\n  tier: journey\n  skills: [generate_journey_baseline]\n  note: The backing skill is PLANNED and returns -32601 today.\n- name: c2md:commercial_deploy\n  description: Commercial deployment rights for any bundle previously generated on this account.\n  tier: pro\n  skills: []\n- name: 7c89fa90-05ca-4779-8128-32c7f11f604b/.default\n  description: 'TIER 3 (by arrangement — enterprise/platform integrations, NOT self-serve): service-principal callers pre-registered to a C2MD platform-of-record account; tier and contract terms resolved server-side. Unregistered principals resolve\
  \ to free-tier (assess only). Contact hello@getvda.ai.'\n  tier: enterprise\n  flow: clientCredentials (Microsoft only)\nwitness_account_scopes:\n- name: seal\n  description: Returned by GET /api/witness/whoami for a valid key; grants sealing on the account's chains.\n- name: read\n  description: Returned by whoami; grants list_records / get_record / report on the account's own records.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getvda-ai/refs/heads/main/scopes/getvda-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- AI Agents
- AI Governance
- Compliance
- Audit Trail
- Agent Identity
- A2A
- MCP
- x402
- EU AI Act
- Human-in-the-Loop
token_urls: []
---
