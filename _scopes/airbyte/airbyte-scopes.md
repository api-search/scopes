---
api_specs:
- filename: airbyte-openapi.yml
  format: yaml
  label: Airbyte
  slug: airbyte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/openapi/airbyte-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.airbyte.com/platform/using-airbyte/configuring-api-access
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Airbyte Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Airbyte publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Airbyte API on a user''s behalf.


  Tokens are issued from https://api.airbyte.com/v1/applications/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Airbyte
provider_slug: airbyte
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.airbyte.com/v1/applications/token
  name: clientCredentials
  source: https://airbyte.com/.well-known/openid-configuration
scope_count: 2
scope_names:
- openid
- api
scopes:
- description: Standard OpenID Connect scope; returned in the client_credentials token.
  flows:
  - clientCredentials
  scope: openid
- description: Grants access to the Airbyte public API. Effective authorization is bound to the permissions of the user that owns the Application (workspace/organization RBAC), not to fine-grained OAuth scopes.
  flows:
  - clientCredentials
  scope: api
slug: airbyte-scopes
source_filename: airbyte-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://airbyte.com/.well-known/openid-configuration\ndocs: https://docs.airbyte.com/platform/using-airbyte/configuring-api-access\nschemes:\n- name: clientCredentials\n  source: https://airbyte.com/.well-known/openid-configuration\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.airbyte.com/v1/applications/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; returned in the client_credentials token.\n  flows: [clientCredentials]\n  sources: [https://airbyte.com/.well-known/openid-configuration]\n- scope: api\n  description: >-\n    Grants access to the Airbyte public API. Effective authorization is bound to\n    the permissions of the user that owns the Application (workspace/organization\n    RBAC), not to fine-grained OAuth scopes.\n  flows: [clientCredentials]\n  sources: [https://airbyte.com/.well-known/openid-configuration]\nnotes: >-\n  Airbyte exposes only the coarse OIDC scopes\
  \ 'openid' and 'api'. Access is\n  governed by workspace/organization RBAC roles attached to the Application's\n  owning user rather than by granular API scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/scopes/airbyte-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
token_urls:
- https://api.airbyte.com/v1/applications/token
---
