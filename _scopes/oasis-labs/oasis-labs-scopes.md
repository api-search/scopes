---
authorization_urls: []
description: ''
docs: https://docs.oasislabs.com/parcel/latest
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Oasis Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oasis Labs publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Oasis Labs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oasis Labs
provider_slug: oasis-labs
schemes:
- audience: https://api.oasislabs.com/parcel
  flow: clientCredentials
  name: OAuth2ClientCredentials
  tokenUrl: https://auth.oasislabs.com/oauth/token
scope_count: 7
scope_names:
- parcel.full
- parcel.identity.*
- parcel.dataset.*
- parcel.app.*
- parcel.grant.*
- parcel.permission.*
- parcel.job.*
scopes:
- description: Full access to all Parcel resources and actions (default scope).
  flows: []
  scope: parcel.full
- description: Manage identities (create/read/update/delete).
  flows: []
  scope: parcel.identity.*
- description: Manage datasets — upload, read metadata, update, delete tokenized data.
  flows: []
  scope: parcel.dataset.*
- description: Manage Parcel apps and their configuration.
  flows: []
  scope: parcel.app.*
- description: Manage access grants that govern who can compute over which data.
  flows: []
  scope: parcel.grant.*
- description: Manage permissions attached to apps and grants.
  flows: []
  scope: parcel.permission.*
- description: Manage confidential compute jobs.
  flows: []
  scope: parcel.job.*
slug: oasis-labs-scopes
source_filename: oasis-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  github.com/oasislabs/parcel-clients typescript/src/token.ts (Scope type\n  definition) — parcel.full | parcel.<resource>.<action>\ndocs: https://docs.oasislabs.com/parcel/latest\nschemes:\n- name: OAuth2ClientCredentials\n  flow: clientCredentials\n  tokenUrl: https://auth.oasislabs.com/oauth/token\n  audience: https://api.oasislabs.com/parcel\nscope_grammar: \"parcel.<resource>.<action>\"\nresources:\n- identity\n- dataset\n- app\n- grant\n- permission\n- job\nactions:\n- create\n- read\n- update\n- delete\nscopes:\n- scope: parcel.full\n  description: Full access to all Parcel resources and actions (default scope).\n- scope: \"parcel.identity.*\"\n  description: Manage identities (create/read/update/delete).\n- scope: \"parcel.dataset.*\"\n  description: Manage datasets — upload, read metadata, update, delete tokenized data.\n- scope: \"parcel.app.*\"\n  description: Manage Parcel apps and their configuration.\n- scope:\
  \ \"parcel.grant.*\"\n  description: Manage access grants that govern who can compute over which data.\n- scope: \"parcel.permission.*\"\n  description: Manage permissions attached to apps and grants.\n- scope: \"parcel.job.*\"\n  description: Manage confidential compute jobs.\nnotes: >-\n  Scopes follow the pattern parcel.<resource>.<action> where <resource> is one of\n  identity, dataset, app, grant, permission, job (or *) and <action> is one of\n  create, read, update, delete (or *). parcel.full grants everything. The wildcard\n  entries above enumerate the per-resource families; concrete tokens combine a\n  single resource with a single action (e.g. parcel.dataset.read).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oasis-labs/refs/heads/main/scopes/oasis-labs-scopes.yml
summary_line: 7 scopes
tags:
- Company
- Privacy
- Data Governance
- Confidential Computing
- Blockchain
- Differential Privacy
- Machine Learning
- Developer Platform
- Web3
token_urls: []
---
