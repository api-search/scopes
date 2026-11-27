---
api_specs:
- filename: google-cloud-data-catalog-catalog-api-openapi.yml
  format: yaml
  label: Google Cloud Data Catalog Catalog API
  slug: google-cloud-data-catalog-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-data-catalog/openapi/google-cloud-data-catalog-catalog-api-openapi.yml
- filename: google-cloud-data-catalog-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Data Catalog Folders API
  slug: google-cloud-data-catalog-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-data-catalog/openapi/google-cloud-data-catalog-folders-api-openapi.yml
- filename: google-cloud-data-catalog-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Data Catalog Organizations API
  slug: google-cloud-data-catalog-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-data-catalog/openapi/google-cloud-data-catalog-organizations-api-openapi.yml
- filename: google-cloud-data-catalog-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Data Catalog Projects API
  slug: google-cloud-data-catalog-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-data-catalog/openapi/google-cloud-data-catalog-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Data Catalog Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Data Catalog publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Data Catalog API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Data Catalog
provider_slug: google-cloud-data-catalog
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-data-catalog-datacatalog-catalog-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-data-catalog-datacatalog-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-data-catalog-datacatalog-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-data-catalog-datalineage-folders-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-data-catalog-datalineage-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-data-catalog-datalineage-projects-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/datalineage.read-write
- https://www.googleapis.com/auth/datalineage.readonly
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: See, edit, configure, and delete your Google Cloud Data Lineage data and see the email address for your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/datalineage.read-write
- description: See your Google Cloud Data Lineage data and the email address of your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/datalineage.readonly
slug: google-cloud-data-catalog-scopes
source_filename: google-cloud-data-catalog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-data-catalog-datacatalog-catalog-api-openapi.yml, openapi/google-cloud-data-catalog-datacatalog-organizations-api-openapi.yml,\n  openapi/google-cloud-data-catalog-datacatalog-projects-api-openapi.yml, openapi/google-cloud-data-catalog-datalineage-folders-api-openapi.yml,\n  openapi/google-cloud-data-catalog-datalineage-organizations-api-openapi.yml, openapi/google-cloud-data-catalog-datalineage-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-data-catalog-datacatalog-catalog-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-data-catalog-datacatalog-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n\
  - name: oauth2\n  source: openapi/google-cloud-data-catalog-datacatalog-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-data-catalog-datalineage-folders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-data-catalog-datalineage-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-data-catalog-datalineage-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n\
  scopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-data-catalog-datacatalog-catalog-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datacatalog-organizations-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datacatalog-projects-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datalineage-folders-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datalineage-organizations-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datalineage-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/datalineage.read-write\n  description: See, edit, configure, and delete your Google Cloud Data Lineage data and see\n    the email address for your Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-data-catalog-datalineage-folders-api-openapi.yml\n\
  \  - openapi/google-cloud-data-catalog-datalineage-organizations-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datalineage-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/datalineage.readonly\n  description: See your Google Cloud Data Lineage data and the email address of your Google\n    Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-data-catalog-datalineage-folders-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datalineage-organizations-api-openapi.yml\n  - openapi/google-cloud-data-catalog-datalineage-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-data-catalog/scopes/google-cloud-data-catalog-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Data Catalog
- Data Governance
- Google Cloud
- Metadata
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
