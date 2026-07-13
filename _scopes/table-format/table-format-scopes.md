---
api_specs:
- filename: rest-catalog-open-api.yaml
  format: yaml
  label: Apache Iceberg REST Catalog API
  slug: apache-iceberg-rest-catalog
  spec_type: OpenAPI
  url: https://github.com/apache/iceberg/blob/main/open-api/rest-catalog-open-api.yaml
- filename: all.yaml
  format: yaml
  label: Unity Catalog
  slug: unity-catalog
  spec_type: OpenAPI
  url: https://github.com/unitycatalog/unitycatalog/blob/main/api/all.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Table Format Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Table Format publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Table Format API on a user''s behalf.


  Tokens are issued from /v1/oauth/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Table Format
provider_slug: table-format
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth/tokens
  name: OAuth2
  source: openapi/apache-iceberg-rest-catalog-openapi.yml
scope_count: 1
scope_names:
- catalog
scopes:
- description: Access catalog operations
  flows:
  - clientCredentials
  scope: catalog
slug: table-format-scopes
source_filename: table-format-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-iceberg-rest-catalog-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/apache-iceberg-rest-catalog-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/tokens\nscopes:\n- scope: catalog\n  description: Access catalog operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apache-iceberg-rest-catalog-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/table-format/refs/heads/main/scopes/table-format-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Data Lakehouse
- Open Table Format
- Apache Iceberg
- Delta Lake
- Apache Hudi
- Data Lake
- ACID Transactions
- Schema Evolution
- Time Travel
token_urls:
- /v1/oauth/tokens
---
