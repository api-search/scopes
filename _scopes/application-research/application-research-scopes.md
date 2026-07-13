---
api_specs:
- filename: score-openapi.yml
  format: yaml
  label: Score Workload Specification API
  slug: score-workload-specification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/score-openapi.yml
- filename: cloud-native-application-bundle-openapi.yml
  format: yaml
  label: Cloud Native Application Bundle API
  slug: cloud-native-application-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/cloud-native-application-bundle-openapi.yml
- filename: open-component-model-openapi.yml
  format: yaml
  label: Open Component Model API
  slug: open-component-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/open-component-model-openapi.yml
- filename: open-resource-discovery-openapi.yml
  format: yaml
  label: Open Resource Discovery API
  slug: open-resource-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/open-resource-discovery-openapi.yml
- filename: radius-openapi.yml
  format: yaml
  label: Radius Application Platform API
  slug: radius-application-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/radius-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Application Research Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Application Research publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Application Research API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Application Research
provider_slug: application-research
schemes:
- description: OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: oauth2
  source: openapi/open-resource-discovery-openapi.yml
scope_count: 3
scope_names:
- ord:admin
- ord:read
- ord:write
scopes:
- description: Administrative access to ORD resources
  flows:
  - clientCredentials
  scope: ord:admin
- description: Read access to ORD resources
  flows:
  - clientCredentials
  scope: ord:read
- description: Write access to ORD resources
  flows:
  - clientCredentials
  scope: ord:write
slug: application-research-scopes
source_filename: application-research-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/open-resource-discovery-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/open-resource-discovery-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: OAuth 2.0 authentication\nscopes:\n- scope: ord:admin\n  description: Administrative access to ORD resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/open-resource-discovery-openapi.yml\n- scope: ord:read\n  description: Read access to ORD resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/open-resource-discovery-openapi.yml\n- scope: ord:write\n  description: Write access to ORD resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/open-resource-discovery-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/scopes/application-research-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Application Dependencies
- Cloud Native
- Integration
- Research
- Specifications
- Workload Specifications
token_urls:
- /oauth/token
---
