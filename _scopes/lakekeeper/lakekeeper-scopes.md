---
api_specs:
- filename: lakekeeper-generic-table-api-openapi.yml
  format: yaml
  label: Lakekeeper Generic Table (Data) API
  slug: lakekeeper-generic-table-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-generic-table-api-openapi.yml
- filename: lakekeeper-authorization-api-openapi.yml
  format: yaml
  label: Lakekeeper Authorization API
  slug: lakekeeper-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-authorization-api-openapi.yml
- filename: lakekeeper-catalog-api-api-openapi.yml
  format: yaml
  label: Lakekeeper Catalog API
  slug: lakekeeper-catalog-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-catalog-api-api-openapi.yml
- filename: lakekeeper-configuration-api-api-openapi.yml
  format: yaml
  label: Lakekeeper Configuration API
  slug: lakekeeper-configuration-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-configuration-api-api-openapi.yml
- filename: lakekeeper-oauth2-api-api-openapi.yml
  format: yaml
  label: Lakekeeper OAuth2 API
  slug: lakekeeper-oauth2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-oauth2-api-api-openapi.yml
- filename: lakekeeper-permissions-cedar-api-openapi.yml
  format: yaml
  label: Lakekeeper Permissions Cedar API
  slug: lakekeeper-permissions-cedar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-permissions-cedar-api-openapi.yml
- filename: lakekeeper-permissions-openfga-api-openapi.yml
  format: yaml
  label: Lakekeeper Permissions Openfga API
  slug: lakekeeper-permissions-openfga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-permissions-openfga-api-openapi.yml
- filename: lakekeeper-project-api-openapi.yml
  format: yaml
  label: Lakekeeper Project API
  slug: lakekeeper-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-project-api-openapi.yml
- filename: lakekeeper-role-api-openapi.yml
  format: yaml
  label: Lakekeeper Role API
  slug: lakekeeper-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-role-api-openapi.yml
- filename: lakekeeper-server-api-openapi.yml
  format: yaml
  label: Lakekeeper Server API
  slug: lakekeeper-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-server-api-openapi.yml
- filename: lakekeeper-tasks-api-openapi.yml
  format: yaml
  label: Lakekeeper Tasks API
  slug: lakekeeper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-tasks-api-openapi.yml
- filename: lakekeeper-user-api-openapi.yml
  format: yaml
  label: Lakekeeper User API
  slug: lakekeeper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-user-api-openapi.yml
- filename: lakekeeper-warehouse-api-openapi.yml
  format: yaml
  label: Lakekeeper Warehouse API
  slug: lakekeeper-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-warehouse-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lakekeeper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lakekeeper publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lakekeeper API on a user''s behalf.


  Tokens are issued from /v1/oauth/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lakekeeper
provider_slug: lakekeeper
schemes:
- description: 'This scheme is used for OAuth2 authorization.


    For unauthorized requests, services should return an appropriate 401 or 403 response. Implementations must not return altered success (200) responses when a request is unauthenticated or unauthorized.

    If a separate authorization server is used, substitute the tokenUrl with the full token path of the external authorization server, and use the resulting token to access the resources defined in the spec.'
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth/tokens
  name: OAuth2
  source: openapi/lakekeeper-catalog-api-openapi.yml
scope_count: 1
scope_names:
- catalog
scopes:
- description: Allows interacting with the Config and Catalog APIs
  flows:
  - clientCredentials
  scope: catalog
slug: lakekeeper-scopes
source_filename: lakekeeper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: derived\nsource: openapi/lakekeeper-catalog-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lakekeeper-catalog-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/tokens\n  description: |-\n    This scheme is used for OAuth2 authorization.\n\n    For unauthorized requests, services should return an appropriate 401 or 403 response. Implementations must not return altered success (200) responses when a request is unauthenticated or unauthorized.\n    If a separate authorization server is used, substitute the tokenUrl with the full token path of the external authorization server, and use the resulting token to access the resources defined in the spec.\nscopes:\n- scope: catalog\n  description: Allows interacting with the Config and Catalog APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lakekeeper-catalog-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/scopes/lakekeeper-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Apache Iceberg
- Data Catalog
- Lakehouse
- Open Source
- Rust
- Data Governance
- Access Control
- Object Storage
- Metadata
- Self-Hosted
- OpenFGA
- Data Engineering
token_urls:
- /v1/oauth/tokens
---
