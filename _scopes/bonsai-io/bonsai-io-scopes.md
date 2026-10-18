---
api_specs:
- filename: bonsai-io-clusters-api-openapi.yml
  format: yaml
  label: Bonsai Clusters API
  slug: bonsai-io-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-clusters-api-openapi.yml
- filename: bonsai-io-plans-api-openapi.yml
  format: yaml
  label: Bonsai Plans API
  slug: bonsai-io-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-plans-api-openapi.yml
- filename: bonsai-io-releases-api-openapi.yml
  format: yaml
  label: Bonsai Releases API
  slug: bonsai-io-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-releases-api-openapi.yml
- filename: bonsai-io-spaces-api-openapi.yml
  format: yaml
  label: Bonsai Spaces API
  slug: bonsai-io-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/openapi/bonsai-io-spaces-api-openapi.yml
authorization_urls: []
description: ''
docs: https://bonsai.io/docs/account/api-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bonsai Io Scopes
name_suffix: OAuth Scopes
note: 'A new token is read-only by default: account:read and clusters:read are checked, and clusters:write is not. Bonsai tokens are scoped API tokens, not OAuth 2.0.'
overview: 'Bonsai publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bonsai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bonsai
provider_slug: bonsai-io
schemes: []
scope_count: 3
scope_names:
- account:read
- clusters:read
- clusters:write
scopes:
- description: List and read the plans, spaces and releases available to the account (the Plans , Spaces and Releases APIs).
  flows: []
  scope: account:read
- description: List and read the account's clusters.
  flows: []
  scope: clusters:read
- description: Create, update and delete clusters.
  flows: []
  scope: clusters:write
slug: bonsai-io-scopes
source_filename: bonsai-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Bonsai API Token Scopes\ngenerated: '2026-10-14'\nmethod: searched\nsource: https://bonsai.io/docs/account/api-tokens\ndocs: https://bonsai.io/docs/account/api-tokens\nscopes:\n- name: account:read\n  description: List and read the plans, spaces and releases available to the account (the Plans , Spaces and Releases APIs).\n  operations:\n  - listPlans\n  - getPlan\n  - listReleases\n  - getRelease\n  - listSpaces\n  - getSpace\n- name: clusters:read\n  description: List and read the account's clusters.\n  operations:\n  - listClusters\n  - getCluster\n- name: clusters:write\n  description: Create, update and delete clusters.\n  operations:\n  - createCluster\n  - updateCluster\n  - deleteCluster\nnote: 'A new token is read-only by default: account:read and clusters:read are checked, and clusters:write is not. Bonsai tokens are scoped API tokens, not OAuth 2.0.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonsai-io/refs/heads/main/scopes/bonsai-io-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Search
- Elasticsearch
- OpenSearch
- Managed Service
- Vector Search
- Cloud Infrastructure
token_bound: false
token_urls: []
---
