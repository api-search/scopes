---
api_specs:
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Approvals API
  slug: workday-business-processes-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Business Process Definitions API
  slug: workday-business-processes-business-process-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Inbox Items API
  slug: workday-business-processes-inbox-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-business-process-openapi.yml
  format: yaml
  label: Workday Business Processes Process Instances API
  slug: workday-business-processes-process-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-business-process-openapi.yml
- filename: workday-business-processes-custom-business-process-config-openapi.yml
  format: yaml
  label: Workday Custom Business Process Config API
  slug: workday-business-processes-custom-business-process-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/openapi/workday-business-processes-custom-business-process-config-openapi.yml
authorization_urls:
- https://{tenantAuthorizationHostname}/authorize
- https://auth.api.workday.com/v1/authorize
description: ''
docs: https://developer.workday.com/doc/zwx1518028675482.md
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Workday Business Processes Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Workday Business Processes publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Workday Business Processes API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Workday Business Processes
provider_slug: workday-business-processes
schemes:
- declared_scopes: 0
  flows:
  - authorizationUrl: https://{tenantAuthorizationHostname}/authorize
    flow: implicit
    note: published as the literal <tenantAuthorizationHostname>; per-tenant
  name: OAuth2
  note: The businessProcess v1 spec declares an EMPTY scopes map. The real scope requirement is in each operation description — captured in operation_scopes[] below.
  source: openapi/workday-business-processes-business-process-openapi.yml
  type: oauth2
- declared_scopes: 2
  description: Register an API Client
  flows:
  - authorizationUrl: https://auth.api.workday.com/v1/authorize
    flow: implicit
  name: oAuth2
  source: openapi/workday-business-processes-custom-business-process-config-openapi.yml
  type: oauth2
scope_count: 2
scope_names:
- read
- write
scopes:
- description: read custom business process types
  flows:
  - implicit
  scope: read
- description: modify custom business process types
  flows:
  - implicit
  scope: write
slug: workday-business-processes-scopes
source_filename: workday-business-processes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/_original/workday-business-processes-business-process-v1-openapi.json + openapi/_original/workday-business-processes-custom-business-process-config-v1-openapi.json\ndocs: https://developer.workday.com/doc/zwx1518028675482.md\ndocs_note: Workday REST authorization is TWO-LAYERED and neither layer alone is enough. (1) OAuth scopes are selected when an API\n  client is registered in the Developer Site Console; Workday calls them \"scopes\" but they are FUNCTIONAL AREAS, not the fine-grained\n  read:x/write:x scopes most APIs publish, and the scope a given endpoint needs is stated in the endpoint description in the REST\n  API Explorer rather than in a scopes reference page. (2) The tenant business process security policy still governs whether the\n  authenticated security group may take the action. An agent holding a valid token can still be refused by policy.\nschemes:\n- name: OAuth2\n  source: openapi/workday-business-processes-business-process-openapi.yml\n\
  \  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://{tenantAuthorizationHostname}/authorize\n    note: published as the literal <tenantAuthorizationHostname>; per-tenant\n  declared_scopes: 0\n  note: The businessProcess v1 spec declares an EMPTY scopes map. The real scope requirement is in each operation description —\n    captured in operation_scopes[] below.\n- name: oAuth2\n  source: openapi/workday-business-processes-custom-business-process-config-openapi.yml\n  type: oauth2\n  description: Register an API Client\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.api.workday.com/v1/authorize\n  declared_scopes: 2\ndocumented_flows:\n- flow: authorizationCode\n  docs: https://developer.workday.com/doc/jzx1537909761291.md\n- flow: clientCredentials\n  docs: https://developer.workday.com/doc/axp1537909839739.md\n- flow: refreshToken\n  docs: https://developer.workday.com/doc/cqa1553122177664.md\nscopes:\n- scope: read\n  description: read custom\
  \ business process types\n  flows:\n  - implicit\n  sources:\n  - openapi/workday-business-processes-custom-business-process-config-openapi.yml\n- scope: write\n  description: modify custom business process types\n  flows:\n  - implicit\n  sources:\n  - openapi/workday-business-processes-custom-business-process-config-openapi.yml\nfunctional_area_scopes:\n- Adaptive Planning for Financial Plans\n- Adaptive Planning for the Workforce\n- Benefits\n- Tenant Non-Configurable\noperation_scopes:\n- operation: GET /types\n  functional_areas:\n  - Tenant Non-Configurable\n- operation: GET /types/{ID}\n  functional_areas:\n  - Tenant Non-Configurable\n- operation: GET /types/{ID}/attachmentCategories\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /eventSteps\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n\
  \  - Tenant Non-Configurable\n- operation: POST /eventSteps/{ID}/questionnaire\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST /eventSteps/{ID}/reassign\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST /eventSteps/{ID}/deny\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /eventSteps/{ID}\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST /eventSteps/{ID}/toDo\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST\
  \ /eventSteps/{ID}/approve\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST /eventSteps/{ID}/sendBack\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events/{ID}/remainingSteps\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST /events/{ID}/rescind\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events/{ID}/comments\n  functional_areas:\n  - Adaptive Planning\
  \ for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events/{ID}\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events/{ID}/inProgressSteps\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: POST /events/{ID}/cancel\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events/{ID}/attachments\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n  - Benefits\n  - Tenant Non-Configurable\n- operation: GET /events/{ID}/completedSteps\n  functional_areas:\n  - Adaptive Planning for Financial Plans\n  - Adaptive Planning for the Workforce\n\
  \  - Benefits\n  - Tenant Non-Configurable\ngap:\n  scopes_reference_page: false\n  note: Workday publishes no scopes/permissions reference page for REST. The only machine-readable statement of scope per operation\n    is the \"Scope:\" line embedded in each operation description, extracted above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-business-processes/refs/heads/main/scopes/workday-business-processes-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Business Processes
- Workflows
- Approvals
- Human Resources
- Enterprise
- Software-as-a-Service
- HCM
- Financial Management
- Process Automation
- Event Steps
- SOAP
- GraphQL
token_urls: []
---
