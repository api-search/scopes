---
api_specs:
- filename: riot-awareness-api-openapi.yml
  format: yaml
  label: Riot Awareness API
  slug: riot-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-awareness-api-openapi.yml
- filename: riot-breaches-api-openapi.yml
  format: yaml
  label: Riot Breaches API
  slug: riot-breaches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-breaches-api-openapi.yml
- filename: riot-general-api-openapi.yml
  format: yaml
  label: Riot General API
  slug: riot-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-general-api-openapi.yml
- filename: riot-groups-api-openapi.yml
  format: yaml
  label: Riot Groups API
  slug: riot-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-groups-api-openapi.yml
- filename: riot-inbox-api-openapi.yml
  format: yaml
  label: Riot Inbox API
  slug: riot-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-inbox-api-openapi.yml
- filename: riot-scim-api-openapi.yml
  format: yaml
  label: Riot SCIM API
  slug: riot-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-scim-api-openapi.yml
- filename: riot-simulation-api-openapi.yml
  format: yaml
  label: Riot Simulation API
  slug: riot-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-simulation-api-openapi.yml
- filename: riot-slash-api-openapi.yml
  format: yaml
  label: Riot Slash API
  slug: riot-slash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-slash-api-openapi.yml
- filename: riot-sonar-api-openapi.yml
  format: yaml
  label: Riot Sonar API
  slug: riot-sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-sonar-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.tryriot.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Riot Scopes
name_suffix: OAuth Scopes
note: Riot does NOT use OAuth 2.0. This artifact records the API-key scope model the provider documents in the OpenAPI `info.description` under "Authorization". Scopes are attached to an `x-api-key` credential, not granted through an authorization flow, so there are no authorization/token endpoints and no consent step. The `components.securitySchemes.apiKeyAuth` object declares no scopes, and no operation declares a `security[]` scope requirement — the scope names below come from the prose reference only, which is why the scope-to-operation binding is recorded as not-published.
overview: 'Riot publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Riot API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Riot
provider_slug: riot
schemes:
- flows: []
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  source: openapi/riot-public-api-openapi.yml
  type: apiKey
scope_count: 4
scope_names:
- awareness:read
- simulation:read
- breach:read
- workspace:read
scopes:
- description: Read access to the awareness surface — courses, course settings and employee learning progress.
  flows: []
  scope: awareness:read
- description: Read access to the phishing simulation surface — campaigns, attacks, attack events and login domains.
  flows: []
  scope: simulation:read
- description: Read access to credential breach data and compromised employees.
  flows: []
  scope: breach:read
- description: Read access to organization and workspace metadata, employees, groups and domains.
  flows: []
  scope: workspace:read
slug: riot-scopes
source_filename: riot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://public-api.tryriot.com/openapi\ndocs: https://docs.tryriot.com/\nmodel: api-key-scopes\nnote: >-\n  Riot does NOT use OAuth 2.0. This artifact records the API-key scope model the provider documents in the\n  OpenAPI `info.description` under \"Authorization\". Scopes are attached to an `x-api-key` credential, not\n  granted through an authorization flow, so there are no authorization/token endpoints and no consent step.\n  The `components.securitySchemes.apiKeyAuth` object declares no scopes, and no operation declares a\n  `security[]` scope requirement — the scope names below come from the prose reference only, which is why\n  the scope-to-operation binding is recorded as not-published.\nkey_scoping:\n  levels:\n  - level: organization\n    description: >-\n      Organization-scoped keys can access any workspace belonging to the organization. Endpoints that take a\n      `workspace_id` parameter accept any workspace\
  \ of that organization.\n  - level: workspace\n    description: >-\n      Workspace-scoped keys are restricted to a single workspace. Requests targeting a different workspace\n      through a `workspace_id` parameter are rejected with a 403 status code.\n  enforcement_status: 403\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  source: openapi/riot-public-api-openapi.yml\n  flows: []\nscopes:\n- scope: awareness:read\n  description: Read access to the awareness surface — courses, course settings and employee learning progress.\n  likely_operations:\n  - courses_get_paginated_DJESCNQ\n  - courses_get_statistics_DJESCNQ\n  - courses_get_employees_progress_DJESCNQ\n  - courses_get_course_statuses_of_employees_DJESCNQ\n  binding: inferred-from-tag\n  confidence: medium\n  sources:\n  - https://public-api.tryriot.com/openapi\n- scope: simulation:read\n  description: Read access to the phishing simulation surface — campaigns, attacks, attack events and login\
  \ domains.\n  likely_operations:\n  - campaigns_get_paginated_CWCTX3I\n  - campaigns_get_statistics_CWCTX3I\n  - attacks_get_paginated_KCLEOEQ\n  - attack_login_domains_get_attack_login_domain_paginated_XU5W4YI\n  binding: inferred-from-tag\n  confidence: medium\n  sources:\n  - https://public-api.tryriot.com/openapi\n- scope: breach:read\n  description: Read access to credential breach data and compromised employees.\n  likely_operations:\n  - breaches_get_paginated_FAUE35Y\n  - breaches_get_statistics_FAUE35Y\n  - breaches_get_breach_compromised_employees_FAUE35Y\n  binding: inferred-from-tag\n  confidence: medium\n  sources:\n  - https://public-api.tryriot.com/openapi\n- scope: workspace:read\n  description: Read access to organization and workspace metadata, employees, groups and domains.\n  likely_operations:\n  - organizations_get_XEBQFJQ\n  - employees_get_paginated_LRY7OLI\n  - employees_get_LRY7OLI\n  - employees_get_statistics_LRY7OLI\n  - groups_get_paginated_BOILCUA\n  - groups_get_group_employees_BOILCUA\n\
  \  - domains_get_paginated_domains_OOWLIAA\n  binding: inferred-from-tag\n  confidence: medium\n  sources:\n  - https://public-api.tryriot.com/openapi\ngaps:\n- >-\n  The documented scope list is introduced with \"such as\", so it may not be exhaustive. No scope is published\n  for the Inbox/Slash endpoints or for the SCIM 2.0 provisioning surface.\n- >-\n  No per-operation `security[]` scope requirements appear in the OpenAPI, so an agent cannot compute the\n  minimum scope set for a call from the machine-readable contract alone.\n- API keys are not self-service — the docs state customers must contact the technical team to acquire one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/scopes/riot-scopes.yml
summary_line: 4 scopes
tags:
- Cybersecurity
- Security Awareness
- Human Risk Management
- Phishing Simulation
- employee-security
- Security Posture Management
- breach-detection
- Email Security
- SaaS Security
- SCIM
- Webhook
- OCSF
- France
token_urls: []
---
