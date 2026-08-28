---
api_specs:
- filename: lakekeeper-management-api-openapi.yml
  format: yaml
  label: Lakekeeper Management API
  slug: lakekeeper-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-management-api-openapi.yml
- filename: lakekeeper-catalog-api-openapi.yml
  format: yaml
  label: Lakekeeper Iceberg REST Catalog API
  slug: lakekeeper-iceberg-rest-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-catalog-api-openapi.yml
- filename: lakekeeper-generic-table-api-openapi.yml
  format: yaml
  label: Lakekeeper Generic Table (Data) API
  slug: lakekeeper-generic-table-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-generic-table-api-openapi.yml
- filename: lakekeeper-management-plus-api-openapi.yml
  format: yaml
  label: Lakekeeper+ Management API
  slug: lakekeeper-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-management-plus-api-openapi.yml
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
