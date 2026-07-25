---
api_specs:
- filename: bynder-account-api-openapi.yml
  format: yaml
  label: Bynder Account API
  slug: bynder-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-account-api-openapi.yml
- filename: bynder-analytics-api-openapi.yml
  format: yaml
  label: Bynder Analytics API
  slug: bynder-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-analytics-api-openapi.yml
- filename: bynder-authentication-api-openapi.yml
  format: yaml
  label: Bynder Authentication API
  slug: bynder-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-authentication-api-openapi.yml
- filename: bynder-automation-api-openapi.yml
  format: yaml
  label: Bynder Automation API
  slug: bynder-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-automation-api-openapi.yml
- filename: bynder-brands-api-openapi.yml
  format: yaml
  label: Bynder Brands API
  slug: bynder-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-brands-api-openapi.yml
- filename: bynder-collections-api-openapi.yml
  format: yaml
  label: Bynder Collections API
  slug: bynder-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-collections-api-openapi.yml
- filename: bynder-contentaccess-api-openapi.yml
  format: yaml
  label: Bynder ContentAccess API
  slug: bynder-contentaccess-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-contentaccess-api-openapi.yml
- filename: bynder-derivatives-api-openapi.yml
  format: yaml
  label: Bynder Derivatives API
  slug: bynder-derivatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-derivatives-api-openapi.yml
- filename: bynder-media-api-openapi.yml
  format: yaml
  label: Bynder Media API
  slug: bynder-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-media-api-openapi.yml
- filename: bynder-metaproperties-api-openapi.yml
  format: yaml
  label: Bynder Metaproperties API
  slug: bynder-metaproperties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-metaproperties-api-openapi.yml
- filename: bynder-orders-api-openapi.yml
  format: yaml
  label: Bynder Orders API
  slug: bynder-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-orders-api-openapi.yml
- filename: bynder-quarantine-api-openapi.yml
  format: yaml
  label: Bynder Quarantine API
  slug: bynder-quarantine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-quarantine-api-openapi.yml
- filename: bynder-smartfilters-api-openapi.yml
  format: yaml
  label: Bynder Smartfilters API
  slug: bynder-smartfilters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-smartfilters-api-openapi.yml
- filename: bynder-tags-api-openapi.yml
  format: yaml
  label: Bynder Tags API
  slug: bynder-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-tags-api-openapi.yml
- filename: bynder-taxonomy-api-openapi.yml
  format: yaml
  label: Bynder Taxonomy API
  slug: bynder-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-taxonomy-api-openapi.yml
- filename: bynder-trash-api-openapi.yml
  format: yaml
  label: Bynder Trash API
  slug: bynder-trash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-trash-api-openapi.yml
- filename: bynder-upload-api-openapi.yml
  format: yaml
  label: Bynder Upload API
  slug: bynder-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-upload-api-openapi.yml
- filename: bynder-users-api-openapi.yml
  format: yaml
  label: Bynder Users API
  slug: bynder-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-users-api-openapi.yml
- filename: bynder-webhooks-api-openapi.yml
  format: yaml
  label: Bynder Webhooks API
  slug: bynder-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-webhooks-api-openapi.yml
- filename: bynder-workflow-api-openapi.yml
  format: yaml
  label: Bynder Workflow API
  slug: bynder-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-workflow-api-openapi.yml
authorization_urls:
- https://yourportal.bynder.com/v6/authentication/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bynder Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bynder publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bynder API on a user''s behalf.


  Tokens are issued from https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bynder
provider_slug: bynder
schemes:
- description: OAuth 2.0 with JWT bearer access tokens
  flows:
  - authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization
  - flow: clientCredentials
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials
  name: oauth2
  source: openapi/bynder-openapi.yml
scope_count: 7
scope_names:
- asset:read
- asset:write
- collection:read
- collection:write
- meta.assetbank:read
- meta.assetbank:write
- offline
scopes:
- description: Read assets
  flows:
  - authorizationCode
  - clientCredentials
  scope: asset:read
- description: Write assets
  flows:
  - authorizationCode
  - clientCredentials
  scope: asset:write
- description: Read collections
  flows:
  - authorizationCode
  scope: collection:read
- description: Write collections
  flows:
  - authorizationCode
  scope: collection:write
- description: Read asset bank metaproperties
  flows:
  - authorizationCode
  scope: meta.assetbank:read
- description: Write asset bank metaproperties
  flows:
  - authorizationCode
  scope: meta.assetbank:write
- description: Refresh token access
  flows:
  - authorizationCode
  scope: offline
slug: bynder-scopes
source_filename: bynder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bynder-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bynder-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization\n  - flow: clientCredentials\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials\n  description: OAuth 2.0 with JWT bearer access tokens\nscopes:\n- scope: asset:read\n  description: Read assets\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: asset:write\n  description: Write assets\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: collection:read\n  description: Read collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope:\
  \ collection:write\n  description: Write collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: meta.assetbank:read\n  description: Read asset bank metaproperties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: meta.assetbank:write\n  description: Write asset bank metaproperties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: offline\n  description: Refresh token access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/scopes/bynder-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Digital Asset Management
- DAM
- Brand Management
- Content Management
- Marketing
token_urls:
- https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization
- https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials
---
