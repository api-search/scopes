---
api_specs:
- filename: growthspace-admin-api-openapi.yml
  format: yaml
  label: GrowthSpace Admin API
  slug: growthspace-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-admin-api-openapi.yml
- filename: growthspace-ah-api-openapi.yml
  format: yaml
  label: GrowthSpace Ah API
  slug: growthspace-ah-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-ah-api-openapi.yml
- filename: growthspace-growthspace-engineering-public-api-management-api-openapi.yml
  format: yaml
  label: GrowthSpace @growthspace Engineering/public Api Management API
  slug: growthspace-growthspace-engineering-public-api-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-growthspace-engineering-public-api-management-api-openapi.yml
- filename: growthspace-healthz-api-openapi.yml
  format: yaml
  label: GrowthSpace Healthz API
  slug: growthspace-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-healthz-api-openapi.yml
- filename: growthspace-public-api-openapi.yml
  format: yaml
  label: GrowthSpace Public API
  slug: growthspace-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-public-api-openapi.yml
- filename: growthspace-up-time-check-api-openapi.yml
  format: yaml
  label: GrowthSpace Up Time Check API
  slug: growthspace-up-time-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/openapi/growthspace-up-time-check-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Growthspace Scopes
name_suffix: OAuth Scopes
note: The Growthspace Public API scope catalogue is served anonymously (HTTP 200, application/json) by the Public API Management microservice at GET /admin/scopes. The scope names, labels, descriptions and READ/WRITE access class below are copied verbatim from that response on 2026-08-22. Growthspace publishes no developer portal or scopes reference page, so this live endpoint is the only public source for them.
overview: 'GrowthSpace publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the GrowthSpace API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GrowthSpace
provider_slug: growthspace
schemes:
- flows: []
  name: growthspace-public-api-app
  note: Applications are provisioned in the Growthspace admin console (Admin -> Public API), which issues a clientId + clientSecret pair and a bearer token via POST /admin/apps/{appId}/token; tokens are renewed through POST /public/refresh. The published OpenAPI declares no securitySchemes, so the grant details below are recorded from the management API surface and the admin console strings, not from a spec declaration.
  source: probe:/admin/scopes
scope_count: 11
scope_names:
- programs.read
- participants.read
- workshops.read
- company.read
- reporting.read
- integration.read
- programs.write
- participants.write
- workshops.write
- integration.write
- joker
scopes:
- description: Read programs, sessions, and program catalog
  flows: []
  scope: programs.read
- description: Read participants, employees, and skills
  flows: []
  scope: participants.read
- description: Read workshop events and management data
  flows: []
  scope: workshops.read
- description: Read company info, admins, and integrations
  flows: []
  scope: company.read
- description: Read reports, analytics, KPIs (read-only by design)
  flows: []
  scope: reporting.read
- description: 'Read access for integrations: participants, programs, company'
  flows: []
  scope: integration.read
- description: Create/update programs and run program sessions
  flows: []
  scope: programs.write
- description: Create/update participants and employees
  flows: []
  scope: participants.write
- description: Create/update workshops and workshop events
  flows: []
  scope: workshops.write
- description: 'Write access for integrations: participants and programs'
  flows: []
  scope: integration.write
- description: Global cross-company access — GS Admin only
  flows: []
  scope: joker
slug: growthspace-scopes
source_filename: growthspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/admin/scopes\nnote: >-\n  The Growthspace Public API scope catalogue is served anonymously (HTTP 200,\n  application/json) by the Public API Management microservice at\n  GET /admin/scopes. The scope names, labels, descriptions and READ/WRITE access\n  class below are copied verbatim from that response on 2026-08-22. Growthspace\n  publishes no developer portal or scopes reference page, so this live endpoint\n  is the only public source for them.\ndocs: null\nschemes:\n- name: growthspace-public-api-app\n  source: probe:/admin/scopes\n  note: >-\n    Applications are provisioned in the Growthspace admin console (Admin ->\n    Public API), which issues a clientId + clientSecret pair and a bearer token\n    via POST /admin/apps/{appId}/token; tokens are renewed through\n    POST /public/refresh. The published OpenAPI declares no securitySchemes, so\n    the grant\
  \ details below are recorded from the management API surface and the\n    admin console strings, not from a spec declaration.\n  flows: []\nscope_count: 11\nscopes:\n- scope: programs.read\n  label: Programs\n  access: READ\n  description: Read programs, sessions, and program catalog\n- scope: participants.read\n  label: Participants\n  access: READ\n  description: Read participants, employees, and skills\n- scope: workshops.read\n  label: Workshops\n  access: READ\n  description: Read workshop events and management data\n- scope: company.read\n  label: Company\n  access: READ\n  description: Read company info, admins, and integrations\n- scope: reporting.read\n  label: Reporting\n  access: READ\n  description: Read reports, analytics, KPIs (read-only by design)\n- scope: integration.read\n  label: Integration\n  access: READ\n  description: 'Read access for integrations: participants, programs, company'\n- scope: programs.write\n  label: Programs\n  access: WRITE\n  description: Create/update\
  \ programs and run program sessions\n- scope: participants.write\n  label: Participants\n  access: WRITE\n  description: Create/update participants and employees\n- scope: workshops.write\n  label: Workshops\n  access: WRITE\n  description: Create/update workshops and workshop events\n- scope: integration.write\n  label: Integration\n  access: WRITE\n  description: 'Write access for integrations: participants and programs'\n- scope: joker\n  label: Joker (Cross-Company)\n  access: null\n  is_joker: true\n  description: \"Global cross-company access — GS Admin only\"\nx-evidence:\n- url: https://public-api-management-dot-growthspace-246311.oa.r.appspot.com/admin/scopes\n  http_status: 200\n  content_type: application/json; charset=utf-8\n  fetched: '2026-08-22'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthspace/refs/heads/main/scopes/growthspace-scopes.yml
summary_line: 11 scopes
tags:
- Company
- Learning and Development
- Talent Development
- Human Resources
- Coaching
- Employee Experience
- Skills
- Workforce
- Enterprise Software
- Artificial Intelligence
token_urls: []
---
