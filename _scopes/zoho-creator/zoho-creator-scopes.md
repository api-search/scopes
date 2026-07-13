---
api_specs:
- filename: downloadOAS
  format: yaml
  label: Zoho Creator REST API v2.1
  slug: zoho-creator-rest-api-v21
  spec_type: OpenAPI
  url: https://creator.zoho.com/api/v2/downloadOAS
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth?access_type=offline
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Creator Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Creator publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Creator API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Creator
provider_slug: zoho-creator
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth?access_type=offline
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: oauth2
  source: openapi/openapi.json
scope_count: 10
scope_names:
- ZohoCreator.bulk.CREATE
- ZohoCreator.bulk.READ
- ZohoCreator.dashboard.READ
- ZohoCreator.form.CREATE
- ZohoCreator.meta.application.READ
- ZohoCreator.meta.form.READ
- ZohoCreator.report.CREATE
- ZohoCreator.report.DELETE
- ZohoCreator.report.READ
- ZohoCreator.report.UPDATE
scopes:
- description: Create a bulk read or bulk insert job.
  flows:
  - authorizationCode
  scope: ZohoCreator.bulk.CREATE
- description: Check the status or download the result of a bulk read or bulk insert job.
  flows:
  - authorizationCode
  scope: ZohoCreator.bulk.READ
- description: Get applications.
  flows:
  - authorizationCode
  scope: ZohoCreator.dashboard.READ
- description: Add records to a form.
  flows:
  - authorizationCode
  scope: ZohoCreator.form.CREATE
- description: Get forms, reports in an application.
  flows:
  - authorizationCode
  scope: ZohoCreator.meta.application.READ
- description: Get list of fields in a form.
  flows:
  - authorizationCode
  scope: ZohoCreator.meta.form.READ
- description: Upload file to a record in a report.
  flows:
  - authorizationCode
  scope: ZohoCreator.report.CREATE
- description: Delete records in a report.
  flows:
  - authorizationCode
  scope: ZohoCreator.report.DELETE
- description: Get records and download file in a report.
  flows:
  - authorizationCode
  scope: ZohoCreator.report.READ
- description: Update records in a report.
  flows:
  - authorizationCode
  scope: ZohoCreator.report.UPDATE
slug: zoho-creator-scopes
source_filename: zoho-creator-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nschemes:\n- name: oauth2\n  source: openapi/openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth?access_type=offline\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\nscopes:\n- scope: ZohoCreator.bulk.CREATE\n  description: Create a bulk read or bulk insert job.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.bulk.READ\n  description: Check the status or download the result of a bulk read or bulk insert job.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.dashboard.READ\n  description: Get applications.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.form.CREATE\n  description: Add records to a form.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.meta.application.READ\n\
  \  description: Get forms, reports in an application.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.meta.form.READ\n  description: Get list of fields in a form.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.report.CREATE\n  description: Upload file to a record in a report.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.report.DELETE\n  description: Delete records in a report.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.report.READ\n  description: Get records and download file in a report.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n- scope: ZohoCreator.report.UPDATE\n  description: Update records in a report.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/scopes/zoho-creator-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Low-Code
- Application Development
- No-Code
- Forms
- Records
- Workflows
- Database
- CRUD
- Business Applications
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
