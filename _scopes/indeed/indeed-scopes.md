---
api_specs:
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Job Sync API
  slug: job-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Employer API
  slug: employer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Indeed Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Indeed publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Indeed API on a user''s behalf.


  Tokens are issued from https://apis.indeed.com/oauth/v2/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Indeed
provider_slug: indeed
schemes:
- description: Indeed OAuth 2.0 authentication for partner applications.
  flows:
  - flow: clientCredentials
    tokenUrl: https://apis.indeed.com/oauth/v2/tokens
  name: OAuth2
  source: openapi/indeed-employer-api-openapi.yml
scope_count: 3
scope_names:
- candidate_read
- employer_access
- job_posting_write
scopes:
- description: Read candidate and application data
  flows:
  - clientCredentials
  scope: candidate_read
- description: Access and manage employer data
  flows:
  - clientCredentials
  scope: employer_access
- description: Create and manage job postings
  flows:
  - clientCredentials
  scope: job_posting_write
slug: indeed-scopes
source_filename: indeed-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/indeed-employer-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/indeed-employer-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.indeed.com/oauth/v2/tokens\n  description: Indeed OAuth 2.0 authentication for partner applications.\nscopes:\n- scope: candidate_read\n  description: Read candidate and application data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/indeed-employer-api-openapi.yml\n- scope: employer_access\n  description: Access and manage employer data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/indeed-employer-api-openapi.yml\n- scope: job_posting_write\n  description: Create and manage job postings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/indeed-employer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/scopes/indeed-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
token_urls:
- https://apis.indeed.com/oauth/v2/tokens
---
