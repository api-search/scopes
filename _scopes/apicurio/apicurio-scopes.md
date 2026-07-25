---
api_specs:
- filename: apicurio-admin-api-openapi.yml
  format: yaml
  label: Apicurio Admin API
  slug: apicurio-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-admin-api-openapi.yml
- filename: apicurio-ai-api-openapi.yml
  format: yaml
  label: Apicurio AI API
  slug: apicurio-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-ai-api-openapi.yml
- filename: apicurio-artifact-rules-api-openapi.yml
  format: yaml
  label: Apicurio Artifact rules API
  slug: apicurio-artifact-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-artifact-rules-api-openapi.yml
- filename: apicurio-artifact-type-api-openapi.yml
  format: yaml
  label: Apicurio Artifact Type API
  slug: apicurio-artifact-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-artifact-type-api-openapi.yml
- filename: apicurio-artifacts-api-openapi.yml
  format: yaml
  label: Apicurio Artifacts API
  slug: apicurio-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-artifacts-api-openapi.yml
- filename: apicurio-branches-api-openapi.yml
  format: yaml
  label: Apicurio Branches API
  slug: apicurio-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-branches-api-openapi.yml
- filename: apicurio-content-api-openapi.yml
  format: yaml
  label: Apicurio Content API
  slug: apicurio-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-content-api-openapi.yml
- filename: apicurio-contracts-api-openapi.yml
  format: yaml
  label: Apicurio Contracts API
  slug: apicurio-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-contracts-api-openapi.yml
- filename: apicurio-gitops-api-openapi.yml
  format: yaml
  label: Apicurio GitOps API
  slug: apicurio-gitops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-gitops-api-openapi.yml
- filename: apicurio-global-rules-api-openapi.yml
  format: yaml
  label: Apicurio Global rules API
  slug: apicurio-global-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-global-rules-api-openapi.yml
- filename: apicurio-group-rules-api-openapi.yml
  format: yaml
  label: Apicurio Group rules API
  slug: apicurio-group-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-group-rules-api-openapi.yml
- filename: apicurio-groups-api-openapi.yml
  format: yaml
  label: Apicurio Groups API
  slug: apicurio-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-groups-api-openapi.yml
- filename: apicurio-kafkasql-api-openapi.yml
  format: yaml
  label: Apicurio KafkaSQL API
  slug: apicurio-kafkasql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-kafkasql-api-openapi.yml
- filename: apicurio-metadata-api-openapi.yml
  format: yaml
  label: Apicurio Metadata API
  slug: apicurio-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-metadata-api-openapi.yml
- filename: apicurio-search-api-openapi.yml
  format: yaml
  label: Apicurio Search API
  slug: apicurio-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-search-api-openapi.yml
- filename: apicurio-snapshot-api-openapi.yml
  format: yaml
  label: Apicurio Snapshot API
  slug: apicurio-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-snapshot-api-openapi.yml
- filename: apicurio-system-api-openapi.yml
  format: yaml
  label: Apicurio System API
  slug: apicurio-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-system-api-openapi.yml
- filename: apicurio-users-api-openapi.yml
  format: yaml
  label: Apicurio Users API
  slug: apicurio-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-users-api-openapi.yml
- filename: apicurio-versions-api-openapi.yml
  format: yaml
  label: Apicurio Versions API
  slug: apicurio-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/openapi/apicurio-versions-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Apicurio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apicurio publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apicurio API on a user''s behalf.


  Tokens are issued from https://example.com/realms/apicurio/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apicurio
provider_slug: apicurio
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token
  name: OAuth2
  source: openapi/apicurio-openapi.yml
scope_count: 3
scope_names:
- admin
- read
- write
scopes:
- description: Admin access
  flows:
  - clientCredentials
  scope: admin
- description: Read access
  flows:
  - clientCredentials
  scope: read
- description: Write access
  flows:
  - clientCredentials
  scope: write
slug: apicurio-scopes
source_filename: apicurio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicurio-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/apicurio-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token\nscopes:\n- scope: admin\n  description: Admin access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apicurio-openapi.yml\n- scope: read\n  description: Read access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apicurio-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/apicurio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/scopes/apicurio-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Apache License
- API Design
- API Registry
- Avro
- AsyncAPI
- Java
- Open Source
- OpenAPI
- Red Hat
- Schema Registry
token_urls:
- https://example.com/realms/apicurio/protocol/openid-connect/token
---
