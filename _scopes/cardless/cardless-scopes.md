---
authorization_urls:
- https://docs.cardless.com/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Cardless Scopes
name_suffix: OAuth Scopes
note: The only OAuth scope surface Cardless publishes anonymously belongs to the documentation MCP server at docs.cardless.com/mcp, not to the partner API. The partner API's own token response reports a fixed scope value of "partner" (see authentication/cardless-authentication.yml); it is not a delegated-consent scope system and Cardless publishes no scope reference page.
overview: 'Cardless publishes 1 OAuth 2.0 scope via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cardless API on a user''s behalf.


  Tokens are issued from https://docs.cardless.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cardless
provider_slug: cardless
schemes:
- code_challenge_methods:
  - S256
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://docs.cardless.com/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://docs.cardless.com/mcp/oauth/token
  - flow: clientCredentials
    tokenUrl: https://docs.cardless.com/mcp/oauth/token
  - flow: refreshToken
    tokenUrl: https://docs.cardless.com/mcp/oauth/token
  issuer: https://docs.cardless.com/mcp/oauth
  name: Cardless Docs MCP OAuth
  protected_resource: https://docs.cardless.com
  registration_endpoint: https://docs.cardless.com/mcp/oauth/register
  source: well-known/cardless-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  - client_secret_basic
scope_count: 1
scope_names:
- mcp:search
scopes:
- description: Search and read the Cardless documentation corpus through the MCP server.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:search
slug: cardless-scopes
source_filename: cardless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.cardless.com/.well-known/oauth-authorization-server\ndocs: null\nnote: 'The only OAuth scope surface Cardless publishes anonymously belongs to the\n  documentation MCP server at docs.cardless.com/mcp, not to the partner API. The\n  partner API''s own token response reports a fixed scope value of \"partner\" (see\n  authentication/cardless-authentication.yml); it is not a delegated-consent scope\n  system and Cardless publishes no scope reference page.'\nschemes:\n- name: Cardless Docs MCP OAuth\n  source: well-known/cardless-oauth-authorization-server.json\n  issuer: https://docs.cardless.com/mcp/oauth\n  protected_resource: https://docs.cardless.com\n  registration_endpoint: https://docs.cardless.com/mcp/oauth/register\n  dynamic_client_registration: true\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  flows:\n  - flow: authorizationCode\n  \
  \  authorizationUrl: https://docs.cardless.com/mcp/oauth/authorize\n    tokenUrl: https://docs.cardless.com/mcp/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://docs.cardless.com/mcp/oauth/token\n  - flow: refreshToken\n    tokenUrl: https://docs.cardless.com/mcp/oauth/token\nscopes:\n- scope: mcp:search\n  description: Search and read the Cardless documentation corpus through the MCP server.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/cardless-oauth-authorization-server.json]\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://docs.cardless.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardless/refs/heads/main/scopes/cardless-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Financial-Services
- Fintech
- Credit Cards
- Card Issuing
- Embedded Finance
- Payments
- Banking as a Service
- Lending
- Co-Branded Cards
- Loyalty
token_urls:
- https://docs.cardless.com/mcp/oauth/token
---
