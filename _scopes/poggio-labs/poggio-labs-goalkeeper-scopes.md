---
api_specs:
- filename: poggio-labs-goalkeeper-openapi.json
  format: json
  label: Goalkeeper API
  slug: goalkeeper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/poggio-labs/refs/heads/main/openapi/poggio-labs-goalkeeper-openapi.json
authorization_urls: []
description: ''
docs: https://docs.gkeeper.ai/docs/concepts/api-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Poggio Labs Goalkeeper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Poggio Labs publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Poggio Labs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Poggio Labs
provider_slug: poggio-labs
schemes:
- description: A Goalkeeper API token or provider-issued OAuth access token.
  name: bearerAuth
  scheme: bearer
  source: openapi/poggio-labs-goalkeeper-openapi.json
  type: http
- in: cookie
  name: cookieAuth
  parameter_name: goalkeeper_session
  source: openapi/poggio-labs-goalkeeper-openapi.json
  type: apiKey
scope_count: 6
scope_names:
- goals:read
- goals:write
- goals:read:all
- goals:write:all
- labels:read
- labels:write
scopes:
- description: Read goals owned by the token owner.
  flows: []
  scope: goals:read
- description: Create goals, update metadata, and report status for goals owned by the token owner.
  flows: []
  scope: goals:write
- description: Read every goal visible to the token owner.
  flows: []
  scope: goals:read:all
- description: Create goals, update metadata, and report status for every goal writable by the token owner.
  flows: []
  scope: goals:write:all
- description: Read organization goal labels.
  flows: []
  scope: labels:read
- description: Create, update, and delete organization goal labels.
  flows: []
  scope: labels:write
slug: poggio-labs-goalkeeper-scopes
source_filename: poggio-labs-goalkeeper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.gkeeper.ai/docs/concepts/api-tokens\ndocs: https://docs.gkeeper.ai/docs/concepts/api-tokens\nspec_source: openapi/poggio-labs-goalkeeper-openapi.json#/components/schemas/ApiTokenScope\napplies_to: Goalkeeper (github.com/poggiolabs/goalkeeper) API tokens and MCP OAuth\nregistry_endpoint: GET /v1/api-token-scopes\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: A Goalkeeper API token or provider-issued OAuth access token.\n  source: openapi/poggio-labs-goalkeeper-openapi.json\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter_name: goalkeeper_session\n  source: openapi/poggio-labs-goalkeeper-openapi.json\nscope_count: 6\nscopes:\n- scope: goals:read\n  description: Read goals owned by the token owner.\n  default: true\n  note: The token creation form initially selects only this scope.\n- scope: goals:write\n  description: >-\n    Create goals, update metadata, and report status\
  \ for goals owned by the token owner.\n- scope: goals:read:all\n  description: Read every goal visible to the token owner.\n  implies: [goals:read]\n- scope: goals:write:all\n  description: >-\n    Create goals, update metadata, and report status for every goal writable by the\n    token owner.\n  implies: [goals:write]\n- scope: labels:read\n  description: Read organization goal labels.\n- scope: labels:write\n  description: Create, update, and delete organization goal labels.\nrules:\n- All-goals scopes include the corresponding own-goals capability.\n- Write scopes do NOT imply read access.\n- Every token must carry at least one scope.\n- >-\n  authorizeApiToken denies capabilities absent from the registry and revalidates the\n  token owner's current authority on every request; removing that authority blocks the\n  token without requiring token replacement.\n- >-\n  API tokens cannot call token-management operations; those require an interactive\n  browser session.\ntoken_policy:\n\
  \  storage: SHA-256 hash of a 256-bit random secret\n  secret_visibility: returned in full once at creation; later responses expose only a prefix\n  expiry_days: {min: 1, max: 365, default: 90}\n  revocation: persistent and immediate\n  last_used_write_interval: 5 minutes\n  opaque: >-\n    API tokens are intentionally not JWTs so that revocation and current-policy checks\n    stay authoritative on every request.\nmcp_oauth_scopes:\n  supported: [goals:read, goals:write, labels:read, labels:write]\n  initial: [goals:read, labels:read]\n  note: >-\n    Configured on a hosted deployment via MCP_OAUTH_SCOPES_SUPPORTED /\n    MCP_OAUTH_INITIAL_SCOPES; see mcp/poggio-labs-goalkeeper-mcp.yml.\npoggio_platform_note: >-\n  The hosted Poggio platform API (api.poggio.io/v2) publishes OAuth 2.0 authorization\n  server metadata with no scopes_supported key at all, and its MCP protected-resource\n  metadata publishes scopes_supported as an EMPTY array — Poggio's hosted surface has no\n  scope vocabulary;\
  \ organization is inferred from the access token instead. This scopes\n  artifact therefore covers Goalkeeper only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poggio-labs/refs/heads/main/scopes/poggio-labs-goalkeeper-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Ai
- Revenue Intelligence
- Sales
- Account Intelligence
- CRM
- Salesforce
- MCP
- AI Agents
- Enterprise
- Open Source
- Goals
- Gong
- Slack
token_urls: []
---
