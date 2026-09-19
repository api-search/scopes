---
api_specs:
- filename: workday-advanced-compensation-compensation-rest-v3-openapi.json
  format: json
  label: Workday Compensation REST API v3
  slug: workday-compensation-rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-compensation-rest-v3-openapi.json
- filename: workday-advanced-compensation-bonus-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Bonus Plans API
  slug: workday-advanced-compensation-bonus-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-bonus-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-budgets-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Budgets API
  slug: workday-advanced-compensation-compensation-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-budgets-api-openapi.yml
- filename: workday-advanced-compensation-compensation-grades-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Grades API
  slug: workday-advanced-compensation-compensation-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-grades-api-openapi.yml
- filename: workday-advanced-compensation-compensation-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Plans API
  slug: workday-advanced-compensation-compensation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-reviews-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Reviews API
  slug: workday-advanced-compensation-compensation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-reviews-api-openapi.yml
- filename: workday-advanced-compensation-employee-compensation-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Employee Compensation API
  slug: workday-advanced-compensation-employee-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-employee-compensation-api-openapi.yml
- filename: workday-advanced-compensation-merit-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Merit Plans API
  slug: workday-advanced-compensation-merit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-merit-plans-api-openapi.yml
- filename: workday-advanced-compensation-stock-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Stock Plans API
  slug: workday-advanced-compensation-stock-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-stock-plans-api-openapi.yml
authorization_urls:
- https://<tenantAuthorizationHostname>
description: ''
docs: https://developer.workday.com/doc/axp1537909839739.md
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Workday Advanced Compensation Scopes
name_suffix: OAuth Scopes
note: 'Workday REST authorization is scoped by named FUNCTIONAL AREAS (Workday calls them "Scopes") combined with a security DOMAIN that the Integration System User or API Client must be granted. Every operation description in Workday''s published compensation OpenAPI names both, e.g. "Secured By Domain: Set Up: Merit and Bonus" / "Scope: Advanced Compensation". These are the real scope strings an API Client is registered with in Workday; they are NOT OAuth scope tokens in the flows[].scopes map, which Workday publishes empty.'
overview: 'Workday Advanced Compensation publishes 3 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Advanced Compensation API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Advanced Compensation
provider_slug: workday-advanced-compensation
schemes:
- description: Workday OAuth 2.0. The published specs declare the implicit flow with a templated tenant authorization host; Workday's own docs document Authorization Code and Client Credentials (Integration System User) grants for server-to-server integrations.
  docs:
  - https://developer.workday.com/doc/jzx1537909761291.md
  - https://developer.workday.com/doc/axp1537909839739.md
  flows:
  - authorizationUrl: https://<tenantAuthorizationHostname>
    flow: implicit
  name: OAuth2
  source: openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json
scope_count: 3
scope_names:
- Advanced Compensation
- Core Compensation
- Staffing
scopes:
- description: Workday functional-area scope covering compensation scorecards, scorecard results and merit/bonus setup. Named on 20 of the 26 operations in the published compensation v1-v3 specs.
  flows: []
  scope: Advanced Compensation
- description: Workday functional-area scope covering one-time payment requests against a worker.
  flows: []
  scope: Core Compensation
- description: Workday functional-area scope covering the worker read surface the compensation service exposes (/workers, /workers/{ID}).
  flows: []
  scope: Staffing
slug: workday-advanced-compensation-scopes
source_filename: workday-advanced-compensation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\ndocs: https://developer.workday.com/doc/axp1537909839739.md\nnote: >-\n  Workday REST authorization is scoped by named FUNCTIONAL AREAS (Workday calls them \"Scopes\")\n  combined with a security DOMAIN that the Integration System User or API Client must be granted.\n  Every operation description in Workday's published compensation OpenAPI names both, e.g.\n  \"Secured By Domain: Set Up: Merit and Bonus\" / \"Scope: Advanced Compensation\". These are the\n  real scope strings an API Client is registered with in Workday; they are NOT OAuth scope tokens\n  in the flows[].scopes map, which Workday publishes empty.\nschemes:\n- name: OAuth2\n  source: openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://<tenantAuthorizationHostname>\n  description: >-\n    Workday OAuth\
  \ 2.0. The published specs declare the implicit flow with a templated tenant\n    authorization host; Workday's own docs document Authorization Code and Client Credentials\n    (Integration System User) grants for server-to-server integrations.\n  docs:\n  - https://developer.workday.com/doc/jzx1537909761291.md\n  - https://developer.workday.com/doc/axp1537909839739.md\nscopes:\n- scope: Advanced Compensation\n  description: >-\n    Workday functional-area scope covering compensation scorecards, scorecard results and\n    merit/bonus setup. Named on 20 of the 26 operations in the published compensation v1-v3 specs.\n  secured_by_domain: 'Set Up: Merit and Bonus'\n  operations: 20\n  sources:\n  - openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\n- scope: Core Compensation\n  description: >-\n    Workday functional-area scope covering one-time payment requests against a worker.\n  operations: 3\n  sources:\n  - openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\n\
  - scope: Staffing\n  description: >-\n    Workday functional-area scope covering the worker read surface the compensation service\n    exposes (/workers, /workers/{ID}).\n  secured_by_domain: >-\n    FLW Service, Self-Service: Current Staffing Information, Worker Data: Public Worker Reports\n  operations: 6\n  sources:\n  - openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/scopes/workday-advanced-compensation-scopes.yml
summary_line: 3 scopes · implicit
tags:
- Compensation
- Human Resources
- Payroll
- HCM
- Enterprise Software
- Total Rewards
- Bonus
- Merit
- Stock Compensation
- SOAP
- Software-as-a-Service
token_urls: []
---
