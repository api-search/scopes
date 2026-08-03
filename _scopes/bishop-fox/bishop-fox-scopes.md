---
authorization_urls: []
description: ''
docs: https://docs.brinqa.com/docs/connectors/bishopfox/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Bishop Fox Scopes
name_suffix: OAuth Scopes
note: Bishop Fox publishes no public scope reference — the Cosmos API documentation lives inside the authenticated portal. The scope set below is the one granted to a Cosmos API key/secret pair as documented by Brinqa's published Cosmos connector documentation, which records the scopes returned on the client-credentials token for the cosmos_public audience. Not derived from an OpenAPI (none is published) and not exhaustive — a Cosmos customer with portal access should confirm against the in-portal reference.
overview: 'Bishop Fox publishes 7 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bishop Fox API on a user''s behalf.


  Tokens are issued from https://bishopfox.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bishop Fox
provider_slug: bishop-fox
schemes:
- audience: cosmos_public
  flows:
  - flow: clientCredentials
    tokenUrl: https://bishopfox.auth0.com/oauth/token
  name: CosmosOAuth2ClientCredentials
  source: https://bishopfox.auth0.com/.well-known/openid-configuration
  type: oauth2
scope_count: 7
scope_names:
- get:assets
- list:assets
- update:assets
- get:findings
- update:findings
- read:ingest
- write:ingest
scopes:
- description: Read individual discovered attack-surface assets.
  flows:
  - clientCredentials
  scope: get:assets
- description: List/enumerate discovered attack-surface assets across the asset-view resources.
  flows:
  - clientCredentials
  scope: list:assets
- description: Update asset records (e.g. attribution, ownership, or state changes).
  flows:
  - clientCredentials
  scope: update:assets
- description: Read validated Cosmos findings and finding definitions.
  flows:
  - clientCredentials
  scope: get:findings
- description: Update findings (e.g. triage state, comments, remediation status).
  flows:
  - clientCredentials
  scope: update:findings
- description: Read ingestion configuration/state for customer-supplied seed data.
  flows:
  - clientCredentials
  scope: read:ingest
- description: Submit seed data into the Cosmos ingestion pipeline.
  flows:
  - clientCredentials
  scope: write:ingest
slug: bishop-fox-scopes
source_filename: bishop-fox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.brinqa.com/docs/connectors/bishopfox/\ndocs: https://docs.brinqa.com/docs/connectors/bishopfox/\nnote: >-\n  Bishop Fox publishes no public scope reference — the Cosmos API documentation lives inside the\n  authenticated portal. The scope set below is the one granted to a Cosmos API key/secret pair as documented\n  by Brinqa's published Cosmos connector documentation, which records the scopes returned on the\n  client-credentials token for the cosmos_public audience. Not derived from an OpenAPI (none is published)\n  and not exhaustive — a Cosmos customer with portal access should confirm against the in-portal reference.\nschemes:\n- name: CosmosOAuth2ClientCredentials\n  type: oauth2\n  source: https://bishopfox.auth0.com/.well-known/openid-configuration\n  audience: cosmos_public\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bishopfox.auth0.com/oauth/token\nscopes:\n- scope: get:assets\n  description:\
  \ Read individual discovered attack-surface assets.\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\n- scope: list:assets\n  description: List/enumerate discovered attack-surface assets across the asset-view resources.\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\n- scope: update:assets\n  description: Update asset records (e.g. attribution, ownership, or state changes).\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\n- scope: get:findings\n  description: Read validated Cosmos findings and finding definitions.\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\n- scope: update:findings\n  description: Update findings (e.g. triage state, comments, remediation status).\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\n- scope: read:ingest\n  description: Read\
  \ ingestion configuration/state for customer-supplied seed data.\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\n- scope: write:ingest\n  description: Submit seed data into the Cosmos ingestion pipeline.\n  flows: [clientCredentials]\n  sources: [https://docs.brinqa.com/docs/connectors/bishopfox/]\nsummary:\n  scope_count: 7\n  pattern: verb:resource\n  verbs: [get, list, read, update, write]\n  resources: [assets, findings, ingest]\nx-evidence:\n- url: https://docs.brinqa.com/docs/connectors/bishopfox/\n  http_status: 200\n  fetched: '2026-08-02'\n  kind: third-party connector documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bishop-fox/refs/heads/main/scopes/bishop-fox-scopes.yml
summary_line: 7 scopes · clientCredentials
tags:
- Company
- cybersecurity
- offensive-security
- penetration-testing
- attack-surface-management
- exposure-management
- red-teaming
- vulnerability-management
- security-findings
- asset-discovery
- continuous-threat-exposure-management
- oauth2
token_urls:
- https://bishopfox.auth0.com/oauth/token
---
