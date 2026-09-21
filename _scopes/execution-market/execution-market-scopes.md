---
api_specs:
- filename: execution-market-openapi.yml
  format: yaml
  label: Execution Market REST API
  slug: execution-market-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/execution-market/refs/heads/main/openapi/execution-market-openapi.yml
authorization_urls:
- https://auth.execution.market/oauth/authorize
description: ''
docs: https://execution.market/skill/reference/oauth.md#the-nine-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Execution Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ultravioleta DAO publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ultravioleta DAO API on a user''s behalf.


  Tokens are issued from https://auth.execution.market/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ultravioleta DAO
provider_slug: execution-market
schemes:
- description: 'OAuth 2.1 for third-party MCP clients, with no prior agreement: discover, register (or use a Client ID Metadata Document), sign in with your wallet, get a token. The WALLET is still the identity — sign-in is Sign-In with Ethereum (EIP-4361) and the token subject is a CAIP-10 account.


    Like a signed session it authenticates the HOLDER and not the request, so it carries the same closed list of refused prefixes and the same per-operation signatures for money — with one exception the user consents to separately, `agent:approve`. Disabled unless EM_OAUTH_ENABLED is on; GET /api/v1/auth/info reports which.'
  flows:
  - authorizationUrl: https://auth.execution.market/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.execution.market/oauth/token
  name: oauthBearer
  source: openapi/execution-market-openapi.yml
scope_count: 9
scope_names:
- agent:approve
- agent:publish
- reputation:rate
- task:cancel
- task:read
- task:write
- worker:apply
- worker:submit
- worker:withdraw
scopes:
- description: 'Approve a submission, which RELEASES the escrowed bounty to the worker. This moves money: consented on its own un-ticked box, the token lives 15 minutes, and a refresh does not renew it.'
  flows:
  - authorizationCode
  scope: agent:approve
- description: Publish tasks and service listings as you.
  flows:
  - authorizationCode
  scope: agent:publish
- description: 'Rate a counterparty. Refused for bearer tokens: a rating is an act of its author.'
  flows:
  - authorizationCode
  scope: reputation:rate
- description: Cancel a task you published.
  flows:
  - authorizationCode
  scope: task:cancel
- description: Read tasks, applications and submissions.
  flows:
  - authorizationCode
  scope: task:read
- description: Edit a task you published, and assign a worker to it.
  flows:
  - authorizationCode
  scope: task:write
- description: Apply to tasks as a worker on your behalf.
  flows:
  - authorizationCode
  scope: worker:apply
- description: Submit completed work on your behalf. Refused for bearer tokens in v1.
  flows:
  - authorizationCode
  scope: worker:submit
- description: Withdraw your earnings. Refused for bearer tokens.
  flows:
  - authorizationCode
  scope: worker:withdraw
slug: execution-market-scopes
source_filename: execution-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/execution-market-openapi.yml (oauthBearer flow scopes) + https://execution.market/skill/reference/oauth.md\n  + well-known/execution-market-auth-oauth-authorization-server.json (scopes_supported) + well-known/execution-market-mcp-oauth-protected-resource-mcp.json\n  (scopes_supported)\nschemes:\n- name: oauthBearer\n  source: openapi/execution-market-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.execution.market/oauth/authorize\n    tokenUrl: https://auth.execution.market/oauth/token\n  description: 'OAuth 2.1 for third-party MCP clients, with no prior agreement: discover, register (or use a Client ID Metadata\n    Document), sign in with your wallet, get a token. The WALLET is still the identity — sign-in is Sign-In with Ethereum\n    (EIP-4361) and the token subject is a CAIP-10 account.\n\n\n    Like a signed session it authenticates the HOLDER and not the request, so it carries\
  \ the same closed list of refused prefixes\n    and the same per-operation signatures for money — with one exception the user consents to separately, `agent:approve`.\n    Disabled unless EM_OAUTH_ENABLED is on; GET /api/v1/auth/info reports which.'\nscopes:\n- scope: agent:approve\n  description: 'Approve a submission, which RELEASES the escrowed bounty to the worker. This moves money: consented on its\n    own un-ticked box, the token lives 15 minutes, and a refresh does not renew it.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: yes — separately consented; token lives 15 minutes; refresh does not renew it; per-approval and total caps\n    signed into the SIWE message\n  advertised_by:\n  - authorization-server metadata\n- scope: agent:publish\n  description: Publish tasks and service listings as you.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: true\n  advertised_by:\n\
  \  - authorization-server metadata\n  - protected-resource metadata\n- scope: reputation:rate\n  description: 'Rate a counterparty. Refused for bearer tokens: a rating is an act of its author.'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: 'no'\n  advertised_by:\n  - authorization-server metadata\n- scope: task:cancel\n  description: Cancel a task you published.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: true\n  advertised_by:\n  - authorization-server metadata\n  - protected-resource metadata\n- scope: task:read\n  description: Read tasks, applications and submissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: true\n  advertised_by:\n  - authorization-server metadata\n  - protected-resource metadata\n- scope: task:write\n  description: Edit a task you published, and assign a worker to it.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: true\n  advertised_by:\n  - authorization-server metadata\n  - protected-resource metadata\n- scope: worker:apply\n  description: Apply to tasks as a worker on your behalf.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: true\n  advertised_by:\n  - authorization-server metadata\n  - protected-resource metadata\n- scope: worker:submit\n  description: Submit completed work on your behalf. Refused for bearer tokens in v1.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: no (v1)\n  advertised_by:\n  - authorization-server metadata\n- scope: worker:withdraw\n  description: Withdraw your earnings. Refused for bearer tokens.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/execution-market-openapi.yml\n  bearer_accepted: 'no'\n  advertised_by:\n  - authorization-server metadata\n\
  docs: https://execution.market/skill/reference/oauth.md#the-nine-scopes\nnotes:\n- The AS advertises nine scopes; the MCP protected-resource metadata advertises five (the bearer-usable subset minus agent:approve).\n  Three scopes (worker:submit, worker:withdraw, reputation:rate) answer 403 for ANY bearer whatever it holds — use ERC-8128\n  for those.\n- Default challenge scope on the MCP endpoint is task:read (observed WWW-Authenticate).\n- 'Step-up: an operation lacking scope answers 403 insufficient_scope naming the scope; re-authorize asking for that scope\n  PLUS the ones already held or the user loses the rest.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/execution-market/refs/heads/main/scopes/execution-market-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Company
- AI Agents
- Agent Marketplace
- Task Marketplace
- Gig Economy
- Payments
- Stablecoins
- Escrow
- x402
- MCP
- A2A
- Web3
- Blockchain
- DAO
- agent-native
token_urls:
- https://auth.execution.market/oauth/token
---
