---
api_specs:
- filename: turquoise-health-consumer-pricing-api-openapi.yml
  format: yaml
  label: Turquoise Health Consumer Pricing API
  slug: turquoise-health-consumer-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/openapi/turquoise-health-consumer-pricing-api-openapi.yml
authorization_urls: []
description: ''
docs: https://turquoise.health/api/docs/mcp-reference/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Turquoise Health Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securityScheme in the OpenAPI (the spec declares only http/bearer schemes and no flow scopes), so there is no derived baseline to build on. Every scope below comes from the provider's own published documentation — the llms.txt MCP block and the MCP reference — not from the spec. Turquoise does not publish a dedicated scopes/permissions reference page; these are the only two scopes named anywhere in the public docs, so this list is documented-complete rather than registry-complete.
overview: 'Turquoise Health publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Turquoise Health API on a user''s behalf.


  Tokens are issued from https://api.turquoise.health/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Turquoise Health
provider_slug: turquoise-health
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.turquoise.health/oauth/token
  name: OAuth2 client credentials
  source: https://turquoise.health/api/docs/start-building.md
scope_count: 2
scope_names:
- read:mcp
- read:eligibility
scopes:
- description: Required on every token used against the MCP endpoint (https://consumer-mcp.turquoise.health/mcp). A token without it is rejected with HTTP 403 ("Token is valid but not granted correct scope").
  flows:
  - clientCredentials
  scope: read:mcp
- description: Additionally required by the estimate_out_of_pocket MCP tool and, by extension, the consented 270/271 member eligibility check behind POST /v3/personalized-estimates. For real patient data this scope also requires production access under a signed Business Associate Agreement.
  flows:
  - clientCredentials
  scope: read:eligibility
slug: turquoise-health-scopes
source_filename: turquoise-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://turquoise.health/api/docs/llms.txt\ndocs: https://turquoise.health/api/docs/mcp-reference/\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme in the OpenAPI (the spec declares\n  only http/bearer schemes and no flow scopes), so there is no derived baseline to build\n  on. Every scope below comes from the provider's own published documentation — the\n  llms.txt MCP block and the MCP reference — not from the spec. Turquoise does not publish\n  a dedicated scopes/permissions reference page; these are the only two scopes named\n  anywhere in the public docs, so this list is documented-complete rather than\n  registry-complete.\n\nschemes:\n- name: OAuth2 client credentials\n  source: https://turquoise.health/api/docs/start-building.md\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.turquoise.health/oauth/token\n\nscopes:\n- scope: read:mcp\n  description: >-\n    Required on every token\
  \ used against the MCP endpoint\n    (https://consumer-mcp.turquoise.health/mcp). A token without it is rejected with HTTP\n    403 (\"Token is valid but not granted correct scope\").\n  flows: [clientCredentials]\n  surfaces: [mcp]\n  sources: [https://turquoise.health/api/docs/llms.txt, https://turquoise.health/api/docs/mcp-reference.md]\n- scope: read:eligibility\n  description: >-\n    Additionally required by the estimate_out_of_pocket MCP tool and, by extension, the\n    consented 270/271 member eligibility check behind POST /v3/personalized-estimates. For\n    real patient data this scope also requires production access under a signed Business\n    Associate Agreement.\n  flows: [clientCredentials]\n  surfaces: [mcp, rest]\n  requires_baa: true\n  sources: [https://turquoise.health/api/docs/llms.txt]\n\nmetadata_discovery:\n  authorization_server: https://consumer-mcp.turquoise.health/.well-known/oauth-authorization-server\n  protected_resource: https://consumer-mcp.turquoise.health/.well-known/oauth-protected-resource/mcp\n\
  \  metadata_note: >-\n    The RFC 8414 document advertises scopes_supported [openid, profile, email] and\n    grant_types_supported [authorization_code, refresh_token] — that is the INTERACTIVE\n    browser sign-in path for MCP clients, a different grant from the server-to-server\n    client-credentials flow the docs describe. The RFC 9728 protected-resource document\n    returns an EMPTY scopes_supported array, so neither metadata document advertises\n    read:mcp or read:eligibility. That is a real discovery gap: the scopes an integrator\n    must request are documented in prose only.\n\ninsufficient_scope_error:\n  http: 403\n  code: insufficient_scope\n  message: Token is valid but not granted correct scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/scopes/turquoise-health-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Healthcare
- Price Transparency
- Hospital Rates
- Payer Rates
- Machine-Readable Files
- FHIR
- Health Insurance
- Negotiated Rates
- Out-of-Pocket Costs
- MRF
- Consumer Pricing
- MCP
- Eligibility
- Standard Service Packages
- HIPAA
token_urls:
- https://api.turquoise.health/oauth/token
---
