---
api_specs:
- filename: contensis-content-types-api-openapi.yml
  format: yaml
  label: Contensis Content Types API
  slug: contensis-content-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-content-types-api-openapi.yml
- filename: contensis-entries-api-openapi.yml
  format: yaml
  label: Contensis Entries API
  slug: contensis-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-entries-api-openapi.yml
- filename: contensis-projects-api-openapi.yml
  format: yaml
  label: Contensis Projects API
  slug: contensis-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-projects-api-openapi.yml
- filename: contensis-taxonomy-api-openapi.yml
  format: yaml
  label: Contensis Taxonomy API
  slug: contensis-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-taxonomy-api-openapi.yml
authorization_urls: []
description: OAuth 2.0 scopes for the Contensis Management API. They are passed as a space-separated list in the `scope` parameter of a client_credentials token request against the per-tenant token endpoint. The published table is short — four named scopes covering projects and entries — and one further scope, ContentType_Read, appears in the docs' own worked example without appearing in the table.
docs: https://www.contensis.com/help-and-docs/apis/management-http/security/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Contensis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Contensis uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Contensis
provider_slug: contensis
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: contensis-scopes
source_filename: contensis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Contensis\nproviderId: contensis\ngenerated: '2026-09-06'\nmethod: searched\ndocs: https://www.contensis.com/help-and-docs/apis/management-http/security/scopes\nsource: >-\n  The published scopes reference for the Contensis HTTP Management API (page last updated\n  24 September 2024), cross-read against the provider's markdown mirror at\n  https://github.com/contensis/contensis-docs. The captured OpenAPI declares no\n  securitySchemes, so derive-oauth-scopes.py found nothing — every scope below is read\n  from the provider's own documentation.\ndescription: >-\n  OAuth 2.0 scopes for the Contensis Management API. They are passed as a space-separated\n  list in the `scope` parameter of a client_credentials token request against the\n  per-tenant token endpoint. The published table is short — four named scopes covering\n  projects and entries — and one further scope, ContentType_Read, appears in the\
  \ docs' own\n  worked example without appearing in the table.\nflow: clientCredentials\ntoken_endpoint: https://cms-{alias}.cloud.contensis.com/authenticate/connect/token\nseparator: space\nscopes:\n  - name: Project_Read\n    documented: true\n    description: Read a project.\n    operations:\n      - Get a project\n  - name: Entry_Read\n    documented: true\n    description: Read entries.\n    operations:\n      - Get an entry\n      - List entries\n      - List entries by content type\n  - name: Entry_Write\n    documented: true\n    description: Create, update and publish entries.\n    operations:\n      - Create an entry\n      - Update an entry\n      - Publish an entry\n  - name: Entry_Delete\n    documented: true\n    description: Delete an entry.\n    operations:\n      - Delete an entry\n  - name: ContentType_Read\n    documented: false\n    description: >-\n      Read content types. Not listed in the scopes table, but used in the provider's own\n      token-request example on\
  \ the same page (`scope=Entry_Read ContentType_Read Project_Read`).\n    operations: []\n    evidence: >-\n      Example request body on\n      https://www.contensis.com/help-and-docs/apis/management-http/security/scopes\nfindings:\n  - >-\n    The Management API surface is far larger than the scope table covers. The published\n    reference documents operations for components, content types, workflows, nodes,\n    domains, certificates, blocks, renderers, proxies, assets, roles, groups, users and\n    webhook subscriptions — none of which appear in the scopes table. Either those\n    operations are unscoped, or the table is incomplete; the docs do not say which.\n  - >-\n    ContentType_Read appearing in an example but not the table is a straightforward\n    documentation defect and the kind of thing that makes a client-credentials integration\n    fail on first run with a 401.\n  - >-\n    The Delivery API has no scopes at all — one environment-wide token, read everything.\n    See authentication/contensis-authentication.yml.\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/scopes/contensis-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CMS
- Content
- Headless CMS
- Content Management
- Digital Experience Platform
- Content Delivery
- Webhooks
- Higher Education
token_urls: []
---
