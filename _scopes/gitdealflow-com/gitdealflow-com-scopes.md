---
api_specs:
- filename: gitdealflow-com-agents-api-openapi.yml
  format: yaml
  label: GitDealFlow Agents API
  slug: gitdealflow-com-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-agents-api-openapi.yml
- filename: gitdealflow-com-answer-api-openapi.yml
  format: yaml
  label: GitDealFlow Answer API
  slug: gitdealflow-com-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-answer-api-openapi.yml
- filename: gitdealflow-com-badges-api-openapi.yml
  format: yaml
  label: GitDealFlow Badges API
  slug: gitdealflow-com-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-badges-api-openapi.yml
- filename: gitdealflow-com-brand-api-openapi.yml
  format: yaml
  label: GitDealFlow Brand API
  slug: gitdealflow-com-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-brand-api-openapi.yml
- filename: gitdealflow-com-business-model-api-openapi.yml
  format: yaml
  label: GitDealFlow Business Model API
  slug: gitdealflow-com-business-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-business-model-api-openapi.yml
- filename: gitdealflow-com-citation-api-openapi.yml
  format: yaml
  label: GitDealFlow Citation API
  slug: gitdealflow-com-citation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-citation-api-openapi.yml
- filename: gitdealflow-com-community-api-openapi.yml
  format: yaml
  label: GitDealFlow Community API
  slug: gitdealflow-com-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-community-api-openapi.yml
- filename: gitdealflow-com-deep-signal-api-openapi.yml
  format: yaml
  label: GitDealFlow Deep Signal API
  slug: gitdealflow-com-deep-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-deep-signal-api-openapi.yml
- filename: gitdealflow-com-glossary-api-openapi.yml
  format: yaml
  label: GitDealFlow Glossary API
  slug: gitdealflow-com-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-glossary-api-openapi.yml
- filename: gitdealflow-com-markets-api-openapi.yml
  format: yaml
  label: GitDealFlow Markets API
  slug: gitdealflow-com-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-markets-api-openapi.yml
- filename: gitdealflow-com-meta-api-openapi.yml
  format: yaml
  label: GitDealFlow Meta API
  slug: gitdealflow-com-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-meta-api-openapi.yml
- filename: gitdealflow-com-methodology-api-openapi.yml
  format: yaml
  label: GitDealFlow Methodology API
  slug: gitdealflow-com-methodology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-methodology-api-openapi.yml
- filename: gitdealflow-com-scout-api-openapi.yml
  format: yaml
  label: GitDealFlow Scout API
  slug: gitdealflow-com-scout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-scout-api-openapi.yml
- filename: gitdealflow-com-search-api-openapi.yml
  format: yaml
  label: GitDealFlow Search API
  slug: gitdealflow-com-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-search-api-openapi.yml
- filename: gitdealflow-com-signals-api-openapi.yml
  format: yaml
  label: GitDealFlow Signals API
  slug: gitdealflow-com-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/openapi/gitdealflow-com-signals-api-openapi.yml
authorization_urls: []
description: ''
docs: https://signals.gitdealflow.com/agents.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gitdealflow Com Scopes
name_suffix: OAuth Scopes
note: 'The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py found nothing to derive), but the MCP host publishes OAuth 2.0 authorization-server metadata with a single scope. The token endpoint issues a Bearer JWT to anonymous callers (token_endpoint_auth_methods_supported [none]) — it is an optional, identity-less capability token for the MCP server, "required: false" per mcp.json. The paid REST route uses a separate credit-pack bearer key, not OAuth.'
overview: 'GitDealFlow publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the GitDealFlow API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GitDealFlow
provider_slug: gitdealflow-com
schemes: []
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read access to the MCP server tools/resources/prompts (all free tools are readable without it; the scope exists so clients that insist on a token can obtain one)
  flows: []
  scope: mcp:read
slug: gitdealflow-com-scopes
source_filename: gitdealflow-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://signals.gitdealflow.com/.well-known/oauth-authorization-server (RFC 8414), https://signals.gitdealflow.com/.well-known/mcp.json endpoints.oauth, live POST https://signals.gitdealflow.com/api/oauth/token (grant_type=client_credentials, 2026-09-19)\ndocs: https://signals.gitdealflow.com/agents.md\nnote: >-\n  The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py found nothing to derive), but\n  the MCP host publishes OAuth 2.0 authorization-server metadata with a single scope. The token endpoint\n  issues a Bearer JWT to anonymous callers (token_endpoint_auth_methods_supported [none]) — it is an\n  optional, identity-less capability token for the MCP server, \"required: false\" per mcp.json. The paid\n  REST route uses a separate credit-pack bearer key, not OAuth.\nissuer: https://signals.gitdealflow.com\ntoken_endpoint: https://signals.gitdealflow.com/api/oauth/token\nauthorization_endpoint: null\ngrant_types:\
  \ [client_credentials]\ntoken_endpoint_auth_methods: [none]\nresponse_types: []\ntoken:\n  type: Bearer (JWT, HS256 per header)\n  expires_in: 3600\n  observed: 200 with access_token, token_type Bearer, expires_in 3600, scope mcp:read\nscopes:\n- scope: mcp:read\n  description: Read access to the MCP server tools/resources/prompts (all free tools are readable without it; the scope exists so clients that insist on a token can obtain one)\n  required: false\n  applies_to: https://signals.gitdealflow.com/api/mcp/rpc\nscope_count: 1\nprotected_resource_metadata: absent (/.well-known/oauth-protected-resource 404 on the MCP host)\ndynamic_client_registration: absent (no registration_endpoint in metadata)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitdealflow-com/refs/heads/main/scopes/gitdealflow-com-scopes.yml
summary_line: 1 scope
tags:
- Venture Capital
- Deal Flow
- Startups
- GitHub
- Alternative Data
- Investing
- MCP
- Agents
- Developer Tools
- A2A
token_urls: []
---
