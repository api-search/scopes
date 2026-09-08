---
api_specs:
- filename: upstox-developer-api-openapi.yml
  format: yaml
  label: Upstox Developer API
  slug: upstox-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upstox/refs/heads/main/openapi/upstox-developer-api-openapi.yml
authorization_urls:
- https://api.upstox.com/v2/login/authorization/dialog
description: 'Upstox declares exactly two OAuth scopes — read and write — in its OpenAPI securityScheme, and it publishes no scope reference page. There is no per-resource or per-operation scope vocabulary: an app either reads or it can also trade. The practical permissioning happens elsewhere — token type (standard vs extended vs Analytics Token), app configuration in the developer console, static-IP registration for algo order flow, and the user-controlled kill switch. An agent cannot request a narrow, least-privilege grant such as "portfolio read only" through the scope parameter.'
docs: https://upstox.com/developer/api-documentation/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Upstox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upstox publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Upstox API on a user''s behalf.


  Tokens are issued from https://api.upstox.com/v2/login/authorization/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upstox
provider_slug: upstox
schemes:
- flows:
  - authorizationUrl: https://api.upstox.com/v2/login/authorization/dialog
    flow: authorizationCode
    tokenUrl: https://api.upstox.com/v2/login/authorization/token
  name: OAUTH2
  source: openapi/upstox-developer-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: upstox-scopes
source_filename: upstox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  openapi/upstox-developer-api-openapi.yml (derived baseline) upgraded with\n  https://upstox.com/developer/api-documentation/authentication and\n  https://upstox.com/developer/api-documentation/analytics-token\ndocs: https://upstox.com/developer/api-documentation/authentication\nname: Upstox OAuth scopes\ndescription: >-\n  Upstox declares exactly two OAuth scopes — read and write — in its OpenAPI securityScheme, and it\n  publishes no scope reference page. There is no per-resource or per-operation scope vocabulary: an app\n  either reads or it can also trade. The practical permissioning happens elsewhere — token type\n  (standard vs extended vs Analytics Token), app configuration in the developer console, static-IP\n  registration for algo order flow, and the user-controlled kill switch. An agent cannot request a\n  narrow, least-privilege grant such as \"portfolio read only\" through the scope parameter.\nschemes:\n\
  - name: OAUTH2\n  source: openapi/upstox-developer-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.upstox.com/v2/login/authorization/dialog\n    tokenUrl: https://api.upstox.com/v2/login/authorization/token\nscopes:\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upstox-developer-api-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/upstox-developer-api-openapi.yml\nscope_count: 2\ngranularity: coarse\nalternative_permissioning:\n- mechanism: Analytics Token\n  effect: A read-only token with 1-year validity. Market data is unrestricted; account-scoped reads additionally require a registered static IP.\n  docs: https://upstox.com/developer/api-documentation/analytics-token\n- mechanism: extended_token\n  effect: A longer-lived token that is refused on some APIs, returning UDAPI100067.\n- mechanism: Sandbox token\n  effect: Scoped\
  \ to sandbox orders only; cannot be used against live endpoints.\n- mechanism: Static IP allowlist\n  effect: Order and algo-trading flow is constrained to registered primary and optional secondary IPs per the 5 May 2025 exchange circular.\n  docs: https://upstox.com/developer/api-documentation/update-app-static-ips\n- mechanism: Kill switch\n  effect: The end user can disable trading per segment, blocking new orders and cancelling pending ones regardless of the token's scope.\n  docs: https://upstox.com/developer/api-documentation/update-kill-switch\n- mechanism: MCP server boundary\n  effect: >-\n    The hosted MCP server is read-only by construction — it exposes no write tool at all, which is a\n    stronger guarantee than the write scope being withheld.\n  docs: mcp/upstox-mcp.yml\ngaps:\n- No published scopes or permissions reference page — the two scopes are discoverable only from the OpenAPI securityScheme.\n- No per-resource scopes (no orders:read, portfolio:read, funds:write equivalents).\n\
  - No incremental or step-up authorization documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstox/refs/heads/main/scopes/upstox-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Financial Services
- Stock Trading
- Brokerage
- Market Data
- Investing
- Capital Markets
- Mutual Funds
- Algorithmic Trading
- India
token_urls:
- https://api.upstox.com/v2/login/authorization/token
---
