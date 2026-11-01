---
api_specs:
- filename: namirial-auth-api-openapi.yml
  format: yaml
  label: Namirial Auth API
  slug: namirial-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-auth-api-openapi.yml
- filename: namirial-authorization-api-openapi.yml
  format: yaml
  label: Namirial Authorization API
  slug: namirial-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-authorization-api-openapi.yml
- filename: namirial-automaticprofile-api-openapi.yml
  format: yaml
  label: Namirial Automatic Profile API
  slug: namirial-automaticprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-automaticprofile-api-openapi.yml
- filename: namirial-clients-api-openapi.yml
  format: yaml
  label: Namirial Clients API
  slug: namirial-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-clients-api-openapi.yml
- filename: namirial-clientsinstances-api-openapi.yml
  format: yaml
  label: Namirial Clients Instances API
  slug: namirial-clientsinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-clientsinstances-api-openapi.yml
- filename: namirial-documents-api-openapi.yml
  format: yaml
  label: Namirial Documents API
  slug: namirial-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-documents-api-openapi.yml
- filename: namirial-draft-api-openapi.yml
  format: yaml
  label: Namirial Draft API
  slug: namirial-draft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-draft-api-openapi.yml
- filename: namirial-draftactivity-api-openapi.yml
  format: yaml
  label: Namirial Draft Activity API
  slug: namirial-draftactivity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-draftactivity-api-openapi.yml
- filename: namirial-envelope-api-openapi.yml
  format: yaml
  label: Namirial Envelope API
  slug: namirial-envelope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelope-api-openapi.yml
- filename: namirial-envelopeactivity-api-openapi.yml
  format: yaml
  label: Namirial Envelope Activity API
  slug: namirial-envelopeactivity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelopeactivity-api-openapi.yml
- filename: namirial-envelopebulk-api-openapi.yml
  format: yaml
  label: Namirial Envelope Bulk API
  slug: namirial-envelopebulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelopebulk-api-openapi.yml
- filename: namirial-envelopes-api-openapi.yml
  format: yaml
  label: Namirial Envelopes API
  slug: namirial-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelopes-api-openapi.yml
- filename: namirial-file-api-openapi.yml
  format: yaml
  label: Namirial File API
  slug: namirial-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-file-api-openapi.yml
- filename: namirial-instances-api-openapi.yml
  format: yaml
  label: Namirial Instances API
  slug: namirial-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-instances-api-openapi.yml
- filename: namirial-license-api-openapi.yml
  format: yaml
  label: Namirial License API
  slug: namirial-license-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-license-api-openapi.yml
- filename: namirial-organizations-api-openapi.yml
  format: yaml
  label: Namirial Organizations API
  slug: namirial-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-organizations-api-openapi.yml
- filename: namirial-organizationsinstances-api-openapi.yml
  format: yaml
  label: Namirial Organizations Instances API
  slug: namirial-organizationsinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-organizationsinstances-api-openapi.yml
- filename: namirial-processes-api-openapi.yml
  format: yaml
  label: Namirial Processes API
  slug: namirial-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-processes-api-openapi.yml
- filename: namirial-sealingcertificate-api-openapi.yml
  format: yaml
  label: Namirial Sealing Certificate API
  slug: namirial-sealingcertificate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-sealingcertificate-api-openapi.yml
- filename: namirial-system-api-openapi.yml
  format: yaml
  label: Namirial System API
  slug: namirial-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-system-api-openapi.yml
- filename: namirial-team-api-openapi.yml
  format: yaml
  label: Namirial Team API
  slug: namirial-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-team-api-openapi.yml
- filename: namirial-template-api-openapi.yml
  format: yaml
  label: Namirial Template API
  slug: namirial-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-template-api-openapi.yml
authorization_urls:
- /auth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Namirial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Namirial publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Namirial API on a user''s behalf.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Namirial
provider_slug: namirial
schemes:
- description: This API uses OAuth 2 with the authorization code grant flow.
  flows:
  - authorizationUrl: /auth/authorize
    flow: authorizationCode
    tokenUrl: /auth/token
  name: oAuth2AuthCode
  source: openapi/namirial-connectors-openapi.yml
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oAuth2ClientCredentials
  source: openapi/namirial-connectors-openapi.yml
scope_count: 5
scope_names:
- auth:read
- documents:read
- documents:write
- processes:read
- processes:write
scopes:
- description: Read auth
  flows:
  - authorizationCode
  - clientCredentials
  scope: auth:read
- description: Read documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: documents:read
- description: Modify documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: documents:write
- description: Read processes
  flows:
  - authorizationCode
  - clientCredentials
  scope: processes:read
- description: Modify processes
  flows:
  - authorizationCode
  - clientCredentials
  scope: processes:write
slug: namirial-scopes
source_filename: namirial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/namirial-connectors-openapi.yml\nschemes:\n- name: oAuth2AuthCode\n  source: openapi/namirial-connectors-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /auth/authorize\n    tokenUrl: /auth/token\n  description: This API uses OAuth 2 with the authorization code grant flow.\n- name: oAuth2ClientCredentials\n  source: openapi/namirial-connectors-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: This API uses OAuth 2 with the client credentials grant flow.\nscopes:\n- scope: auth:read\n  description: Read auth\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- scope: documents:read\n  description: Read documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- scope: documents:write\n  description: Modify documents\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- scope: processes:read\n  description: Read processes\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- scope: processes:write\n  description: Modify processes\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/namirial/scopes/namirial-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Company
- Digital Trust
- Electronic Signature
- Identity Verification
- Digital Identity
- Trust Services
- Compliance
token_bound: false
token_urls:
- /auth/token
---
