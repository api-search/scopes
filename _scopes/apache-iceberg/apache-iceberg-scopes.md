---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Apache Iceberg Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apache Iceberg publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apache Iceberg API on a user''s behalf.


  Tokens are issued from /v1/oauth/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schemes:
- description: 'This scheme is used for OAuth2 authorization.


    For unauthorized requests, services should return an appropriate 401 or 403 response. Implementations must not return altered success (200) responses when a request is unauthenticated or unauthorized.

    If a separate authorization server is used, substitute the tokenUrl with the full token path of the external authorization server, and use the resulting token to access the resources defined in the spec.'
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth/tokens
  name: OAuth2
  source: openapi/apache-iceberg-rest-catalog-open-api.yaml
scope_count: 1
scope_names:
- catalog
scopes:
- description: Allows interacting with the Config and Catalog APIs
  flows:
  - clientCredentials
  scope: catalog
slug: apache-iceberg-scopes
source_filename: apache-iceberg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apache-iceberg-rest-catalog-open-api.yaml\nschemes:\n- name: OAuth2\n  source: openapi/apache-iceberg-rest-catalog-open-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/tokens\n  description: |-\n    This scheme is used for OAuth2 authorization.\n\n    For unauthorized requests, services should return an appropriate 401 or 403 response. Implementations must not return altered success (200) responses when a request is unauthenticated or unauthorized.\n    If a separate authorization server is used, substitute the tokenUrl with the full token path of the external authorization server, and use the resulting token to access the resources defined in the spec.\nscopes:\n- scope: catalog\n  description: Allows interacting with the Config and Catalog APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apache-iceberg-rest-catalog-open-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/scopes/apache-iceberg-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
token_urls:
- /v1/oauth/tokens
---
