---
api_specs:
- filename: microsoft-viva-employeeexperience-community-api-openapi.yml
  format: yaml
  label: Microsoft Viva Employee Experience.community API
  slug: microsoft-viva-employeeexperience-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-employeeexperience-community-api-openapi.yml
- filename: microsoft-viva-employeeexperience-employeeexperience-api-openapi.yml
  format: yaml
  label: Microsoft Viva Employee Experience.employee Experience API
  slug: microsoft-viva-employeeexperience-employeeexperience-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-employeeexperience-employeeexperience-api-openapi.yml
- filename: microsoft-viva-employeeexperience-engagementasyncoperation-api-openapi.yml
  format: yaml
  label: Microsoft Viva Employee Experience.engagement Async Operation API
  slug: microsoft-viva-employeeexperience-engagementasyncoperation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-employeeexperience-engagementasyncoperation-api-openapi.yml
- filename: microsoft-viva-employeeexperience-engagementrole-api-openapi.yml
  format: yaml
  label: Microsoft Viva Employee Experience.engagement Role API
  slug: microsoft-viva-employeeexperience-engagementrole-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-employeeexperience-engagementrole-api-openapi.yml
- filename: microsoft-viva-employeeexperience-learningcourseactivity-api-openapi.yml
  format: yaml
  label: Microsoft Viva Employee Experience.learning Course Activity API
  slug: microsoft-viva-employeeexperience-learningcourseactivity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-employeeexperience-learningcourseactivity-api-openapi.yml
- filename: microsoft-viva-employeeexperience-learningprovider-api-openapi.yml
  format: yaml
  label: Microsoft Viva Employee Experience.learning Provider API
  slug: microsoft-viva-employeeexperience-learningprovider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-employeeexperience-learningprovider-api-openapi.yml
- filename: microsoft-viva-me-employeeexperienceuser-api-openapi.yml
  format: yaml
  label: Microsoft Viva Me.employee Experience User API
  slug: microsoft-viva-me-employeeexperienceuser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-me-employeeexperienceuser-api-openapi.yml
- filename: microsoft-viva-users-employeeexperienceuser-api-openapi.yml
  format: yaml
  label: Microsoft Viva Users.employee Experience User API
  slug: microsoft-viva-users-employeeexperienceuser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-viva/openapi/microsoft-viva-users-employeeexperienceuser-api-openapi.yml
authorization_urls: []
description: ''
docs: https://learn.microsoft.com/en-us/graph/permissions-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Microsoft Viva Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Viva publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Viva API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Viva
provider_slug: microsoft-viva
schemes: []
scope_count: 3
scope_names:
- LearningProvider.Read
- LearningProvider.ReadWrite
- Community.ReadWrite.All
scopes:
- description: Least privileged to list learning providers (work or school account); application not supported.
  flows: []
  scope: LearningProvider.Read
- description: Higher privileged for learning provider operations.
  flows: []
  scope: LearningProvider.ReadWrite
- description: Required to create Viva Engage communities (POST /employeeExperience/communities).
  flows: []
  scope: Community.ReadWrite.All
slug: microsoft-viva-scopes
source_filename: microsoft-viva-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/graph/api/employeeexperience-list-learningproviders?view=graph-rest-1.0\ndocs: https://learn.microsoft.com/en-us/graph/permissions-reference\nscopes:\n- name: LearningProvider.Read\n  type: delegated\n  description: Least privileged to list learning providers (work or school account); application not supported.\n- name: LearningProvider.ReadWrite\n  type: delegated\n  description: Higher privileged for learning provider operations.\n- name: Community.ReadWrite.All\n  type: delegated+application\n  description: Required to create Viva Engage communities (POST /employeeExperience/communities).\n  source: https://learn.microsoft.com/en-us/graph/api/employeeexperience-post-communities?view=graph-rest-1.0\n"
source_yaml_url: https://artifacts.apis.io/microsoft-viva/scopes/microsoft-viva-scopes.yml
summary_line: 3 scopes
tags:
- Employee Experience
- Insights
- Learning
- Microsoft
- Microsoft 365
token_bound: false
token_urls: []
---
