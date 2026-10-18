---
api_specs:
- filename: lucca-employee-attributes-api-openapi.yml
  format: yaml
  label: Lucca Employee Attributes API
  slug: lucca-employee-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-attributes-api-openapi.yml
- filename: lucca-employee-job-qualifications-api-openapi.yml
  format: yaml
  label: Lucca Employee Job Qualifications API
  slug: lucca-employee-job-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-job-qualifications-api-openapi.yml
- filename: lucca-employee-occupation-categories-api-openapi.yml
  format: yaml
  label: Lucca Employee Occupation Categories API
  slug: lucca-employee-occupation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-occupation-categories-api-openapi.yml
- filename: lucca-employees-api-openapi.yml
  format: yaml
  label: Lucca Employees API
  slug: lucca-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employees-api-openapi.yml
- filename: lucca-employments-api-openapi.yml
  format: yaml
  label: Lucca Employments API
  slug: lucca-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employments-api-openapi.yml
- filename: lucca-events-api-openapi.yml
  format: yaml
  label: Lucca Events API
  slug: lucca-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-events-api-openapi.yml
- filename: lucca-files-api-openapi.yml
  format: yaml
  label: Lucca Files API
  slug: lucca-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-files-api-openapi.yml
- filename: lucca-organization-api-openapi.yml
  format: yaml
  label: Lucca Organization API
  slug: lucca-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-organization-api-openapi.yml
- filename: lucca-taxonomies-api-openapi.yml
  format: yaml
  label: Lucca Taxonomies API
  slug: lucca-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-taxonomies-api-openapi.yml
- filename: lucca-webhooks-api-openapi.yml
  format: yaml
  label: Lucca Webhooks API
  slug: lucca-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-webhooks-api-openapi.yml
- filename: lucca-working-time-arrangements-api-openapi.yml
  format: yaml
  label: Lucca Working Time Arrangements API
  slug: lucca-working-time-arrangements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-working-time-arrangements-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Lucca Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lucca publishes 36 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lucca API on a user''s behalf.


  Tokens are issued from https://accounts.world.luccasoftware.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lucca
provider_slug: lucca
schemes:
- description: The Lucca API implements the [oAuth 2](https://oauth.net/2/) protocol with the [client-credentials-flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/client-credentials-flow). Refer to RFC8725.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.world.luccasoftware.com/connect/token
  name: oAuth
  source: openapi/lucca-api-2024-11-01.json
scope_count: 36
scope_names:
- business-establishments.readonly
- business-establishments.readwrite
- departments.readonly
- departments.readwrite
- employee-attribute-definitions.readonly
- employee-attribute-definitions.readwrite
- employee-attributes.readonly
- employee-attributes.readwrite
- employee-personal-records.readonly
- employee-personal-records.readwrite
- employees.readonly
- employees.readwrite
- employment-templates.readonly
- employment-templates.readwrite
- employments.readonly
- employments.readwrite
- events.readonly
- files.readonly
- files.readwrite
- job-positions.readonly
- job-positions.readwrite
- job-qualifications.readonly
- job-qualifications.readwrite
- legal-entities.readonly
- legal-entities.readwrite
- occupation-categories.readonly
- occupation-categories.readwrite
- probationary-periods.readonly
- probationary-periods.readwrite
- taxonomies.readonly
- taxonomies.readwrite
- webhook-deliveries.readonly
- webhook-deliveries.readwrite
- webhook-endpoints.readonly
- webhook-endpoints.readwrite
- working-time-arrangements.readonly
scopes:
- description: Read [business-establishments](/api-reference/latest/organization/business-establishment).
  flows:
  - clientCredentials
  scope: business-establishments.readonly
- description: Create, update or delete [business-establishments](/api-reference/latest/organization/business-establishment).
  flows:
  - clientCredentials
  scope: business-establishments.readwrite
- description: Read [departments](/api-reference/latest/organization/department).
  flows:
  - clientCredentials
  scope: departments.readonly
- description: Create, update or delete [departments](/api-reference/latest/organization/department).
  flows:
  - clientCredentials
  scope: departments.readwrite
- description: Read [employee-attribute-definitions](/api-reference/latest/employee-attributes/employee-attribute-definition).
  flows:
  - clientCredentials
  scope: employee-attribute-definitions.readonly
- description: Create, update or delete [employee-attribute-definitions](/api-reference/latest/employee-attributes/employee-attribute-definition) and [taxonomies](/api-reference/latest/taxonomies/taxonomy).
  flows:
  - clientCredentials
  scope: employee-attribute-definitions.readwrite
- description: Read [employee-attributes](/api-reference/latest/employee-attributes/employee-attribute).
  flows:
  - clientCredentials
  scope: employee-attributes.readonly
- description: Create, update or delete [employee-attributes](/api-reference/latest/employee-attributes/employee-attribute).
  flows:
  - clientCredentials
  scope: employee-attributes.readwrite
- description: Read [employee-personal-records](/api-reference/latest/employees/employee-personal-records). This contains highly sensitive data about the personal detail of the person.
  flows:
  - clientCredentials
  scope: employee-personal-records.readonly
- description: Create, update or delete [employee-personal-records](/api-reference/latest/employees/employee-personal-records). This contains highly sensitive data about the personal detail of the person.
  flows:
  - clientCredentials
  scope: employee-personal-records.readwrite
- description: Read [employees](/api-reference/latest/employees/employee).
  flows:
  - clientCredentials
  scope: employees.readonly
- description: Create or update [employees](/api-reference/latest/employees/employee).
  flows:
  - clientCredentials
  scope: employees.readwrite
- description: Read [employment-templates](/api-reference/latest/employments/employment-template).
  flows:
  - clientCredentials
  scope: employment-templates.readonly
- description: Create, update or archive [employment-templates](/api-reference/latest/employments/employment-template).
  flows:
  - clientCredentials
  scope: employment-templates.readwrite
- description: Read [employments](/api-reference/latest/employments/employment).
  flows:
  - clientCredentials
  scope: employments.readonly
- description: Create, update or delete [employments](/api-reference/latest/employments/employment).
  flows:
  - clientCredentials
  scope: employments.readwrite
- description: Read [events](/api-reference/latest/events/event). Only events of resources covered by the client's other scopes are returned (see [access control](/api-reference/latest/events/access-control)).
  flows:
  - clientCredentials
  scope: events.readonly
- description: Read files stored in Lucca.
  flows:
  - clientCredentials
  scope: files.readonly
- description: Upload a file to Lucca.
  flows:
  - clientCredentials
  scope: files.readwrite
- description: Read [job-positions](/api-reference/latest/employments/job-position).
  flows:
  - clientCredentials
  scope: job-positions.readonly
- description: Create, update or delete [job-positions](/api-reference/latest/employments/job-position).
  flows:
  - clientCredentials
  scope: job-positions.readwrite
- description: Read [job-qualifications](/api-reference/latest/employee-occupations/job-qualification) and [professions](/api-reference/latest/employee-occupations/profession).
  flows:
  - clientCredentials
  scope: job-qualifications.readonly
- description: Create, update or delete [job-qualifications](/api-reference/latest/employee-occupations/job-qualification) and [professions](/api-reference/latest/employee-occupations/profession).
  flows:
  - clientCredentials
  scope: job-qualifications.readwrite
- description: Read [legal-entities](/api-reference/latest/organization/legal-entity).
  flows:
  - clientCredentials
  scope: legal-entities.readonly
- description: Create, update or delete [legal-entities](/api-reference/latest/organization/legal-entity).
  flows:
  - clientCredentials
  scope: legal-entities.readwrite
- description: Read [occupation-categories](/api-reference/latest/employee-occupations/occupation-category).
  flows:
  - clientCredentials
  scope: occupation-categories.readonly
- description: Create, update or delete [occupation-categories](/api-reference/latest/employee-occupations/occupation-category).
  flows:
  - clientCredentials
  scope: occupation-categories.readwrite
- description: Read [probationary-periods](/api-reference/latest/employments/probationary-period).
  flows:
  - clientCredentials
  scope: probationary-periods.readonly
- description: Create, update or delete [probationary-periods](/api-reference/latest/employments/probationary-period).
  flows:
  - clientCredentials
  scope: probationary-periods.readwrite
- description: Read [taxonomies](/api-reference/latest/taxonomies/taxonomy) and [taxonomy-labels](/api-reference/latest/taxonomies/taxonomy-label).
  flows:
  - clientCredentials
  scope: taxonomies.readonly
- description: Create, update or delete [taxonomies](/api-reference/latest/taxonomies/taxonomy) and [taxonomy-labels](/api-reference/latest/taxonomies/taxonomy-label).
  flows:
  - clientCredentials
  scope: taxonomies.readwrite
- description: Read webhook-deliveries.
  flows:
  - clientCredentials
  scope: webhook-deliveries.readonly
- description: Send a ping event to a webhook-endpoint.
  flows:
  - clientCredentials
  scope: webhook-deliveries.readwrite
- description: Read webhook-endpoints.
  flows:
  - clientCredentials
  scope: webhook-endpoints.readonly
- description: Create and update webhook-endpoints.
  flows:
  - clientCredentials
  scope: webhook-endpoints.readwrite
- description: Read working-time-arrangements.
  flows:
  - clientCredentials
  scope: working-time-arrangements.readonly
slug: lucca-scopes
source_filename: lucca-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/lucca-api-2024-11-01.json\nschemes:\n- name: oAuth\n  source: openapi/lucca-api-2024-11-01.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.world.luccasoftware.com/connect/token\n  description: The Lucca API implements the [oAuth 2](https://oauth.net/2/) protocol with the\n    [client-credentials-flow](https://auth0.com/docs/get-started/authentication-and-authorization-flow/client-credentials-flow).\n    Refer to RFC8725.\nscopes:\n- scope: business-establishments.readonly\n  description: Read [business-establishments](/api-reference/latest/organization/business-establishment).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: business-establishments.readwrite\n  description: Create, update or delete [business-establishments](/api-reference/latest/organization/business-establishment).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n\
  - scope: departments.readonly\n  description: Read [departments](/api-reference/latest/organization/department).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: departments.readwrite\n  description: Create, update or delete [departments](/api-reference/latest/organization/department).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employee-attribute-definitions.readonly\n  description: Read [employee-attribute-definitions](/api-reference/latest/employee-attributes/employee-attribute-definition).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employee-attribute-definitions.readwrite\n  description: |-\n    Create, update or delete [employee-attribute-definitions](/api-reference/latest/employee-attributes/employee-attribute-definition)\n    and [taxonomies](/api-reference/latest/taxonomies/taxonomy).\n  flows:\n  - clientCredentials\n  sources:\n  -\
  \ openapi/lucca-api-2024-11-01.json\n- scope: employee-attributes.readonly\n  description: Read [employee-attributes](/api-reference/latest/employee-attributes/employee-attribute).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employee-attributes.readwrite\n  description: Create, update or delete [employee-attributes](/api-reference/latest/employee-attributes/employee-attribute).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employee-personal-records.readonly\n  description: |-\n    Read [employee-personal-records](/api-reference/latest/employees/employee-personal-records).\n    This contains highly sensitive data about the personal detail of the person.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employee-personal-records.readwrite\n  description: |-\n    Create, update or delete [employee-personal-records](/api-reference/latest/employees/employee-personal-records).\n\
  \    This contains highly sensitive data about the personal detail of the person.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employees.readonly\n  description: Read [employees](/api-reference/latest/employees/employee).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employees.readwrite\n  description: Create or update [employees](/api-reference/latest/employees/employee).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employment-templates.readonly\n  description: Read [employment-templates](/api-reference/latest/employments/employment-template).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employment-templates.readwrite\n  description: Create, update or archive [employment-templates](/api-reference/latest/employments/employment-template).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n\
  - scope: employments.readonly\n  description: Read [employments](/api-reference/latest/employments/employment).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: employments.readwrite\n  description: Create, update or delete [employments](/api-reference/latest/employments/employment).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: events.readonly\n  description: |-\n    Read [events](/api-reference/latest/events/event).\n    Only events of resources covered by the client's other scopes are returned (see [access control](/api-reference/latest/events/access-control)).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: files.readonly\n  description: Read files stored in Lucca.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: files.readwrite\n  description: Upload a file to Lucca.\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: job-positions.readonly\n  description: Read [job-positions](/api-reference/latest/employments/job-position).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: job-positions.readwrite\n  description: Create, update or delete [job-positions](/api-reference/latest/employments/job-position).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: job-qualifications.readonly\n  description: Read [job-qualifications](/api-reference/latest/employee-occupations/job-qualification)\n    and [professions](/api-reference/latest/employee-occupations/profession).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: job-qualifications.readwrite\n  description: Create, update or delete [job-qualifications](/api-reference/latest/employee-occupations/job-qualification)\n    and [professions](/api-reference/latest/employee-occupations/profession).\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: legal-entities.readonly\n  description: Read [legal-entities](/api-reference/latest/organization/legal-entity).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: legal-entities.readwrite\n  description: Create, update or delete [legal-entities](/api-reference/latest/organization/legal-entity).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: occupation-categories.readonly\n  description: Read [occupation-categories](/api-reference/latest/employee-occupations/occupation-category).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: occupation-categories.readwrite\n  description: Create, update or delete [occupation-categories](/api-reference/latest/employee-occupations/occupation-category).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n\
  - scope: probationary-periods.readonly\n  description: Read [probationary-periods](/api-reference/latest/employments/probationary-period).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: probationary-periods.readwrite\n  description: Create, update or delete [probationary-periods](/api-reference/latest/employments/probationary-period).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: taxonomies.readonly\n  description: Read [taxonomies](/api-reference/latest/taxonomies/taxonomy) and [taxonomy-labels](/api-reference/latest/taxonomies/taxonomy-label).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: taxonomies.readwrite\n  description: Create, update or delete [taxonomies](/api-reference/latest/taxonomies/taxonomy)\n    and [taxonomy-labels](/api-reference/latest/taxonomies/taxonomy-label).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n\
  - scope: webhook-deliveries.readonly\n  description: Read webhook-deliveries.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: webhook-deliveries.readwrite\n  description: Send a ping event to a webhook-endpoint.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: webhook-endpoints.readonly\n  description: Read webhook-endpoints.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: webhook-endpoints.readwrite\n  description: Create and update webhook-endpoints.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n- scope: working-time-arrangements.readonly\n  description: Read working-time-arrangements.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/lucca-api-2024-11-01.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/scopes/lucca-scopes.yml
summary_line: 36 scopes · clientCredentials
tags:
- Company
- Human Resources
- Software-as-a-Service
- Payroll
- Talent Management
token_bound: false
token_urls:
- https://accounts.world.luccasoftware.com/connect/token
---
