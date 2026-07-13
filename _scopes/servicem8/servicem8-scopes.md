---
api_specs:
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Jobs API
  slug: servicem8-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Job Activities API
  slug: servicem8-job-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Clients (Companies) API
  slug: servicem8-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Job Contacts API
  slug: servicem8-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Staff API
  slug: servicem8-staff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Materials API
  slug: servicem8-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Attachments API
  slug: servicem8-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Queues API
  slug: servicem8-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Vendors API
  slug: servicem8-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Badges API
  slug: servicem8-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
- filename: servicem8-openapi.yml
  format: yaml
  label: ServiceM8 Webhooks API
  slug: servicem8-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/openapi/servicem8-openapi.yml
authorization_urls:
- https://go.servicem8.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Servicem8 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ServiceM8 publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ServiceM8 API on a user''s behalf.


  Tokens are issued from https://go.servicem8.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ServiceM8
provider_slug: servicem8
schemes:
- description: OAuth 2.0 for public add-ons. Access tokens expire after 3600 seconds.
  flows:
  - authorizationUrl: https://go.servicem8.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://go.servicem8.com/oauth/access_token
  name: oauth2
  source: openapi/servicem8-openapi.yml
scope_count: 11
scope_names:
- manage_customers
- manage_inventory
- manage_jobs
- manage_schedule
- manage_staff
- publish_email
- publish_sms
- read_customers
- read_jobs
- read_staff
- vendor_logo
scopes:
- description: Read and write customers (companies)
  flows:
  - authorizationCode
  scope: manage_customers
- description: Read and write materials and inventory
  flows:
  - authorizationCode
  scope: manage_inventory
- description: Read and write jobs
  flows:
  - authorizationCode
  scope: manage_jobs
- description: Read and write scheduling and job activities
  flows:
  - authorizationCode
  scope: manage_schedule
- description: Read and write staff
  flows:
  - authorizationCode
  scope: manage_staff
- description: Send email messages
  flows:
  - authorizationCode
  scope: publish_email
- description: Send SMS messages
  flows:
  - authorizationCode
  scope: publish_sms
- description: Read customers (companies)
  flows:
  - authorizationCode
  scope: read_customers
- description: Read jobs
  flows:
  - authorizationCode
  scope: read_jobs
- description: Read staff
  flows:
  - authorizationCode
  scope: read_staff
- description: Read vendor account information
  flows:
  - authorizationCode
  scope: vendor_logo
slug: servicem8-scopes
source_filename: servicem8-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/servicem8-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/servicem8-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://go.servicem8.com/oauth/authorize\n    tokenUrl: https://go.servicem8.com/oauth/access_token\n  description: OAuth 2.0 for public add-ons. Access tokens expire after 3600 seconds.\nscopes:\n- scope: manage_customers\n  description: Read and write customers (companies)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: manage_inventory\n  description: Read and write materials and inventory\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: manage_jobs\n  description: Read and write jobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: manage_schedule\n  description: Read and write scheduling and job activities\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/servicem8-openapi.yml\n- scope: manage_staff\n  description: Read and write staff\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: publish_email\n  description: Send email messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: publish_sms\n  description: Send SMS messages\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: read_customers\n  description: Read customers (companies)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: read_jobs\n  description: Read jobs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: read_staff\n  description: Read staff\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n- scope: vendor_logo\n  description: Read vendor account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/servicem8-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicem8/refs/heads/main/scopes/servicem8-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Field Service
- Job Management
- Trades
- Scheduling
- Dispatch
- Invoicing
- Home Services
token_urls:
- https://go.servicem8.com/oauth/access_token
---
