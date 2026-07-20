---
authorization_urls:
- https://kfinance.kensho.com/integrations/authorize
description: ''
docs: https://docs.kensho.com/llmreadyapi/mcp/custom/oauth-client-credentials
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Kensho Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kensho publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kensho API on a user''s behalf.


  Tokens are issued from https://kfinance.kensho.com/integrations/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kensho
provider_slug: kensho
schemes:
- flows:
  - authorizationUrl: https://kfinance.kensho.com/integrations/authorize
    flow: authorizationCode
    tokenUrl: https://kfinance.kensho.com/integrations/token
  - flow: clientCredentials
    tokenUrl: https://kfinance.kensho.com/integrations/token
  - flow: refreshToken
    tokenUrl: https://kfinance.kensho.com/integrations/token
  issuer: https://kfinance.kensho.com/integrations
  name: OAuth2
  source: well-known/kensho-oauth-authorization-server.json
scope_count: 2
scope_names:
- kensho:app:kfinance
- offline_access
scopes:
- description: Access to the Kensho LLM-ready API (kfinance) application and its S&P Global financial-data retrieval surface via the hosted MCP server.
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  scope: kensho:app:kfinance
- description: Issue a refresh token so the client can obtain new access tokens without re-authorization (OpenID Connect / OAuth 2.0 offline access).
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
slug: kensho-scopes
source_filename: kensho-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://kfinance.kensho.com/.well-known/oauth-authorization-server\ndocs: https://docs.kensho.com/llmreadyapi/mcp/custom/oauth-client-credentials\nschemes:\n- name: OAuth2\n  source: well-known/kensho-oauth-authorization-server.json\n  issuer: https://kfinance.kensho.com/integrations\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://kfinance.kensho.com/integrations/authorize\n    tokenUrl: https://kfinance.kensho.com/integrations/token\n  - flow: clientCredentials\n    tokenUrl: https://kfinance.kensho.com/integrations/token\n  - flow: refreshToken\n    tokenUrl: https://kfinance.kensho.com/integrations/token\nscopes:\n- scope: kensho:app:kfinance\n  description: >-\n    Access to the Kensho LLM-ready API (kfinance) application and its S&P Global\n    financial-data retrieval surface via the hosted MCP server.\n  flows: [authorizationCode, clientCredentials, refreshToken]\n  sources: [well-known/kensho-oauth-authorization-server.json]\n\
  - scope: offline_access\n  description: >-\n    Issue a refresh token so the client can obtain new access tokens without\n    re-authorization (OpenID Connect / OAuth 2.0 offline access).\n  flows: [authorizationCode, refreshToken]\n  sources: [well-known/kensho-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kensho/refs/heads/main/scopes/kensho-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Financial Data
- Speech to Text
- Transcription
- Document Extraction
- Named Entity Recognition
- Natural Language Processing
- LLM
- Model Context Protocol
- Retrieval
- S&P Global
token_urls:
- https://kfinance.kensho.com/integrations/token
---
