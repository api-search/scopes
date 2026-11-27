---
api_specs:
- filename: google-cloud-vmware-engine-projects-api-openapi.yml
  format: yaml
  label: Google Cloud VMware Engine Cloud Vmware Engine Projects API
  slug: google-cloud-vmware-engine-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-vmware-engine/openapi/google-cloud-vmware-engine-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud VMware Engine Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud VMware Engine publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud VMware Engine API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud VMware Engine
provider_slug: google-cloud-vmware-engine
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-vmware-engine-projects-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-cloud-vmware-engine-scopes
source_filename: google-cloud-vmware-engine-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-vmware-engine-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-vmware-engine-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-vmware-engine-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-vmware-engine/scopes/google-cloud-vmware-engine-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Compute
- Google Cloud
- Migration
- Private Cloud
- Virtualization
- VMware
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
