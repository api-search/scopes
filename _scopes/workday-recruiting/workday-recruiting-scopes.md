---
api_specs:
- filename: workday-recruiting-agentdefinition-api-openapi.yml
  format: yaml
  label: Workday Recruiting agentDefinition API
  slug: workday-recruiting-agentdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-agentdefinition-api-openapi.yml
- filename: workday-recruiting-applicants-api-openapi.yml
  format: yaml
  label: Workday Recruiting Applicants API
  slug: workday-recruiting-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-applicants-api-openapi.yml
- filename: workday-recruiting-background-checks-api-openapi.yml
  format: yaml
  label: Workday Recruiting Background Checks API
  slug: workday-recruiting-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-background-checks-api-openapi.yml
- filename: workday-recruiting-candidates-api-openapi.yml
  format: yaml
  label: Workday Recruiting Candidates API
  slug: workday-recruiting-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-candidates-api-openapi.yml
- filename: workday-recruiting-configuration-api-openapi.yml
  format: yaml
  label: Workday Recruiting Configuration API
  slug: workday-recruiting-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-configuration-api-openapi.yml
- filename: workday-recruiting-evergreen-requisitions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Evergreen Requisitions API
  slug: workday-recruiting-evergreen-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-evergreen-requisitions-api-openapi.yml
- filename: workday-recruiting-interviews-api-openapi.yml
  format: yaml
  label: Workday Recruiting Interviews API
  slug: workday-recruiting-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-interviews-api-openapi.yml
- filename: workday-recruiting-job-applications-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Applications API
  slug: workday-recruiting-job-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-applications-api-openapi.yml
- filename: workday-recruiting-job-postings-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Postings API
  slug: workday-recruiting-job-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-postings-api-openapi.yml
- filename: workday-recruiting-job-requisitions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Requisitions API
  slug: workday-recruiting-job-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-requisitions-api-openapi.yml
- filename: workday-recruiting-positions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Positions API
  slug: workday-recruiting-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-positions-api-openapi.yml
- filename: workday-recruiting-recruiting-agencies-api-openapi.yml
  format: yaml
  label: Workday Recruiting Recruiting Agencies API
  slug: workday-recruiting-recruiting-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-recruiting-agencies-api-openapi.yml
authorization_urls:
- https://{tenant}.workday.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Workday Recruiting Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Recruiting publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Recruiting API on a user''s behalf.


  Tokens are issued from https://{tenant}.workday.com/ccx/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Recruiting
provider_slug: workday-recruiting
schemes:
- description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting scopes, and obtain access tokens.
  flows:
  - authorizationUrl: https://{tenant}.workday.com/authorize
    flow: authorizationCode
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token
  name: oauth2
  source: openapi/workday-recruiting-rest-api-openapi.yml
scope_count: 2
scope_names:
- recruiting:read
- recruiting:write
scopes:
- description: Read recruiting data
  flows:
  - authorizationCode
  scope: recruiting:read
- description: Modify recruiting data
  flows:
  - authorizationCode
  scope: recruiting:write
slug: workday-recruiting-scopes
source_filename: workday-recruiting-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-recruiting-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/workday-recruiting-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.workday.com/authorize\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/token\n  description: OAuth 2.0 authentication. Register an API client in Workday, grant recruiting\n    scopes, and obtain access tokens.\nscopes:\n- scope: recruiting:read\n  description: Read recruiting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-recruiting-rest-api-openapi.yml\n- scope: recruiting:write\n  description: Modify recruiting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-recruiting-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/scopes/workday-recruiting-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- HCM
- Human Resources
- Recruiting
- Software-as-a-Service
- Talent Acquisition
token_urls:
- https://{tenant}.workday.com/ccx/oauth2/token
---
