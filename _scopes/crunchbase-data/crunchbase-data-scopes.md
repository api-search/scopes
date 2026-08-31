---
api_specs:
- filename: crunchbase-data-autocomplete-api-openapi.yml
  format: yaml
  label: Crunchbase Autocomplete API
  slug: crunchbase-data-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-autocomplete-api-openapi.yml
- filename: crunchbase-data-deleted-entities-api-openapi.yml
  format: yaml
  label: Crunchbase Deleted Entities API
  slug: crunchbase-data-deleted-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-deleted-entities-api-openapi.yml
- filename: crunchbase-data-entity-api-openapi.yml
  format: yaml
  label: Crunchbase Entity API
  slug: crunchbase-data-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-entity-api-openapi.yml
- filename: crunchbase-data-metadata-api-openapi.yml
  format: yaml
  label: Crunchbase Metadata API
  slug: crunchbase-data-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-metadata-api-openapi.yml
- filename: crunchbase-data-search-api-openapi.yml
  format: yaml
  label: Crunchbase Search API
  slug: crunchbase-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-search-api-openapi.yml
authorization_urls:
- https://www.crunchbase.com/oauth/authorize
description: 'The REST Data API has no OAuth surface at all - it is a single account-level API key (X-cb-user-key) with no scopes, so the six published OpenAPI documents declare no oauth2 security scheme and derive-oauth-scopes.py correctly finds nothing. The OAuth surface belongs entirely to the MCP server: mcp.crunchbase.com is an RFC 9728 protected resource whose authorization server is www.crunchbase.com, and both metadata documents are anonymously readable. The scopes below are read verbatim from those two live documents, not from the specs.'
docs: https://data.crunchbase.com/docs/connecting-ai-tools
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Crunchbase Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Crunchbase publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Crunchbase API on a user''s behalf.


  Tokens are issued from https://oauth.crunchbase.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Crunchbase
provider_slug: crunchbase-data
schemes:
- flows:
  - authorizationUrl: https://www.crunchbase.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://oauth.crunchbase.com/revoke
    tokenUrl: https://oauth.crunchbase.com/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://www.crunchbase.com
  name: OAuth 2.1
  pkce_methods:
  - plain
  - S256
  response_types:
  - code
  source: https://www.crunchbase.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - client_secret_post
  - none
scope_count: 2
scope_names:
- offline_access
- lists.read
scopes:
- description: Issues a refresh token so the client can keep calling the MCP server after the access token expires without re-prompting the user.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read access to the signed-in user's Crunchbase saved lists. Backs the cb_list_query and cb_list_get MCP tools.
  flows:
  - authorizationCode
  scope: lists.read
slug: crunchbase-data-scopes
source_filename: crunchbase-data-scopes.yml
source_heading: OAuth Scopes
source_url: https://www.crunchbase.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://www.crunchbase.com/.well-known/oauth-authorization-server\nsources:\n- https://www.crunchbase.com/.well-known/oauth-authorization-server\n- https://mcp.crunchbase.com/.well-known/oauth-protected-resource\n- https://data.crunchbase.com/docs/connecting-ai-tools\ndocs: https://data.crunchbase.com/docs/connecting-ai-tools\ndescription: >-\n  The REST Data API has no OAuth surface at all - it is a single account-level API\n  key (X-cb-user-key) with no scopes, so the six published OpenAPI documents declare\n  no oauth2 security scheme and derive-oauth-scopes.py correctly finds nothing. The\n  OAuth surface belongs entirely to the MCP server: mcp.crunchbase.com is an RFC\n  9728 protected resource whose authorization server is www.crunchbase.com, and both\n  metadata documents are anonymously readable. The scopes below are read verbatim\n  from those two live documents, not from the specs.\napplies_to: MCP server (https://mcp.crunchbase.com)\
  \ - NOT the REST Data API\nschemes:\n- name: OAuth 2.1\n  source: https://www.crunchbase.com/.well-known/oauth-authorization-server\n  issuer: https://www.crunchbase.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.crunchbase.com/oauth/authorize\n    tokenUrl: https://oauth.crunchbase.com/token\n    revocationUrl: https://oauth.crunchbase.com/revoke\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  pkce_methods:\n  - plain\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\nscopes:\n- scope: offline_access\n  description: >-\n    Issues a refresh token so the client can keep calling the MCP server after the\n    access token expires without re-prompting the user.\n  advertised_by:\n  - https://www.crunchbase.com/.well-known/oauth-authorization-server\n  - https://mcp.crunchbase.com/.well-known/oauth-protected-resource\n  flows:\n  - authorizationCode\n- scope: lists.read\n  description: >-\n\
  \    Read access to the signed-in user's Crunchbase saved lists. Backs the\n    cb_list_query and cb_list_get MCP tools.\n  advertised_by:\n  - https://www.crunchbase.com/.well-known/oauth-authorization-server\n  flows:\n  - authorizationCode\nnotes: >-\n  Two scopes only, and the pair is narrower than the tool surface it fronts: the MCP\n  Tool Reference documents cb_list_create and cb_list_add_entities as write\n  operations against Crunchbase lists, but no lists.write scope is advertised in\n  either metadata document, and the protected-resource document at\n  mcp.crunchbase.com advertises offline_access alone. Data access itself is not\n  scoped - it is governed by the MCP seat assigned to the user's account, which\n  Crunchbase documents as carrying its highest level of data access including\n  predictions and insights. Dynamic Client Registration is explicitly not supported;\n  clients either present a Client ID Metadata Document or use a client_id/secret\n  pre-registered by a Crunchbase\
  \ CSM.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/scopes/crunchbase-data-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company Data
- Web Intelligence
- Funding Data
- Firmographics
- B2B Data
- Investor Data
- Reference Data
- Private Markets
- Predictions
- Market Insights
- MCP
- Fortune 1000
token_urls:
- https://oauth.crunchbase.com/token
---
