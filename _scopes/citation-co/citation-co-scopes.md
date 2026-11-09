---
api_specs:
- filename: citation-co-balance-api-openapi.yml
  format: yaml
  label: Citation Balance API
  slug: citation-co-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-balance-api-openapi.yml
- filename: citation-co-checks-api-openapi.yml
  format: yaml
  label: Citation Checks API
  slug: citation-co-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-checks-api-openapi.yml
- filename: citation-co-documents-api-openapi.yml
  format: yaml
  label: Citation Documents API
  slug: citation-co-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-documents-api-openapi.yml
- filename: citation-co-events-api-openapi.yml
  format: yaml
  label: Citation Events API
  slug: citation-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-events-api-openapi.yml
- filename: citation-co-exports-api-openapi.yml
  format: yaml
  label: Citation Exports API
  slug: citation-co-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-exports-api-openapi.yml
- filename: citation-co-files-api-openapi.yml
  format: yaml
  label: Citation Files API
  slug: citation-co-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-files-api-openapi.yml
- filename: citation-co-imports-api-openapi.yml
  format: yaml
  label: Citation Imports API
  slug: citation-co-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-imports-api-openapi.yml
- filename: citation-co-jobs-api-openapi.yml
  format: yaml
  label: Citation Jobs API
  slug: citation-co-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-jobs-api-openapi.yml
- filename: citation-co-ledger-api-openapi.yml
  format: yaml
  label: Citation Ledger API
  slug: citation-co-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-ledger-api-openapi.yml
- filename: citation-co-me-api-openapi.yml
  format: yaml
  label: Citation Me API
  slug: citation-co-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-me-api-openapi.yml
- filename: citation-co-pricing-api-openapi.yml
  format: yaml
  label: Citation Pricing API
  slug: citation-co-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-pricing-api-openapi.yml
- filename: citation-co-sources-api-openapi.yml
  format: yaml
  label: Citation Sources API
  slug: citation-co-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-sources-api-openapi.yml
- filename: citation-co-webhooks-api-openapi.yml
  format: yaml
  label: Citation Webhooks API
  slug: citation-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-webhooks-api-openapi.yml
- filename: citation-co-write-api-openapi.yml
  format: yaml
  label: Citation Write API
  slug: citation-co-write-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/citation-co/openapi/citation-co-write-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Citation Co Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Citation publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Citation API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Citation
provider_slug: citation-co
schemes: []
scope_count: 13
scope_names:
- documents:read
- documents:write
- sources:read
- sources:write
- exports:read
- ai:write
- checks:write
- files:write
- sharing:read
- sharing:write
- comments:read
- comments:write
- webhooks:write
scopes:
- description: Read documents and history
  flows: []
  scope: documents:read
- description: Create, update, trash, restore and apply edits to documents
  flows: []
  scope: documents:write
- description: Read sources, resolve new sources and format references
  flows: []
  scope: sources:read
- description: Save and update source records
  flows: []
  scope: sources:write
- description: Export and download document files
  flows: []
  scope: exports:read
- description: Use the Write tools
  flows: []
  scope: ai:write
- description: Start Check and review findings
  flows: []
  scope: checks:write
- description: Upload and import files
  flows: []
  scope: files:write
- description: Read document access
  flows: []
  scope: sharing:read
- description: Manage document guests, invitations and public links
  flows: []
  scope: sharing:write
- description: Read comments
  flows: []
  scope: comments:read
- description: Add and resolve comments
  flows: []
  scope: comments:write
- description: Manage webhook subscriptions and deliveries
  flows: []
  scope: webhooks:write
slug: citation-co-scopes
source_filename: citation-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://citation.co/docs/api/markdown\nscopes:\n  - name: documents:read\n    description: Read documents and history\n  - name: documents:write\n    description: Create, update, trash, restore and apply edits to documents\n  - name: sources:read\n    description: Read sources, resolve new sources and format references\n  - name: sources:write\n    description: Save and update source records\n  - name: exports:read\n    description: Export and download document files\n  - name: ai:write\n    description: Use the Write tools\n  - name: checks:write\n    description: Start Check and review findings\n  - name: files:write\n    description: Upload and import files\n  - name: sharing:read\n    description: Read document access\n  - name: sharing:write\n    description: Manage document guests, invitations and public links\n  - name: comments:read\n    description: Read comments\n  - name: comments:write\n    description: Add and\
  \ resolve comments\n  - name: webhooks:write\n    description: Manage webhook subscriptions and deliveries\n"
source_yaml_url: https://artifacts.apis.io/citation-co/scopes/citation-co-scopes.yml
summary_line: 13 scopes
tags:
- Citations
- Bibliography
- WritingTool
- Academic
- Productivity
token_bound: false
token_urls: []
---
