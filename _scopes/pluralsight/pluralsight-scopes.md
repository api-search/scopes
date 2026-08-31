---
api_specs:
- filename: pluralsight-catalog-api-openapi.yml
  format: yaml
  label: Pluralsight Catalog API
  slug: pluralsight-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-catalog-api-openapi.yml
- filename: pluralsight-coding-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Coding Metrics API
  slug: pluralsight-coding-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-coding-metrics-api-openapi.yml
- filename: pluralsight-collaboration-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight Collaboration Metrics API
  slug: pluralsight-collaboration-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-collaboration-metrics-api-openapi.yml
- filename: pluralsight-commits-api-openapi.yml
  format: yaml
  label: Pluralsight Commits API
  slug: pluralsight-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-commits-api-openapi.yml
- filename: pluralsight-dora-metrics-api-openapi.yml
  format: yaml
  label: Pluralsight DORA Metrics API
  slug: pluralsight-dora-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-dora-metrics-api-openapi.yml
- filename: pluralsight-graphql-api-openapi.yml
  format: yaml
  label: Pluralsight GraphQL API
  slug: pluralsight-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-graphql-api-openapi.yml
- filename: pluralsight-integrations-api-openapi.yml
  format: yaml
  label: Pluralsight Integrations API
  slug: pluralsight-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-integrations-api-openapi.yml
- filename: pluralsight-licensing-api-openapi.yml
  format: yaml
  label: Pluralsight Licensing API
  slug: pluralsight-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-licensing-api-openapi.yml
- filename: pluralsight-pull-requests-api-openapi.yml
  format: yaml
  label: Pluralsight Pull Requests API
  slug: pluralsight-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-pull-requests-api-openapi.yml
- filename: pluralsight-reports-api-openapi.yml
  format: yaml
  label: Pluralsight Reports API
  slug: pluralsight-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-reports-api-openapi.yml
- filename: pluralsight-repos-api-openapi.yml
  format: yaml
  label: Pluralsight Repos API
  slug: pluralsight-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-repos-api-openapi.yml
- filename: pluralsight-teams-api-openapi.yml
  format: yaml
  label: Pluralsight Teams API
  slug: pluralsight-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-teams-api-openapi.yml
- filename: pluralsight-tickets-api-openapi.yml
  format: yaml
  label: Pluralsight Tickets API
  slug: pluralsight-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-tickets-api-openapi.yml
- filename: pluralsight-users-api-openapi.yml
  format: yaml
  label: Pluralsight Users API
  slug: pluralsight-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/openapi/pluralsight-users-api-openapi.yml
authorization_urls: []
description: Pluralsight's only OAuth-scoped surface is its remote MCP gateway. The Skills GraphQL API uses plan-admin API keys with no OAuth scopes at all - entitlement there is expressed as release-stage access on the key plus plan permissions, not as scopes. The four scopes below are published anonymously in the gateway's RFC 9728 protected-resource metadata and its RFC 8414 authorization-server metadata.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Pluralsight Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pluralsight uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pluralsight
provider_slug: pluralsight
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: pluralsight-scopes
source_filename: pluralsight-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://mcp.pluralsight.com/.well-known/oauth-protected-resource\nprovider: Pluralsight\nproviderId: pluralsight\ndescription: >-\n  Pluralsight's only OAuth-scoped surface is its remote MCP gateway. The Skills GraphQL API uses\n  plan-admin API keys with no OAuth scopes at all - entitlement there is expressed as release-stage\n  access on the key plus plan permissions, not as scopes. The four scopes below are published\n  anonymously in the gateway's RFC 9728 protected-resource metadata and its RFC 8414\n  authorization-server metadata.\ndocs: null\ndocs_note: >-\n  No human-readable scopes reference page exists. These values come from the machine-readable\n  discovery documents only; the semantics below are read from the scope names and are marked as\n  inferred where Pluralsight does not describe them.\nsurfaces:\n- name: Pluralsight MCP Gateway\n  resource: https://mcp.pluralsight.com/mcp\n  authorization_server: https://mcp.pluralsight.com\n\
  \  flow: authorization_code\n  pkce: S256\n  bearer_methods_supported:\n  - header\n  scopes:\n  - name: invoke:gateway\n    description: Call tools exposed through the gateway.\n    inferred: true\n  - name: author:gateway\n    description: Authoring-level access to gateway tools.\n    inferred: true\n  - name: employee:gateway\n    description: Pluralsight-employee-level access to gateway tools.\n    inferred: true\n  - name: admin:gateway\n    description: Administrative access to the gateway.\n    inferred: true\n  note: >-\n    Pluralsight publishes the scope STRINGS but not their meanings. The descriptions above are read\n    from the names and are flagged inferred; none is quoted from Pluralsight documentation.\n- name: Skills GraphQL API\n  resource: https://paas-api.pluralsight.com/graphql\n  scheme: apiKey\n  scopes: []\n  note: >-\n    No OAuth. Access is gated by (a) whether the plan has the API entitlement\n    (https://developer.pluralsight.com/plan-permissions) and (b) the\
  \ release stage attached to the\n    individual API key (GR / Beta / Alpha). That is an entitlement model, not a scope model - an\n    agent cannot request a narrower grant than the key already carries.\nx-evidence:\n- fetched: '2026-08-29'\n  url: https://mcp.pluralsight.com/.well-known/oauth-protected-resource\n  http_status: 200\n  file: ../well-known/pluralsight-mcp-oauth-protected-resource.json\n- fetched: '2026-08-29'\n  url: https://mcp.pluralsight.com/.well-known/oauth-authorization-server\n  http_status: 200\n  file: ../well-known/pluralsight-mcp-oauth-authorization-server.json\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pluralsight/refs/heads/main/scopes/pluralsight-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Courses
- Education
- Engineering Metrics
- Learning
- Skills Assessment
- Technology
- Video Training
token_urls: []
---
