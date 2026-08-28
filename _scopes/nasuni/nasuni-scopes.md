---
api_specs:
- filename: nasuni-nmc-v1-2-openapi.yml
  format: yaml
  label: Nasuni Management Console (NMC) API
  slug: nasuni-management-console-nmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-nmc-v1-2-openapi.yml
- filename: nasuni-portal-v0-openapi.yml
  format: yaml
  label: Nasuni Portal API
  slug: nasuni-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-portal-v0-openapi.yml
- filename: nasuni-global-file-acceleration-telemetry-openapi.yml
  format: yaml
  label: Global File Acceleration (GFA) Telemetry API
  slug: global-file-acceleration-gfa-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-global-file-acceleration-telemetry-openapi.yml
- filename: nasuni-nasuni-data-service-azure-openapi.yml
  format: yaml
  label: Nasuni Data Service (NDS) for Azure API
  slug: nasuni-data-service-nds-for-azure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-nasuni-data-service-azure-openapi.yml
- filename: nasuni-nasuni-data-service-aws-openapi.yml
  format: yaml
  label: Nasuni Data Service (NDS) for AWS API
  slug: nasuni-data-service-nds-for-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/openapi/nasuni-nasuni-data-service-aws-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.api.nasuni.com/api/portal/v0/introduction/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Nasuni Scopes
name_suffix: OAuth Scopes
note: 'The Portal API declares an OAuth 2.0 clientCredentials flow but publishes an EMPTY scopes map, and no operation carries a scope requirement. Authorization is not scope-based: it is role-based and resolved server-side from the caller''s Portal IAM role. The permission vocabulary is retrievable at runtime — GET /iam/permissions lists every permission in the system, GET /iam/roles/{role_id}/permissions the set attached to a role, and GET /iam/me the caller''s own — but Nasuni publishes no static scope or permission reference page, so there is nothing to search for and enrich. scope_count is a real zero, not a gap in this harvest.'
overview: 'Nasuni uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nasuni
provider_slug: nasuni
schemes:
- description: Standard OAuth2 Client Credentials flow (RFC 6749 §4.4). Send `client_id` (service key) and `client_secret` (service secret) as form-encoded body parameters to the token endpoint.
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: OAuth2ClientCredentials
  source: openapi/nasuni-portal-v0-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: nasuni-scopes
source_filename: nasuni-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/nasuni-portal-v0-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/nasuni-portal-v0-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: Standard OAuth2 Client Credentials flow (RFC 6749 §4.4). Send `client_id` (service key) and `client_secret`\n    (service secret) as form-encoded body parameters to the token endpoint.\nscopes: []\nname: Nasuni Portal API OAuth scopes\ndocs: https://docs.api.nasuni.com/api/portal/v0/introduction/\nnote: 'The Portal API declares an OAuth 2.0 clientCredentials flow but publishes an EMPTY scopes map, and no operation\n  carries a scope requirement. Authorization is not scope-based: it is role-based and resolved server-side from\n  the caller''s Portal IAM role. The permission vocabulary is retrievable at runtime — GET /iam/permissions lists\n  every permission in the system, GET /iam/roles/{role_id}/permissions the set attached\
  \ to a role, and GET /iam/me\n  the caller''s own — but Nasuni publishes no static scope or permission reference page, so there is nothing to\n  search for and enrich. scope_count is a real zero, not a gap in this harvest.'\nauthorization_model: role-based (Portal IAM), not scope-based\nruntime_permission_endpoints:\n- GET /iam/permissions\n- GET /iam/roles\n- GET /iam/roles/{role_id}/permissions\n- GET /iam/me\nscope_count: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasuni/refs/heads/main/scopes/nasuni-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- File Storage
- Hybrid Cloud
- Object Storage
- Enterprise Storage
- Data Management
- Backup and Recovery
- Ransomware Protection
- Infrastructure
- Observability
- MCP
- agent-native
token_urls:
- /auth/token
---
