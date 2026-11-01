---
api_specs:
- filename: pdfbroker-io-pdf-api-openapi.yml
  format: yaml
  label: pdfbroker-io PDF API
  slug: pdfbroker-io-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pdfbroker-io/openapi/pdfbroker-io-pdf-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Pdfbroker Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'pdfbroker-io publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the pdfbroker-io API on a user''s behalf.


  Tokens are issued from https://login.pdfbroker.io/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: pdfbroker-io
provider_slug: pdfbroker-io
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.pdfbroker.io/connect/token
  name: OAuth2
  source: openapi/pdfbroker-io.json
scope_count: 1
scope_names:
- pdfbroker
scopes:
- description: Scope to access the PdfBroker API.
  flows:
  - clientCredentials
  scope: pdfbroker
slug: pdfbroker-io-scopes
source_filename: pdfbroker-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/pdfbroker-io.json\nschemes:\n- name: OAuth2\n  source: openapi/pdfbroker-io.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.pdfbroker.io/connect/token\nscopes:\n- scope: pdfbroker\n  description: Scope to access the PdfBroker API.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pdfbroker-io.json\n"
source_yaml_url: https://artifacts.apis.io/pdfbroker-io/scopes/pdfbroker-io-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- PDF Generation
- REST API
- HTML to PDF
- PDF/A
- PDF/UA
- PDF Utilities
- XSL-FO
token_bound: false
token_urls:
- https://login.pdfbroker.io/connect/token
---
