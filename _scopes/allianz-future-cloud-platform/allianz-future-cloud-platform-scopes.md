---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Allianz Future Cloud Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allianz Future Cloud Platform publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allianz Future Cloud Platform API on a user''s behalf.


  Tokens are issued from https://platform.allianz.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schemes:
- description: OAuth2 for Allianz internal platform API access
  flows:
  - flow: clientCredentials
    tokenUrl: https://platform.allianz.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-future-cloud-platform-services.yaml
scope_count: 6
scope_names:
- deployments:read
- deployments:write
- infrastructure:write
- observability:read
- services:read
- services:write
scopes:
- description: Read deployment history
  flows:
  - clientCredentials
  scope: deployments:read
- description: Trigger deployments
  flows:
  - clientCredentials
  scope: deployments:write
- description: Provision infrastructure resources
  flows:
  - clientCredentials
  scope: infrastructure:write
- description: Access platform metrics
  flows:
  - clientCredentials
  scope: observability:read
- description: Read service definitions
  flows:
  - clientCredentials
  scope: services:read
- description: Register and manage services
  flows:
  - clientCredentials
  scope: services:write
slug: allianz-future-cloud-platform-scopes
source_filename: allianz-future-cloud-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-future-cloud-platform-services.yaml\nschemes:\n- name: OAuth2\n  source: openapi/allianz-future-cloud-platform-services.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://platform.allianz.com/oauth2/token\n  description: OAuth2 for Allianz internal platform API access\nscopes:\n- scope: deployments:read\n  description: Read deployment history\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-future-cloud-platform-services.yaml\n- scope: deployments:write\n  description: Trigger deployments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-future-cloud-platform-services.yaml\n- scope: infrastructure:write\n  description: Provision infrastructure resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-future-cloud-platform-services.yaml\n- scope: observability:read\n  description: Access platform metrics\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/allianz-future-cloud-platform-services.yaml\n- scope: services:read\n  description: Read service definitions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-future-cloud-platform-services.yaml\n- scope: services:write\n  description: Register and manage services\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-future-cloud-platform-services.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/scopes/allianz-future-cloud-platform-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
token_urls:
- https://platform.allianz.com/oauth2/token
---
