---
api_specs:
- filename: luminance-accounts-api-openapi.yml
  format: yaml
  label: Luminance Accounts API
  slug: luminance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-accounts-api-openapi.yml
- filename: luminance-annotation-source-relations-api-openapi.yml
  format: yaml
  label: Luminance Annotation Source Relations API
  slug: luminance-annotation-source-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotation-source-relations-api-openapi.yml
- filename: luminance-annotation-sources-api-openapi.yml
  format: yaml
  label: Luminance Annotation Sources API
  slug: luminance-annotation-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotation-sources-api-openapi.yml
- filename: luminance-annotation-types-api-openapi.yml
  format: yaml
  label: Luminance Annotation Types API
  slug: luminance-annotation-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotation-types-api-openapi.yml
- filename: luminance-annotations-api-openapi.yml
  format: yaml
  label: Luminance Annotations API
  slug: luminance-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotations-api-openapi.yml
- filename: luminance-contract-creation-api-openapi.yml
  format: yaml
  label: Luminance Contract Creation API
  slug: luminance-contract-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-contract-creation-api-openapi.yml
- filename: luminance-document-templates-api-openapi.yml
  format: yaml
  label: Luminance Document Templates API
  slug: luminance-document-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-document-templates-api-openapi.yml
- filename: luminance-documents-api-openapi.yml
  format: yaml
  label: Luminance Documents API
  slug: luminance-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-documents-api-openapi.yml
- filename: luminance-folders-api-openapi.yml
  format: yaml
  label: Luminance Folders API
  slug: luminance-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-folders-api-openapi.yml
- filename: luminance-matter-versions-api-openapi.yml
  format: yaml
  label: Luminance Matter Versions API
  slug: luminance-matter-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-matter-versions-api-openapi.yml
- filename: luminance-matters-api-openapi.yml
  format: yaml
  label: Luminance Matters API
  slug: luminance-matters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-matters-api-openapi.yml
- filename: luminance-project-users-api-openapi.yml
  format: yaml
  label: Luminance Project Users API
  slug: luminance-project-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-project-users-api-openapi.yml
- filename: luminance-projects-api-openapi.yml
  format: yaml
  label: Luminance Projects API
  slug: luminance-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-projects-api-openapi.yml
- filename: luminance-reviews-api-openapi.yml
  format: yaml
  label: Luminance Reviews API
  slug: luminance-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-reviews-api-openapi.yml
- filename: luminance-root-api-openapi.yml
  format: yaml
  label: Luminance Root API
  slug: luminance-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-root-api-openapi.yml
- filename: luminance-search-api-openapi.yml
  format: yaml
  label: Luminance Search API
  slug: luminance-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-search-api-openapi.yml
- filename: luminance-system-api-openapi.yml
  format: yaml
  label: Luminance System API
  slug: luminance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-system-api-openapi.yml
- filename: luminance-tasks-api-openapi.yml
  format: yaml
  label: Luminance Tasks API
  slug: luminance-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-tasks-api-openapi.yml
- filename: luminance-traffic-light-analysis-api-openapi.yml
  format: yaml
  label: Luminance Traffic Light Analysis API
  slug: luminance-traffic-light-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-traffic-light-analysis-api-openapi.yml
- filename: luminance-users-api-openapi.yml
  format: yaml
  label: Luminance Users API
  slug: luminance-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-users-api-openapi.yml
- filename: luminance-workflows-api-openapi.yml
  format: yaml
  label: Luminance Workflows API
  slug: luminance-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Luminance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Luminance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://moniker.app.luminance.com/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Luminance
provider_slug: luminance
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://moniker.app.luminance.com/auth/oauth2/token
  name: OAuth2
  source: openapi/luminance-api-v1-3-openapi-original.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://moniker.app.luminance.com/auth/oauth2/token
  name: OAuth2
  source: openapi/luminance-api-v1-4-openapi-original.yml
scope_count: 0
scope_names: []
scopes: []
slug: luminance-scopes
source_filename: luminance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/luminance-api-v1-3-openapi-original.yml, openapi/luminance-api-v1-4-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/luminance-api-v1-3-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://moniker.app.luminance.com/auth/oauth2/token\n- name: OAuth2\n  source: openapi/luminance-api-v1-4-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://moniker.app.luminance.com/auth/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/scopes/luminance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Legal
- Artificial Intelligence
- Contracts
- Contract Lifecycle Management
- Document Intelligence
- Compliance
- Legal Technology
- Enterprise Software
- Automation
token_urls:
- https://moniker.app.luminance.com/auth/oauth2/token
---
