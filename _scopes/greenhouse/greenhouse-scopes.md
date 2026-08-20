---
api_specs:
- filename: greenhouse-applications-api-openapi.yml
  format: yaml
  label: Greenhouse Applications API
  slug: greenhouse-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-applications-api-openapi.yml
- filename: greenhouse-candidates-api-openapi.yml
  format: yaml
  label: Greenhouse Candidates API
  slug: greenhouse-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-candidates-api-openapi.yml
- filename: greenhouse-departments-api-openapi.yml
  format: yaml
  label: Greenhouse Departments API
  slug: greenhouse-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-departments-api-openapi.yml
- filename: greenhouse-education-api-openapi.yml
  format: yaml
  label: Greenhouse Education API
  slug: greenhouse-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-education-api-openapi.yml
- filename: greenhouse-graphql-api-openapi.yml
  format: yaml
  label: Greenhouse Graphql API
  slug: greenhouse-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-graphql-api-openapi.yml
- filename: greenhouse-greenhouse-job-board-api-api-openapi.yml
  format: yaml
  label: Greenhouse Greenhouse Job Board API API
  slug: greenhouse-greenhouse-job-board-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-greenhouse-job-board-api-api-openapi.yml
- filename: greenhouse-jobs-api-openapi.yml
  format: yaml
  label: Greenhouse Jobs API
  slug: greenhouse-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-jobs-api-openapi.yml
- filename: greenhouse-offices-api-openapi.yml
  format: yaml
  label: Greenhouse Offices API
  slug: greenhouse-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-offices-api-openapi.yml
- filename: greenhouse-prospects-api-openapi.yml
  format: yaml
  label: Greenhouse Prospects API
  slug: greenhouse-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-prospects-api-openapi.yml
- filename: greenhouse-sections-api-openapi.yml
  format: yaml
  label: Greenhouse Sections API
  slug: greenhouse-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-sections-api-openapi.yml
- filename: greenhouse-tracking-api-openapi.yml
  format: yaml
  label: Greenhouse Tracking API
  slug: greenhouse-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-tracking-api-openapi.yml
- filename: greenhouse-users-api-openapi.yml
  format: yaml
  label: Greenhouse Users API
  slug: greenhouse-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-users-api-openapi.yml
authorization_urls:
- https://api.greenhouse.io/oauth/authorize
description: ''
docs: https://developers.greenhouse.io/candidate-ingestion.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Greenhouse Scopes
name_suffix: OAuth Scopes
note: The Candidate Ingestion API documents four OAuth permission scopes (they do not apply when authenticating via Basic Auth). The Harvest API v3 also uses granular OAuth scopes in the pattern harvest:<resource>:<action> (via auth.greenhouse.io), but Greenhouse publishes no complete public list; only the two example scopes named in the Harvest partner OAuth guide (https://harvestdocs.greenhouse.io/docs/harvest-partner-oauth) are recorded here.
overview: 'Greenhouse publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Greenhouse API on a user''s behalf.


  Tokens are issued from https://api.greenhouse.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Greenhouse
provider_slug: greenhouse
schemes:
- flows:
  - authorizationUrl: https://api.greenhouse.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.greenhouse.io/oauth/token
  name: oauth2
  source: openapi/greenhouse-ingestion-openapi.yml
scope_count: 6
scope_names:
- candidates.create
- candidates.view
- jobs.view
- prospect_pools.view
- harvest:candidates:list
- harvest:job_posts:list
scopes:
- description: Create new candidates or prospects.
  flows: []
  scope: candidates.create
- description: View candidates imported via this partner.
  flows: []
  scope: candidates.view
- description: View my jobs.
  flows: []
  scope: jobs.view
- description: Retrieve prospect pools and their stages for an organization.
  flows: []
  scope: prospect_pools.view
- description: List candidates via the Harvest API v3 (example scope named in the Harvest partner OAuth guide).
  flows: []
  scope: harvest:candidates:list
- description: List job posts via the Harvest API v3 (example scope named in the Harvest partner OAuth guide).
  flows: []
  scope: harvest:job_posts:list
slug: greenhouse-scopes
source_filename: greenhouse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/greenhouse-ingestion-openapi.yml\ndocs: https://developers.greenhouse.io/candidate-ingestion.html\nnote: >-\n  The Candidate Ingestion API documents four OAuth permission scopes (they do not apply\n  when authenticating via Basic Auth). The Harvest API v3 also uses granular OAuth scopes\n  in the pattern harvest:<resource>:<action> (via auth.greenhouse.io), but Greenhouse\n  publishes no complete public list; only the two example scopes named in the Harvest\n  partner OAuth guide (https://harvestdocs.greenhouse.io/docs/harvest-partner-oauth)\n  are recorded here.\nschemes:\n- name: oauth2\n  source: openapi/greenhouse-ingestion-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.greenhouse.io/oauth/authorize\n    tokenUrl: https://api.greenhouse.io/oauth/token\nscopes:\n- scope: candidates.create\n  description: Create new candidates or prospects.\n  sources:\n  - https://developers.greenhouse.io/candidate-ingestion.html\n\
  - scope: candidates.view\n  description: View candidates imported via this partner.\n  sources:\n  - https://developers.greenhouse.io/candidate-ingestion.html\n- scope: jobs.view\n  description: View my jobs.\n  sources:\n  - https://developers.greenhouse.io/candidate-ingestion.html\n- scope: prospect_pools.view\n  description: Retrieve prospect pools and their stages for an organization.\n  sources:\n  - https://developers.greenhouse.io/candidate-ingestion.html\n- scope: harvest:candidates:list\n  description: List candidates via the Harvest API v3 (example scope named in the Harvest partner OAuth guide).\n  sources:\n  - https://harvestdocs.greenhouse.io/docs/harvest-partner-oauth\n- scope: harvest:job_posts:list\n  description: List job posts via the Harvest API v3 (example scope named in the Harvest partner OAuth guide).\n  sources:\n  - https://harvestdocs.greenhouse.io/docs/harvest-partner-oauth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/scopes/greenhouse-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- ATS
- Recruiting
- Candidates
- Job
- Onboarding
- HR
token_urls:
- https://api.greenhouse.io/oauth/token
---
