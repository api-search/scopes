---
authorization_urls: []
description: ''
docs: https://cloud.trisotech.com/help/admin/client-apps.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Trisotech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trisotech publishes 20 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trisotech API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trisotech
provider_slug: trisotech
schemes: []
scope_count: 20
scope_names:
- repo_r
- repo_w
- service_x
- group_r
- group_w
- graph_r
- users_r
- users_w
- admin
- mvn_r
- mvn_w
- mvn_d
- emitter_r
- emitter_w
- bpmn_x
- cmmn_x
- dmn_x
- docker_r
- asset_w
- openid
scopes:
- description: Read modeling places.
  flows: []
  scope: repo_r
- description: Write, delete, rename and create models in modeling places.
  flows: []
  scope: repo_w
- description: Deprecated scope that was used to transform model types.
  flows: []
  scope: service_x
- description: Read groups.
  flows: []
  scope: group_r
- description: Write, delete, rename and invite to groups.
  flows: []
  scope: group_w
- description: Use the SPARQL API on the Digital Enterprise Graph.
  flows: []
  scope: graph_r
- description: Read users.
  flows: []
  scope: users_r
- description: Write and delete users.
  flows: []
  scope: users_w
- description: The admin API is not documented for customers and this scope should not be used.
  flows: []
  scope: admin
- description: Query the execution environments and their content.
  flows: []
  scope: mvn_r
- description: Publish and delete services in execution environments.
  flows: []
  scope: mvn_w
- description: Download services from execution environments.
  flows: []
  scope: mvn_d
- description: Read emitter configuration and audit log files.
  flows: []
  scope: emitter_r
- description: Write emitter configuration.
  flows: []
  scope: emitter_w
- description: Access the workflow automation API.
  flows: []
  scope: bpmn_x
- description: Access the case automation API.
  flows: []
  scope: cmmn_x
- description: Access the decision automation API.
  flows: []
  scope: dmn_x
- description: Download containers built locally.
  flows: []
  scope: docker_r
- description: Write to the static assets resource.
  flows: []
  scope: asset_w
- description: Can be used by Digital Distributed Containers to obtain an OpenID token identity.
  flows: []
  scope: openid
slug: trisotech-scopes
source_filename: trisotech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://cloud.trisotech.com/help/admin/client-apps.html\ndocs: https://cloud.trisotech.com/help/admin/client-apps.html\nname: Trisotech Digital Enterprise Suite OAuth 2 Scopes\nsummary: >-\n  Trisotech publishes the complete grant/scope reference for Client Apps in the\n  Digital Enterprise Suite administration documentation. Scopes are attached to a\n  Client App as \"grants\" and inherited by every bearer token the app issues.\n  Transcribed verbatim from the provider's own table; no scope was inferred.\nflows:\n  authorization_code:\n    authorizationUrl: https://{instance}.trisotech.com/oauth2/auth\n    tokenUrl: https://{instance}.trisotech.com/oauth2/token\n    pkce: supported\n  client_credentials:\n    tokenUrl: https://{instance}.trisotech.com/oauth2/token\n    note: >-\n      Enabled per Client App via the \"Support Client Credentials\" flag; the app's\n      Associated System Account supplies the identity used in\
  \ access checks.\nscope_count: 20\nscopes:\n  - scope: repo_r\n    name: Repository read\n    description: Read modeling places.\n  - scope: repo_w\n    name: Repository write\n    description: Write, delete, rename and create models in modeling places.\n  - scope: service_x\n    name: Service execution\n    description: Deprecated scope that was used to transform model types.\n    deprecated: true\n  - scope: group_r\n    name: Group read\n    description: Read groups.\n  - scope: group_w\n    name: Group write\n    description: Write, delete, rename and invite to groups.\n  - scope: graph_r\n    name: Graph read\n    description: Use the SPARQL API on the Digital Enterprise Graph.\n  - scope: users_r\n    name: Users read\n    description: Read users.\n  - scope: users_w\n    name: Users write\n    description: Write and delete users.\n  - scope: admin\n    name: Admin\n    description: >-\n      The admin API is not documented for customers and this scope should not be used.\n    note:\
  \ Provider explicitly discourages use.\n  - scope: mvn_r\n    name: Execution environment read\n    description: Query the execution environments and their content.\n  - scope: mvn_w\n    name: Execution environment write\n    description: Publish and delete services in execution environments.\n  - scope: mvn_d\n    name: Execution environment download\n    description: Download services from execution environments.\n  - scope: emitter_r\n    name: Emitter read\n    description: Read emitter configuration and audit log files.\n  - scope: emitter_w\n    name: Emitter write\n    description: Write emitter configuration.\n  - scope: bpmn_x\n    name: BPMN execution\n    description: Access the workflow automation API.\n  - scope: cmmn_x\n    name: CMMN execution\n    description: Access the case automation API.\n  - scope: dmn_x\n    name: DMN execution\n    description: Access the decision automation API.\n  - scope: docker_r\n    name: Docker read\n    description: Download containers built\
  \ locally.\n  - scope: asset_w\n    name: Assets write\n    description: Write to the static assets resource.\n  - scope: openid\n    name: OpenID\n    description: >-\n      Can be used by Digital Distributed Containers to obtain an OpenID token identity.\nnotes:\n  - >-\n    20 grants are published. One (service_x) is marked deprecated by the provider and\n    one (openid) is an identity grant rather than an API access scope; both are kept\n    in the list and flagged rather than dropped.\n  - >-\n    Scopes are granted at the Client App level in the Administration application,\n    not requested per-authorization-request in the docs shown.\nevidence:\n  - url: https://cloud.trisotech.com/help/admin/client-apps.html\n    status: 200\n  - url: https://cloud.trisotech.com/oauth2/token\n    status: 405\n    note: GET rejected with \"HTTP method GET is not supported by this URL\" — endpoint is live and POST-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trisotech/refs/heads/main/scopes/trisotech-scopes.yml
summary_line: 20 scopes
tags:
- Business Process Management
- Decision Management
- Workflow Automation
- Low Code
- BPMN
- DMN
- CMMN
- Healthcare
- FHIR
- Clinical Decision Support
- Standards
- AI Agents
- Model Context Protocol
- Enterprise Architecture
token_urls: []
---
