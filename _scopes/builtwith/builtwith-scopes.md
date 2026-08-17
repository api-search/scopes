---
api_specs:
- filename: builtwith-live-feed-asyncapi.yml
  format: yaml
  label: BuiltWith Live Feed API
  slug: builtwith-live-feed-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/asyncapi/builtwith-live-feed-asyncapi.yml
- filename: builtwith-agent-stripe-topup-openapi.json
  format: json
  label: BuiltWith Agent Payment API
  slug: builtwith-agent-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-agent-stripe-topup-openapi.json
- filename: builtwith-rest-api-openapi.json
  format: json
  label: BuiltWith REST API
  slug: builtwith-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-rest-api-openapi.json
- filename: builtwith-x402-pay-per-call-openapi.json
  format: json
  label: BuiltWith x402 Pay-per-Call API
  slug: builtwith-x402-pay-per-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-x402-pay-per-call-openapi.json
- filename: builtwith-bulk-processing-api-openapi.yml
  format: yaml
  label: BuiltWith Bulk Processing API
  slug: builtwith-bulk-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-bulk-processing-api-openapi.yml
- filename: builtwith-domain-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Domain Lookup API
  slug: builtwith-domain-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-lookup-api-openapi.yml
- filename: builtwith-domain-relationships-api-openapi.yml
  format: yaml
  label: BuiltWith Domain Relationships API
  slug: builtwith-domain-relationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-domain-relationships-api-openapi.yml
- filename: builtwith-free-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Free Lookup API
  slug: builtwith-free-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-free-lookup-api-openapi.yml
- filename: builtwith-tag-lookup-api-openapi.yml
  format: yaml
  label: BuiltWith Tag Lookup API
  slug: builtwith-tag-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-tag-lookup-api-openapi.yml
- filename: builtwith-technology-changes-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Changes API
  slug: builtwith-technology-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-changes-api-openapi.yml
- filename: builtwith-technology-lists-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Lists API
  slug: builtwith-technology-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-lists-api-openapi.yml
- filename: builtwith-technology-trends-api-openapi.yml
  format: yaml
  label: BuiltWith Technology Trends API
  slug: builtwith-technology-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/openapi/builtwith-technology-trends-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Builtwith Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securityScheme in any OpenAPI (BuiltWith's specs declare apiKey and bearer only). The OAuth surface is not in the specs - it is published as RFC 8414 / RFC 9728 discovery documents at the well-known paths below, which is how an MCP client negotiates access to https://api.builtwith.com/mcp. Scopes are recorded from those probed documents, not derived or invented.
overview: 'BuiltWith publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the BuiltWith API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BuiltWith
provider_slug: builtwith
schemes: []
scope_count: 2
scope_names:
- api.read
- api.write
scopes:
- description: Read access to the BuiltWith API resource. Not further described by the provider; every intelligence endpoint (domain, lists, trends, relationships, change, trust, keywords, product, vector, ask) is a read.
  flows:
  - authorizationCode
  scope: api.read
- description: Write access to the BuiltWith API resource. Not further described by the provider; the only mutating published operations are account credit purchases and x402 credit/List-pass purchases.
  flows:
  - authorizationCode
  scope: api.write
slug: builtwith-scopes
source_filename: builtwith-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.builtwith.com/.well-known/oauth-protected-resource\ndocs: null\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme in any OpenAPI (BuiltWith's specs\n  declare apiKey and bearer only). The OAuth surface is not in the specs - it is published as\n  RFC 8414 / RFC 9728 discovery documents at the well-known paths below, which is how an MCP\n  client negotiates access to https://api.builtwith.com/mcp. Scopes are recorded from those\n  probed documents, not derived or invented.\nprotected_resource:\n  spec: RFC 9728\n  url: https://api.builtwith.com/.well-known/oauth-protected-resource\n  http_status: 200\n  resource: https://api.builtwith.com/\n  resource_name: BuiltWith API\n  authorization_servers:\n  - https://api.builtwith.com/\n  bearer_methods_supported: [header]\nauthorization_server:\n  spec: RFC 8414\n  url: https://api.builtwith.com/.well-known/oauth-authorization-server\n  http_status: 200\n \
  \ issuer: https://api.builtwith.com\n  authorization_endpoint: https://api.builtwith.com/authorize\n  token_endpoint: https://api.builtwith.com/token\n  registration_endpoint: https://api.builtwith.com/oauth/register\n  response_types_supported: [code]\n  grant_types_supported: [authorization_code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  dynamic_client_registration: true\n  pkce_required: true\nscopes:\n- scope: api.read\n  description: >-\n    Read access to the BuiltWith API resource. Not further described by the provider; every\n    intelligence endpoint (domain, lists, trends, relationships, change, trust, keywords,\n    product, vector, ask) is a read.\n  flows: [authorizationCode]\n  sources: [.well-known/oauth-protected-resource]\n- scope: api.write\n  description: >-\n    Write access to the BuiltWith API resource. Not further described by the provider; the only\n    mutating published operations are account credit purchases\
  \ and x402 credit/List-pass\n    purchases.\n  flows: [authorizationCode]\n  sources: [.well-known/oauth-protected-resource]\ngaps:\n- No scopes reference page is published on the docs site; the two scope strings above are the\n  complete published set and carry no provider-authored descriptions.\n- The authorization server advertises token_endpoint_auth_methods_supported=[none] with PKCE\n  S256 and open dynamic client registration, which is the standard MCP public-client shape.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/builtwith/refs/heads/main/scopes/builtwith-scopes.yml
summary_line: 2 scopes
tags:
- Technology Profiling
- Lead Generation
- Web Intelligence
- Technology Detection
- Website Analysis
- Market Research
- Technographics
- Sales Intelligence
- AI Agents
- Model Context Protocol
- Agentic Commerce
- Real-time Data
token_urls: []
---
