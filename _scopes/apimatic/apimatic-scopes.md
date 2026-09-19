---
api_specs:
- filename: apimatic-portals-api-openapi.yml
  format: yaml
  label: APIMatic Portals API
  slug: apimatic-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-portals-api-openapi.yml
- filename: apimatic-sdk-generation-api-openapi.yml
  format: yaml
  label: APIMatic SDK Generation API
  slug: apimatic-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-sdk-generation-api-openapi.yml
- filename: apimatic-transformation-api-openapi.yml
  format: yaml
  label: APIMatic Transformation API
  slug: apimatic-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-transformation-api-openapi.yml
- filename: apimatic-validation-api-openapi.yml
  format: yaml
  label: APIMatic Validation API
  slug: apimatic-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-validation-api-openapi.yml
- filename: apimatic-apis-api-openapi.yml
  format: yaml
  label: APIMatic AP Is API
  slug: apimatic-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-apis-api-openapi.yml
authorization_urls:
- https://chatbotapi.apimatic.io/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Apimatic Scopes
name_suffix: OAuth Scopes
note: APIMatic's PLATFORM API has no OAuth surface — it authenticates with a custom Authorization header carrying an Auth Key (see authentication/apimatic-authentication.yml). The only OAuth scope APIMatic publishes belongs to its hosted MCP server, whose RFC 8414 and RFC 9728 discovery documents were fetched live on 2026-09-15. Recorded here because a scope an agent can actually request is a scope, whichever surface serves it; it is NOT evidence of OAuth on the Platform API.
overview: 'APIMatic publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the APIMatic API on a user''s behalf.


  Tokens are issued from https://chatbotapi.apimatic.io/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: APIMatic
provider_slug: apimatic
schemes:
- code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://chatbotapi.apimatic.io/authorize
    flow: authorizationCode
    tokenUrl: https://chatbotapi.apimatic.io/token
  - flow: clientCredentials
    tokenUrl: https://chatbotapi.apimatic.io/token
  issuer: https://chatbotapi.apimatic.io
  name: chatbotapi-mcp-oauth
  registration_endpoint: https://chatbotapi.apimatic.io/register
  resource: https://chatbotapi.apimatic.io
  source: https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - none
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Call the tools exposed by the APIMatic Integration Agent MCP server (ask, update_activity, model_search, endpoint_search). The only scope the authorization server advertises.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:tools
slug: apimatic-scopes
source_filename: apimatic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: probed\nsource: https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server\ndocs: null\nnote: >-\n  APIMatic's PLATFORM API has no OAuth surface — it authenticates with a custom Authorization\n  header carrying an Auth Key (see authentication/apimatic-authentication.yml). The only OAuth\n  scope APIMatic publishes belongs to its hosted MCP server, whose RFC 8414 and RFC 9728\n  discovery documents were fetched live on 2026-09-15. Recorded here because a scope an agent\n  can actually request is a scope, whichever surface serves it; it is NOT evidence of OAuth on\n  the Platform API.\napplies_to: mcp\nschemes:\n  - name: chatbotapi-mcp-oauth\n    source: https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server\n    issuer: https://chatbotapi.apimatic.io\n    resource: https://chatbotapi.apimatic.io\n    token_endpoint_auth_methods_supported: [none]\n    code_challenge_methods_supported: [S256]\n    registration_endpoint:\
  \ https://chatbotapi.apimatic.io/register\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://chatbotapi.apimatic.io/authorize\n        tokenUrl: https://chatbotapi.apimatic.io/token\n      - flow: clientCredentials\n        tokenUrl: https://chatbotapi.apimatic.io/token\nscopes:\n  - scope: mcp:tools\n    description: >-\n      Call the tools exposed by the APIMatic Integration Agent MCP server (ask, update_activity,\n      model_search, endpoint_search). The only scope the authorization server advertises.\n    flows: [authorizationCode, clientCredentials]\n    sources: [https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server]\nx-evidence:\n  fetched: '2026-09-15'\n  http_status: 200\n  note: >-\n    The MCP endpoint also answered an anonymous initialize and tools/list with HTTP 200, so this\n    OAuth surface is offered rather than enforced.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/scopes/apimatic-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- API Transformation
- Code Generation
- Developer Experience
- Developer Tools
- Documentation
- SDK Generation
token_urls:
- https://chatbotapi.apimatic.io/token
---
