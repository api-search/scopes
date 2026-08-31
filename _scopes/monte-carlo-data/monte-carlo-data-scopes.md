---
authorization_urls: []
description: ''
docs: https://docs.getmontecarlo.com/docs/api-authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Monte Carlo Data Scopes
name_suffix: OAuth Scopes
note: 'Monte Carlo runs two distinct OAuth scope vocabularies. The MCP/OIDC authorization server at auth.getmontecarlo.com advertises the standard OIDC set plus offline_access. The GraphQL API''s client-credentials flow uses resource-URI scopes instead — an access scope plus an instance-routing scope that names the deployment region. Fine-grained permissioning in Monte Carlo is NOT expressed as OAuth scopes: it is carried by roles, authorization groups and domains, which is why the scope list is short.'
overview: 'Monte Carlo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Monte Carlo
provider_slug: monte-carlo-data
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: monte-carlo-data-scopes
source_filename: monte-carlo-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  live read of https://auth.getmontecarlo.com/.well-known/oauth-authorization-server\n  and https://mcp.getmontecarlo.com/.well-known/oauth-protected-resource/mcp,\n  plus https://docs.getmontecarlo.com/docs/api-authentication\ndocs: https://docs.getmontecarlo.com/docs/api-authentication\nprovider: Monte Carlo\nproviderId: monte-carlo-data\nnote: >-\n  Monte Carlo runs two distinct OAuth scope vocabularies. The MCP/OIDC\n  authorization server at auth.getmontecarlo.com advertises the standard OIDC\n  set plus offline_access. The GraphQL API's client-credentials flow uses\n  resource-URI scopes instead — an access scope plus an instance-routing scope\n  that names the deployment region. Fine-grained permissioning in Monte Carlo\n  is NOT expressed as OAuth scopes: it is carried by roles, authorization\n  groups and domains, which is why the scope list is short.\nauthorization_servers:\n  - issuer: https://auth.getmontecarlo.com\n\
  \    metadata: https://auth.getmontecarlo.com/.well-known/oauth-authorization-server\n    openid_configuration: https://auth.getmontecarlo.com/.well-known/openid-configuration\n    scopes:\n      - name: openid\n        description: OIDC — issue an ID token for the authenticating user.\n      - name: profile\n        description: OIDC — basic profile claims.\n      - name: email\n        description: OIDC — email claim.\n      - name: offline_access\n        description: >-\n          Issue a refresh token. This is the ONLY scope the MCP protected\n          resource declares as supported (scopes_supported in\n          /.well-known/oauth-protected-resource/mcp), and it is the scope named\n          in the MCP endpoint's WWW-Authenticate challenge.\n  - issuer: https://api.getmontecarlo.com\n    flow: client_credentials\n    token_endpoint: https://api.getmontecarlo.com/oauth2/token\n    scopes:\n      - name: https://api.getmontecarlo.com/access\n        description: Grants access to\
  \ the Monte Carlo GraphQL API.\n      - name: https://instance.getmontecarlo.com/{instance_id}\n        description: >-\n          Instance-routing scope naming the customer's deployment (e.g. us1,\n          eu1). Required alongside the access scope; the instance ID is shown\n          under Account Information -> Instance ID.\n        templated: true\nprotected_resources:\n  - resource: https://mcp.getmontecarlo.com/mcp\n    authorization_servers:\n      - https://auth.getmontecarlo.com\n    scopes_supported:\n      - offline_access\n    bearer_methods_supported:\n      - header\n    metadata_url: https://mcp.getmontecarlo.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\nnon_oauth_authorization:\n  model: roles + authorization groups + domains\n  note: >-\n    MCP access requires the Editor role or above. Account-level API key\n    creation, service OAuth client creation and SSO editing are each governed\n    by named role permissions. Ingestion keys are additionally\
  \ scoped by\n    warehouseIds.\n  docs: https://docs.getmontecarlo.com/docs/authorization\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monte-carlo-data/refs/heads/main/scopes/monte-carlo-data-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AIOps
- Data Observability
- Data Quality
- Data Lineage
- Agent Observability
- Monitoring
- GraphQL
- MCP
- OpenTelemetry
- Data Engineering
token_urls: []
---
