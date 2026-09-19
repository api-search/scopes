---
api_specs:
- filename: mitratech-dashboard-api-openapi.yml
  format: yaml
  label: Mitratech Dashboard API
  slug: mitratech-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-dashboard-api-openapi.yml
- filename: mitratech-files-api-openapi.yml
  format: yaml
  label: Mitratech Files API
  slug: mitratech-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-files-api-openapi.yml
- filename: mitratech-gridconfigurations-api-openapi.yml
  format: yaml
  label: Mitratech Grid Configurations API
  slug: mitratech-gridconfigurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-gridconfigurations-api-openapi.yml
- filename: mitratech-templates-api-openapi.yml
  format: yaml
  label: Mitratech Templates API
  slug: mitratech-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-templates-api-openapi.yml
- filename: mitratech-users-api-openapi.yml
  format: yaml
  label: Mitratech Users API
  slug: mitratech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-users-api-openapi.yml
- filename: mitratech-workflow-api-openapi.yml
  format: yaml
  label: Mitratech Workflow API
  slug: mitratech-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-workflow-api-openapi.yml
- filename: mitratech-workflows-api-openapi.yml
  format: yaml
  label: Mitratech Workflows API
  slug: mitratech-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-workflows-api-openapi.yml
- filename: mitratech-health-check-api-openapi.yml
  format: yaml
  label: Mitratech Health Check API
  slug: mitratech-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/openapi/mitratech-health-check-api-openapi.yml
authorization_urls: []
description: ''
docs: https://success.mitratech.com/TAP/TAP_Solutions/APIs_and_Integrations/TAP_API_Documentation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mitratech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mitratech uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mitratech
provider_slug: mitratech
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: mitratech-scopes
source_filename: mitratech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://success.mitratech.com/TAP/TAP_Solutions/APIs_and_Integrations/TAP_API_Documentation +\n  https://mitratech.com/.well-known/oauth-authorization-server +\n  https://mitratech.com/.well-known/oauth-protected-resource\ndocs: https://success.mitratech.com/TAP/TAP_Solutions/APIs_and_Integrations/TAP_API_Documentation\nsummary: >-\n  Mitratech's OAuth surfaces are scope-bearing but scope-poor. Both published scope vocabularies are a\n  single opaque value, and neither is a permission vocabulary — authorization on TAP is carried by the\n  TAP user account behind the token, not by the scope.\nscopes:\n- name: api\n  api: Mitratech TAP Workflow Automation API\n  description: >-\n    The only scope value documented for the TAP token request. Sent as `scope=api` in the\n    password-grant body to /auth/identity/connect/token.\n  source: https://success.mitratech.com/TAP/TAP_Solutions/APIs_and_Integrations/TAP_API_Documentation\n\
  - name: mcp\n  api: Mitratech MCP Server\n  description: >-\n    The only scope in scopes_supported on both the RFC 8414 authorization-server metadata and the\n    RFC 9728 protected-resource metadata at mitratech.com.\n  source: https://mitratech.com/.well-known/oauth-authorization-server\nscope_count: 2\nnotes:\n- >-\n  TeamConnect's OAuth documentation describes scope as \"(Optional) Specify the scope required for\n  access\" and publishes no scope values at all. No TeamConnect scopes are recorded here because none\n  are published — an honest absence, not an omission.\n- >-\n  Least privilege is not expressible on TAP. Mitratech's own guidance is to use a Super Admin account\n  to obtain the token, warning that a narrower account may silently return incomplete results. An\n  agent therefore cannot be granted a read-only or single-object token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitratech/refs/heads/main/scopes/mitratech-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Legal
- Legal Operations
- Enterprise Legal Management
- Matter Management
- Governance Risk and Compliance
- Compliance
- Workflow-Automation
- Contract Lifecycle Management
- HR Compliance
- Risk Management
- Immigration
- OData
- MCP
token_urls: []
---
