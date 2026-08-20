---
api_specs:
- filename: pdffiller-applications-api-openapi.yml
  format: yaml
  label: PDFfiller Applications API
  slug: pdffiller-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-applications-api-openapi.yml
- filename: pdffiller-auth-api-openapi.yml
  format: yaml
  label: PDFfiller Auth API
  slug: pdffiller-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-auth-api-openapi.yml
- filename: pdffiller-callbacks-api-openapi.yml
  format: yaml
  label: PDFfiller Callbacks API
  slug: pdffiller-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-callbacks-api-openapi.yml
- filename: pdffiller-custom-logos-api-openapi.yml
  format: yaml
  label: PDFfiller Custom Logos API
  slug: pdffiller-custom-logos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-custom-logos-api-openapi.yml
- filename: pdffiller-fillable-forms-api-openapi.yml
  format: yaml
  label: PDFfiller Fillable Forms API
  slug: pdffiller-fillable-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-fillable-forms-api-openapi.yml
- filename: pdffiller-folders-api-openapi.yml
  format: yaml
  label: PDFfiller Folders API
  slug: pdffiller-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-folders-api-openapi.yml
- filename: pdffiller-signature-requests-api-openapi.yml
  format: yaml
  label: PDFfiller Signature Requests API
  slug: pdffiller-signature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-signature-requests-api-openapi.yml
- filename: pdffiller-templates-api-openapi.yml
  format: yaml
  label: PDFfiller Templates API
  slug: pdffiller-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-templates-api-openapi.yml
- filename: pdffiller-tokens-api-openapi.yml
  format: yaml
  label: PDFfiller Tokens API
  slug: pdffiller-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-tokens-api-openapi.yml
- filename: pdffiller-tools-api-openapi.yml
  format: yaml
  label: PDFfiller Tools API
  slug: pdffiller-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-tools-api-openapi.yml
- filename: pdffiller-users-api-openapi.yml
  format: yaml
  label: PDFfiller Users API
  slug: pdffiller-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/openapi/pdffiller-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Pdffiller Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PDFfiller publishes 2 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PDFfiller API on a user''s behalf.


  Tokens are issued from https://api.pdffiller.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PDFfiller
provider_slug: pdffiller
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.pdffiller.com/v2/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.pdffiller.com/v2/oauth/token
  name: oauth2
  source: openapi/pdffiller-pdffiller-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access
  flows:
  - clientCredentials
  - password
  scope: read
- description: Write access
  flows:
  - clientCredentials
  - password
  scope: write
slug: pdffiller-scopes
source_filename: pdffiller-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pdffiller-pdffiller-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/pdffiller-pdffiller-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.pdffiller.com/v2/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.pdffiller.com/v2/oauth/token\nscopes:\n- scope: read\n  description: Read access\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/pdffiller-pdffiller-api-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/pdffiller-pdffiller-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pdffiller/refs/heads/main/scopes/pdffiller-scopes.yml
summary_line: 2 scopes · password/clientCredentials
tags:
- PDF
- E-Signature
- Document-Management
- Form Builder
- PDF Editing
- Electronic Signature
- Document Workflow
token_urls:
- https://api.pdffiller.com/v2/oauth/token
---
