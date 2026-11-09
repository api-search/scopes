---
api_specs:
- filename: filetypeconverters-com-batches-api-openapi.yml
  format: yaml
  label: FileType Converters Batches API
  slug: filetypeconverters-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-batches-api-openapi.yml
- filename: filetypeconverters-com-convert-api-openapi.yml
  format: yaml
  label: FileType Converters Convert API
  slug: filetypeconverters-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-convert-api-openapi.yml
- filename: filetypeconverters-com-formats-api-openapi.yml
  format: yaml
  label: FileType Converters Formats API
  slug: filetypeconverters-com-formats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-formats-api-openapi.yml
- filename: filetypeconverters-com-jobs-api-openapi.yml
  format: yaml
  label: FileType Converters Jobs API
  slug: filetypeconverters-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-jobs-api-openapi.yml
- filename: filetypeconverters-com-openapi-json-api-openapi.yml
  format: yaml
  label: FileType Converters Openapi.json API
  slug: filetypeconverters-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-openapi-json-api-openapi.yml
- filename: filetypeconverters-com-pairs-api-openapi.yml
  format: yaml
  label: FileType Converters Pairs API
  slug: filetypeconverters-com-pairs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-pairs-api-openapi.yml
- filename: filetypeconverters-com-usage-api-openapi.yml
  format: yaml
  label: FileType Converters Usage API
  slug: filetypeconverters-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-usage-api-openapi.yml
authorization_urls: []
description: ''
docs: https://filetypeconverters.com/api/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Filetypeconverters Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FileType Converters publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the FileType Converters API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FileType Converters
provider_slug: filetypeconverters-com
schemes: []
scope_count: 6
scope_names:
- convert
- jobs:read
- batches:write
- batches:read
- usage:read
- '*'
scopes:
- description: Create sync and async conversions.
  flows: []
  scope: convert
- description: Read job status and download job outputs.
  flows: []
  scope: jobs:read
- description: Create conversion batches.
  flows: []
  scope: batches:write
- description: Read batch status and download ZIP archives.
  flows: []
  scope: batches:read
- description: Read entitlements and current-month usage.
  flows: []
  scope: usage:read
- description: Allow every HTTP API scope on the key.
  flows: []
  scope: '*'
slug: filetypeconverters-com-scopes
source_filename: filetypeconverters-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filetypeconverters.com/api/authentication\ndocs: https://filetypeconverters.com/api/authentication\nname: FileType Converters API key scopes\nscopes:\n  - name: convert\n    description: Create sync and async conversions.\n  - name: jobs:read\n    description: Read job status and download job outputs.\n  - name: batches:write\n    description: Create conversion batches.\n  - name: batches:read\n    description: Read batch status and download ZIP archives.\n  - name: usage:read\n    description: Read entitlements and current-month usage.\n  - name: '*'\n    description: Allow every HTTP API scope on the key.\nmcp_permissions:\n  - name: convert\n    maps_to: conversion routes\n  - name: read\n    maps_to: jobs:read and batches:read\n"
source_yaml_url: https://artifacts.apis.io/filetypeconverters-com/scopes/filetypeconverters-com-scopes.yml
summary_line: 6 scopes
tags:
- File Conversion
- Document Conversion
- PDF
- OCR
- Spreadsheets
- Images
- MCP
- Developer API
- AI Deep Read
- File Formats
token_bound: false
token_urls: []
---
