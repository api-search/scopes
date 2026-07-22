---
api_specs:
- filename: runwhen-papi-openapi-original.json
  format: json
  label: RunWhen Platform API (PAPI)
  slug: runwhen-platform-api-papi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runwhen/refs/heads/main/openapi/runwhen-papi-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.runwhen.com/docs/use/api-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Runwhen Scopes
name_suffix: OAuth Scopes
note: RunWhen PAPI resource endpoints authenticate with JWT Bearer tokens (no per-endpoint OAuth scopes). The OAuth/OIDC authorization server advertises the standard OIDC scopes below for interactive login.
overview: 'RunWhen publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the RunWhen API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RunWhen
provider_slug: runwhen
schemes:
- authorizationUrl: https://papi.beta.runwhen.com/oauth/authorize
  grants:
  - authorization_code
  - refresh_token
  name: RunWhenOAuth
  pkce: S256
  tokenUrl: https://papi.beta.runwhen.com/oauth/token
  type: oauth2-oidc
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access the user's basic profile claims.
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
slug: runwhen-scopes
source_filename: runwhen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://papi.beta.runwhen.com/.well-known/openid-configuration\ndocs: https://docs.runwhen.com/docs/use/api-reference\nnote: RunWhen PAPI resource endpoints authenticate with JWT Bearer tokens (no per-endpoint OAuth scopes).\n  The OAuth/OIDC authorization server advertises the standard OIDC scopes below for interactive login.\nschemes:\n- name: RunWhenOAuth\n  type: oauth2-oidc\n  authorizationUrl: https://papi.beta.runwhen.com/oauth/authorize\n  tokenUrl: https://papi.beta.runwhen.com/oauth/token\n  pkce: S256\n  grants:\n  - authorization_code\n  - refresh_token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n- scope: profile\n  description: Access the user's basic profile claims.\n- scope: email\n  description: Access the user's email address.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runwhen/refs/heads/main/scopes/runwhen-scopes.yml
summary_line: 3 scopes
tags:
- Company
- AIOps
- SRE
- DevOps
- Observability
- Incident Response
- AI Agents
- Kubernetes
- Automation
- MCP
token_urls: []
---
