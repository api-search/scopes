---
authorization_urls:
- https://api.intacct.com/ia/authorize
description: ''
docs: https://developer.sage.com/intacct/docs/1/sage-intacct-rest-api/api-essentials
flows:
- authorizationCode
- clientCredentials
- tokenExchange
kind: oauth-scopes
layout: scope
method: searched
name: Intacct Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sage Intacct publishes 4 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and tokenExchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sage Intacct API on a user''s behalf.


  Tokens are issued from https://api.intacct.com/ia/api/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sage Intacct
provider_slug: intacct
schemes:
- flows:
  - authorizationUrl: https://api.intacct.com/ia/authorize
    flow: authorizationCode
    tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token
  - flow: tokenExchange
    tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token
  issuer: https://api.intacct.com
  name: OAuth2 / OpenID Connect
  source: well-known/intacct-openid-configuration.json
scope_count: 4
scope_names:
- openid
- offline_access
- sage/ai-agents
- token-exchange
scopes:
- description: Request an OpenID Connect ID token identifying the authenticated user/company.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the client can obtain new access tokens without user interaction.
  flows:
  - authorizationCode
  scope: offline_access
- description: Grant AI agents / MCP clients governed access to Sage Intacct data via the AI Gateway.
  flows:
  - authorizationCode
  - clientCredentials
  - tokenExchange
  scope: sage/ai-agents
- description: Permit RFC 8693 OAuth 2.0 token exchange (delegation/impersonation) for downstream calls.
  flows:
  - tokenExchange
  scope: token-exchange
slug: intacct-scopes
source_filename: intacct-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.intacct.com/.well-known/openid-configuration\ndocs: https://developer.sage.com/intacct/docs/1/sage-intacct-rest-api/api-essentials\nschemes:\n- name: OAuth2 / OpenID Connect\n  source: well-known/intacct-openid-configuration.json\n  issuer: https://api.intacct.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.intacct.com/ia/authorize\n    tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token\n  - flow: tokenExchange\n    tokenUrl: https://api.intacct.com/ia/api/v1/oauth2/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token identifying the authenticated user/company.\n  flows: [authorizationCode]\n  sources: [well-known/intacct-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without\
  \ user interaction.\n  flows: [authorizationCode]\n  sources: [well-known/intacct-openid-configuration.json]\n- scope: sage/ai-agents\n  description: Grant AI agents / MCP clients governed access to Sage Intacct data via the AI Gateway.\n  flows: [authorizationCode, clientCredentials, tokenExchange]\n  sources: [well-known/intacct-openid-configuration.json]\n- scope: token-exchange\n  description: Permit RFC 8693 OAuth 2.0 token exchange (delegation/impersonation) for downstream calls.\n  flows: [tokenExchange]\n  sources: [well-known/intacct-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intacct/refs/heads/main/scopes/intacct-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials/tokenExchange
tags:
- Company
- Accounting
- ERP
- Financial Management
- Cloud Accounting
- Invoicing
- Payments
- SaaS
- REST API
- OAuth
token_urls:
- https://api.intacct.com/ia/api/v1/oauth2/token
---
