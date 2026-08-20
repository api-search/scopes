---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Agibot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AgiBot uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AgiBot
provider_slug: agibot
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agibot-scopes
source_filename: agibot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://store-account.agibot.com/.well-known/openid-configuration\nnotes: Scopes are declared by the AGIBOT customer-account authorization server discovery document. They\n  apply to the store commerce surface only; the AimDK robot protocol defines no scopes.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://store-account.agibot.com/.well-known/openid-configuration\n  http_status: 200\nflows:\n- authorization_code\n- refresh_token\n- urn:ietf:params:oauth:grant-type:jwt-bearer\npkce_required_methods:\n- S256\nscopes:\n- name: openid\n  description: Request an OpenID Connect ID token for the signed-in AGIBOT store customer.\n- name: email\n  description: Read the customer’s email address and its verification state.\n- name: customer-account-api:full\n  description: Full access to the customer account API for the signed-in customer.\n- name: customer-account-mcp-api:full\n  description: Full access to the customer-account\
  \ MCP API — the customer-scoped half of the agent commerce\n    surface.\nclaims:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agibot/refs/heads/main/scopes/agibot-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Robotics
- Humanoid Robots
- Embodied AI
- Artificial Intelligence
- Manufacturing
- Hardware
- Middleware
- ROS 2
- gRPC
- Protocol Buffers
- Simulation
- Machine-Learning
- Open-Source
- MCP
- Agentic Commerce
- China
token_urls: []
---
