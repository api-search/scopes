---
authorization_urls: []
description: ''
docs: https://www.workboard.com/developer
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: searched
name: Quantive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Quantive publishes 1 OAuth 2.0 scope via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Quantive API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Quantive
provider_slug: quantive
schemes: []
scope_count: 1
scope_names:
- all
scopes:
- description: Default scope value granting full access consistent with the authorizing user's permissions. Documented as the default value for the scope parameter in WorkBoard API v1.0.
  flows: []
  scope: all
slug: quantive-scopes
source_filename: quantive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: 2026-07-20\nmethod: searched\nsource: https://www.workboard.com/developer\napi: WorkBoard REST API (Quantive)\ndocs: https://www.workboard.com/developer\nflow: authorization_code\nnotes: >-\n  The WorkBoard REST API v1.0 documents a single coarse OAuth scope. No\n  fine-grained scope taxonomy is published, and no OpenAPI declares per-operation\n  scopes, so this is the complete documented set.\nscopes:\n- name: all\n  description: >-\n    Default scope value granting full access consistent with the authorizing\n    user's permissions. Documented as the default value for the scope parameter\n    in WorkBoard API v1.0.\n  default: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantive/refs/heads/main/scopes/quantive-scopes.yml
summary_line: 1 scope · authorization_code
tags:
- Company
- Business Applications
- OKRs
- Strategy Execution
- Goal Management
- Performance Management
- Software-as-a-Service
token_bound: false
token_urls: []
---
