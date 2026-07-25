---
api_specs:
- filename: workday-studio-absence-management-api-openapi.yml
  format: yaml
  label: Workday Studio Absence Management API
  slug: workday-studio-absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-absence-management-api-openapi.yml
- filename: workday-studio-benefits-administration-api-openapi.yml
  format: yaml
  label: Workday Studio Benefits Administration API
  slug: workday-studio-benefits-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-benefits-administration-api-openapi.yml
- filename: workday-studio-compensation-api-openapi.yml
  format: yaml
  label: Workday Studio Compensation API
  slug: workday-studio-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-compensation-api-openapi.yml
- filename: workday-studio-financial-management-api-openapi.yml
  format: yaml
  label: Workday Studio Financial Management API
  slug: workday-studio-financial-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-financial-management-api-openapi.yml
- filename: workday-studio-human-resources-api-openapi.yml
  format: yaml
  label: Workday Studio Human Resources API
  slug: workday-studio-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-human-resources-api-openapi.yml
- filename: workday-studio-integration-assemblies-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Assemblies API
  slug: workday-studio-integration-assemblies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-assemblies-api-openapi.yml
- filename: workday-studio-integration-events-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Events API
  slug: workday-studio-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-events-api-openapi.yml
- filename: workday-studio-integration-systems-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Systems API
  slug: workday-studio-integration-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-systems-api-openapi.yml
- filename: workday-studio-integration-templates-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Templates API
  slug: workday-studio-integration-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-templates-api-openapi.yml
- filename: workday-studio-launch-parameters-api-openapi.yml
  format: yaml
  label: Workday Studio Launch Parameters API
  slug: workday-studio-launch-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-launch-parameters-api-openapi.yml
- filename: workday-studio-payroll-api-openapi.yml
  format: yaml
  label: Workday Studio Payroll API
  slug: workday-studio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-payroll-api-openapi.yml
- filename: workday-studio-recruiting-api-openapi.yml
  format: yaml
  label: Workday Studio Recruiting API
  slug: workday-studio-recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-recruiting-api-openapi.yml
- filename: workday-studio-service-directory-api-openapi.yml
  format: yaml
  label: Workday Studio Service Directory API
  slug: workday-studio-service-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-service-directory-api-openapi.yml
- filename: workday-studio-staffing-api-openapi.yml
  format: yaml
  label: Workday Studio Staffing API
  slug: workday-studio-staffing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-staffing-api-openapi.yml
- filename: workday-studio-time-tracking-api-openapi.yml
  format: yaml
  label: Workday Studio Time Tracking API
  slug: workday-studio-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-time-tracking-api-openapi.yml
authorization_urls:
- https://{baseUrl}/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Workday Studio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Studio publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Studio API on a user''s behalf.


  Tokens are issued from https://{baseUrl}/oauth2/{tenant}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Studio
provider_slug: workday-studio
schemes:
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/workday-studio-integration-openapi.yml
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  source: openapi/workday-studio-web-services-openapi.yml
scope_count: 4
scope_names:
- r:integrations
- r:wws
- w:integrations
- w:wws
scopes:
- description: Read integration data
  flows:
  - authorizationCode
  scope: r:integrations
- description: Read access to web services
  flows:
  - authorizationCode
  scope: r:wws
- description: Write integration data
  flows:
  - authorizationCode
  scope: w:integrations
- description: Write access to web services
  flows:
  - authorizationCode
  scope: w:wws
slug: workday-studio-scopes
source_filename: workday-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-studio-integration-openapi.yml, openapi/workday-studio-web-services-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/workday-studio-integration-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n- name: OAuth2\n  source: openapi/workday-studio-web-services-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\nscopes:\n- scope: r:integrations\n  description: Read integration data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-studio-integration-openapi.yml\n- scope: r:wws\n  description: Read access to web services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-studio-web-services-openapi.yml\n- scope: w:integrations\n  description: Write integration data\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-studio-integration-openapi.yml\n- scope: w:wws\n  description: Write access to web services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/workday-studio-web-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/scopes/workday-studio-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Cloud
- Development
- Enterprise
- Finance
- HR
- IDE
- Integration
token_urls:
- https://{baseUrl}/oauth2/{tenant}/token
---
