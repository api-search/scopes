---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kaggle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kaggle publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kaggle API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kaggle
provider_slug: kaggle
schemes: []
scope_count: 1
scope_names:
- resources.admin:*
scopes:
- description: Only scope advertised in scopes_supported by the Kaggle authorization server and the MCP protected-resource document
  flows: []
  scope: resources.admin:*
slug: kaggle-scopes
source_filename: kaggle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Kaggle OAuth scopes\ngenerated: '2026-11-11'\nmethod: probed\nsource: https://www.kaggle.com/.well-known/oauth-authorization-server\nscopes:\n- name: resources.admin:*\n  description: Only scope advertised in scopes_supported by the Kaggle authorization\n    server and the MCP protected-resource document\n"
source_yaml_url: https://artifacts.apis.io/kaggle/scopes/kaggle-scopes.yml
summary_line: 1 scope
tags:
- CLI
- Competitions
- Data Science
- Datasets
- MCP
- Machine Learning
- Open Data
- Public APIs
token_bound: false
token_urls: []
---
