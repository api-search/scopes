---
api_specs:
- filename: simplivity-backups-api-openapi.yml
  format: yaml
  label: SimpliVity backups API
  slug: simplivity-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-backups-api-openapi.yml
- filename: simplivity-cluster-groups-api-openapi.yml
  format: yaml
  label: SimpliVity cluster_groups API
  slug: simplivity-cluster-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-cluster-groups-api-openapi.yml
- filename: simplivity-datastores-api-openapi.yml
  format: yaml
  label: SimpliVity datastores API
  slug: simplivity-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-datastores-api-openapi.yml
- filename: simplivity-external-stores-api-openapi.yml
  format: yaml
  label: SimpliVity external_stores API
  slug: simplivity-external-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-external-stores-api-openapi.yml
- filename: simplivity-hosts-api-openapi.yml
  format: yaml
  label: SimpliVity hosts API
  slug: simplivity-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-hosts-api-openapi.yml
- filename: simplivity-omnistack-clusters-api-openapi.yml
  format: yaml
  label: SimpliVity omnistack_clusters API
  slug: simplivity-omnistack-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-omnistack-clusters-api-openapi.yml
- filename: simplivity-policies-api-openapi.yml
  format: yaml
  label: SimpliVity policies API
  slug: simplivity-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-policies-api-openapi.yml
- filename: simplivity-security-api-openapi.yml
  format: yaml
  label: SimpliVity security API
  slug: simplivity-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-security-api-openapi.yml
- filename: simplivity-tasks-api-openapi.yml
  format: yaml
  label: SimpliVity tasks API
  slug: simplivity-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-tasks-api-openapi.yml
- filename: simplivity-virtual-machines-api-openapi.yml
  format: yaml
  label: SimpliVity virtual_machines API
  slug: simplivity-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-virtual-machines-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Simplivity Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SimpliVity publishes 2 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SimpliVity API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SimpliVity
provider_slug: simplivity
schemes:
- flows:
  - flow: password
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/simplivity-omnistack-openapi-original.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Grants read access
  flows:
  - password
  scope: read
- description: Grants write access
  flows:
  - password
  scope: write
slug: simplivity-scopes
source_filename: simplivity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/simplivity-omnistack-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/simplivity-omnistack-openapi-original.json\n  flows:\n  - flow: password\n    tokenUrl: /oauth/token\nscopes:\n- scope: read\n  description: Grants read access\n  flows:\n  - password\n  sources:\n  - openapi/simplivity-omnistack-openapi-original.json\n- scope: write\n  description: Grants write access\n  flows:\n  - password\n  sources:\n  - openapi/simplivity-omnistack-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/scopes/simplivity-scopes.yml
summary_line: 2 scopes · password
tags:
- Company
- Big Data
- Hyperconverged Infrastructure
- Virtualization
- Backup
- Disaster Recovery
- Data-Center
- Storage
- Cloud Infrastructure
- HPE
token_urls:
- /oauth/token
---
