---
api_specs:
- filename: authenticx-agent-api-openapi.yml
  format: yaml
  label: Authenticx Agent API
  slug: authenticx-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-agent-api-openapi.yml
- filename: authenticx-conversations-api-openapi.yml
  format: yaml
  label: Authenticx Conversations API
  slug: authenticx-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-conversations-api-openapi.yml
- filename: authenticx-evaluations-api-openapi.yml
  format: yaml
  label: Authenticx Evaluations API
  slug: authenticx-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-evaluations-api-openapi.yml
- filename: authenticx-hierarchy-api-openapi.yml
  format: yaml
  label: Authenticx Hierarchy API
  slug: authenticx-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-hierarchy-api-openapi.yml
- filename: authenticx-interactions-api-openapi.yml
  format: yaml
  label: Authenticx Interactions API
  slug: authenticx-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-interactions-api-openapi.yml
- filename: authenticx-media-api-openapi.yml
  format: yaml
  label: Authenticx Media API
  slug: authenticx-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-media-api-openapi.yml
- filename: authenticx-metadata-api-openapi.yml
  format: yaml
  label: Authenticx Metadata API
  slug: authenticx-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-metadata-api-openapi.yml
- filename: authenticx-modelresults-api-openapi.yml
  format: yaml
  label: Authenticx Model Results API
  slug: authenticx-modelresults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-modelresults-api-openapi.yml
- filename: authenticx-receipts-api-openapi.yml
  format: yaml
  label: Authenticx Receipts API
  slug: authenticx-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-receipts-api-openapi.yml
- filename: authenticx-roles-api-openapi.yml
  format: yaml
  label: Authenticx Roles API
  slug: authenticx-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-roles-api-openapi.yml
- filename: authenticx-scim-resourcetypes-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) ResourceTypes API
  slug: authenticx-scim-resourcetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-resourcetypes-api-openapi.yml
- filename: authenticx-scim-schemas-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) Schemas API
  slug: authenticx-scim-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-schemas-api-openapi.yml
- filename: authenticx-scim-serviceproviderconfig-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) ServiceProviderConfig API
  slug: authenticx-scim-serviceproviderconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-serviceproviderconfig-api-openapi.yml
- filename: authenticx-scim-users-api-openapi.yml
  format: yaml
  label: Authenticx (Scim) Users API
  slug: authenticx-scim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-scim-users-api-openapi.yml
- filename: authenticx-textmedia-api-openapi.yml
  format: yaml
  label: Authenticx Text Media API
  slug: authenticx-textmedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-textmedia-api-openapi.yml
- filename: authenticx-user-api-openapi.yml
  format: yaml
  label: Authenticx User API
  slug: authenticx-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-user-api-openapi.yml
- filename: authenticx-userhierarchy-api-openapi.yml
  format: yaml
  label: Authenticx User Hierarchy API
  slug: authenticx-userhierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-userhierarchy-api-openapi.yml
- filename: authenticx-workflows-api-openapi.yml
  format: yaml
  label: Authenticx Workflows API
  slug: authenticx-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/openapi/authenticx-workflows-api-openapi.yml
authorization_urls: []
description: ''
docs: https://authenticx.readme.io/reference/retrieving-an-access-token
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Authenticx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Authenticx publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Authenticx API on a user''s behalf.


  Tokens are issued from https://api.beauthenticx.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Authenticx
provider_slug: authenticx
schemes:
- flows:
  - flow: clientCredentials
    staging_tokenUrl: https://api.authcx.com/connect/token
    tokenUrl: https://api.beauthenticx.com/connect/token
  name: OAuth2
  source: openapi/authenticx-acxapi-openapi.yml
scope_count: 1
scope_names:
- acxapi
scopes:
- description: Access to Acx API
  flows:
  - clientCredentials
  scope: acxapi
slug: authenticx-scopes
source_filename: authenticx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/authenticx-acxapi-openapi.yml\ndocs: https://authenticx.readme.io/reference/retrieving-an-access-token\ndiscovery: https://api.beauthenticx.com/.well-known/openid-configuration\nschemes:\n- name: OAuth2\n  source: openapi/authenticx-acxapi-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.beauthenticx.com/connect/token\n    staging_tokenUrl: https://api.authcx.com/connect/token\nscopes:\n- scope: acxapi\n  description: Access to Acx API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/authenticx-acxapi-openapi.yml\n  - https://authenticx.readme.io/reference/retrieving-an-access-token\n  - https://api.beauthenticx.com/.well-known/openid-configuration\n  note: >-\n    The one scope AcxAPI integrators request. It is coarse-grained — a single scope grants the whole API\n    surface, including SCIM 2.0 user provisioning and role/hierarchy administration. Per-resource authorization\n \
  \   is enforced by the organization's hierarchy and role model (GET /Roles/All, GET /UserHierarchy/...), not by\n    OAuth scope.\nscopes_advertised_by_provider_not_used_by_acxapi:\n- scope: openid\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n- scope: profile\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n- scope: email\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n- scope: address\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n- scope: roles\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n- scope: offline_access\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n- scope: MyClientId_api\n  source: https://api.beauthenticx.com/.well-known/openid-configuration\n  note: >-\n    Advertised verbatim in scopes_supported. Reads as a template/placeholder identifier left in an\n    IdentityServer configuration rather than a real product\
  \ scope. Recorded as observed, not interpreted.\ncoverage:\n  scopes_in_spec: 1\n  scopes_advertised_by_idp: 8\n  operations_covered_by_scope: 46\n  granularity: coarse\nx-evidence:\n- url: https://api.beauthenticx.com/swagger/v1/swagger.json\n  http_status: 200\n  fetched: '2026-08-06'\n- url: https://api.beauthenticx.com/.well-known/openid-configuration\n  http_status: 200\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authenticx/refs/heads/main/scopes/authenticx-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Conversation Intelligence
- Healthcare
- Speech Analytics
- Contact Center
- Customer Experience
- Quality Assurance
- Pharmacovigilance
- Patient Experience
- Transcription
- Life Sciences
- SCIM
- Authentication
token_urls:
- https://api.beauthenticx.com/connect/token
---
