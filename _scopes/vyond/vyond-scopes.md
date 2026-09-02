---
api_specs:
- filename: vyond-content-generation-api-openapi.yml
  format: yaml
  label: Vyond Content Generation API
  slug: vyond-content-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-content-generation-api-openapi.yml
- filename: vyond-parameter-api-openapi.yml
  format: yaml
  label: Vyond Parameter API
  slug: vyond-parameter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-parameter-api-openapi.yml
- filename: vyond-scim-api-openapi.yml
  format: yaml
  label: Vyond SCIM API
  slug: vyond-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-scim-api-openapi.yml
- filename: vyond-turbo-api-openapi.yml
  format: yaml
  label: Vyond Turbo API
  slug: vyond-turbo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-turbo-api-openapi.yml
- filename: vyond-user-api-openapi.yml
  format: yaml
  label: Vyond User API
  slug: vyond-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-user-api-openapi.yml
- filename: vyond-video-api-openapi.yml
  format: yaml
  label: Vyond Video API
  slug: vyond-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-video-api-openapi.yml
- filename: vyond-video-export-api-openapi.yml
  format: yaml
  label: Vyond Video Export API
  slug: vyond-video-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-video-export-api-openapi.yml
- filename: vyond-webhook-api-openapi.yml
  format: yaml
  label: Vyond Webhook API
  slug: vyond-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/openapi/vyond-webhook-api-openapi.yml
authorization_urls: []
description: ''
docs: https://api.vyond.com/doc/#tag/Introduction
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Vyond Scopes
name_suffix: OAuth Scopes
note: Vyond documents OAuth 2.0 access tokens for its REST API but does NOT declare an oauth2 securityScheme in the OpenAPI — the only scheme in components is `bearer` (http/bearer). The scope names below are therefore not machine-readable from the flows map; they are named explicitly in the 403 response descriptions of the operations that require them, which is the only place Vyond publishes them. There is no published scope-reference page, no authorization/token URL, and no /.well-known/oauth-authorization-server (probed 2026-08-05, 404). Recorded here so the gap is legible rather than absent.
overview: 'Vyond publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vyond API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vyond
provider_slug: vyond
schemes:
- applies_to: both the REST API and the SCIM 2.0 API
  name: bearer
  scheme: bearer
  source: openapi/vyond-openapi-original.json
  token_types:
  - docs: https://help.vyond.com/hc/en-us/articles/32250964864660-SCIM-Provisioning
    issued_at: Vyond app > Security > SCIM Provisioning > Authorization token
    name: API token
    surface: SCIM 2.0 (https://api.vyond.com/scim/v2/)
  - docs: https://help.vyond.com/hc/en-us/articles/51873650828052-How-do-I-use-the-Vyond-API
    issued_at: Vyond app > profile icon > API tokens > Personal Access token
    name: Personal Access Token
    note: Help Center states the API token page is currently hidden and access must be requested from support@vyond.com.
    surface: REST (https://api.vyond.com/rest/)
  - name: OAuth 2.0 access token
    note: Documented in the Introduction as short-lived and refresh-token renewable. No authorization endpoint, token endpoint, grant type or discovery document is published. Vyond states "Vyond will soon support API tokens in REST API authentication."
    surface: REST (https://api.vyond.com/rest/)
  type: http
scope_count: 2
scope_names:
- VYOND_GO
- VIDEO_EXPORT
scopes:
- description: Required to create Vyond Go content generations. Absence returns 403 "Forbidden - missing required VYOND_GO scope or invalid owner type".
  flows: []
  scope: VYOND_GO
- description: Required to create a video export and to retrieve the resulting download URL. Absence returns 403 "Forbidden - missing required VIDEO_EXPORT scope or access denied".
  flows: []
  scope: VIDEO_EXPORT
slug: vyond-scopes
source_filename: vyond-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://api.vyond.com/doc/\ndocs: https://api.vyond.com/doc/#tag/Introduction\nnote: >-\n  Vyond documents OAuth 2.0 access tokens for its REST API but does NOT declare an\n  oauth2 securityScheme in the OpenAPI — the only scheme in components is\n  `bearer` (http/bearer). The scope names below are therefore not machine-readable\n  from the flows map; they are named explicitly in the 403 response descriptions of\n  the operations that require them, which is the only place Vyond publishes them.\n  There is no published scope-reference page, no authorization/token URL, and no\n  /.well-known/oauth-authorization-server (probed 2026-08-05, 404). Recorded here\n  so the gap is legible rather than absent.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  source: openapi/vyond-openapi-original.json\n  applies_to: both the REST API and the SCIM 2.0 API\n  token_types:\n  - name: API token\n    surface: SCIM 2.0 (https://api.vyond.com/scim/v2/)\n\
  \    issued_at: Vyond app > Security > SCIM Provisioning > Authorization token\n    docs: https://help.vyond.com/hc/en-us/articles/32250964864660-SCIM-Provisioning\n  - name: Personal Access Token\n    surface: REST (https://api.vyond.com/rest/)\n    issued_at: Vyond app > profile icon > API tokens > Personal Access token\n    docs: https://help.vyond.com/hc/en-us/articles/51873650828052-How-do-I-use-the-Vyond-API\n    note: >-\n      Help Center states the API token page is currently hidden and access must be\n      requested from support@vyond.com.\n  - name: OAuth 2.0 access token\n    surface: REST (https://api.vyond.com/rest/)\n    note: >-\n      Documented in the Introduction as short-lived and refresh-token renewable.\n      No authorization endpoint, token endpoint, grant type or discovery document is\n      published. Vyond states \"Vyond will soon support API tokens in REST API\n      authentication.\"\nscopes:\n- scope: VYOND_GO\n  description: >-\n    Required to create Vyond\
  \ Go content generations. Absence returns 403\n    \"Forbidden - missing required VYOND_GO scope or invalid owner type\".\n  sources: [openapi/vyond-openapi-original.json]\n  operations:\n  - ContentGenerationController.createGeneration\n- scope: VIDEO_EXPORT\n  description: >-\n    Required to create a video export and to retrieve the resulting download URL.\n    Absence returns 403 \"Forbidden - missing required VIDEO_EXPORT scope or access\n    denied\".\n  sources: [openapi/vyond-openapi-original.json]\n  operations:\n  - VideoController.exportVideo\n  - VideoController.getVideoExportDownload\nunnamed_scope_requirements:\n- operations:\n  - ContentGenerationV2Controller.createGeneration\n  - ParameterController.getParameters\n  - TurboController.createTurbo\n  - TurboController.getTurbo\n  note: >-\n    These operations return 403 \"missing required scope\" but the scope name is not\n    published in the documentation. TurboController additionally requires a Turbo\n    license on the\
  \ account.\nowner_type_constraint: >-\n  Several operations (getUser, all webhook management, content generation v2 read)\n  return 403 \"invalid owner type (non-user token)\" — the token must be a user-owned\n  token, not an account/service token. This is an authorization dimension separate\n  from scope.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://api.vyond.com/doc/openapi.json\n  http_status: 200\n  probed_absent:\n  - {url: 'https://api.vyond.com/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://api.vyond.com/.well-known/openid-configuration', status: 404}\n  - {url: 'https://api.vyond.com/oauth/token', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vyond/refs/heads/main/scopes/vyond-scopes.yml
summary_line: 2 scopes
tags:
- Video
- Animation
- Video Generation
- Artificial Intelligence
- E-Learning
- Learning and Development
- Content Generation
- SCIM
- Identity Provisioning
- Webhook
- Enterprise
- Media
token_urls: []
---
