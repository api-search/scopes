---
api_specs:
- filename: swagger.json
  format: json
  label: Adobe Captivate Prime API
  slug: adobe-captivate-prime-api
  spec_type: OpenAPI
  url: https://learningmanager.adobe.com/primeapi/v2/swagger.json
- filename: adobe-captivate-learning-manager-webhooks-asyncapi.yml
  format: yaml
  label: Adobe Learning Manager Webhooks API
  slug: adobe-learning-manager-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/asyncapi/adobe-captivate-learning-manager-webhooks-asyncapi.yml
authorization_urls:
- https://learningmanager.adobe.com/oauth/o/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Adobe Captivate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adobe Captivate publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adobe Captivate API on a user''s behalf.


  Tokens are issued from https://learningmanager.adobe.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schemes:
- description: OAuth 2.0 authentication via Adobe IMS. Supports authorization code flow for user-context access and client credentials flow for application-level access.
  flows:
  - authorizationUrl: https://learningmanager.adobe.com/oauth/o/authorize
    flow: authorizationCode
    tokenUrl: https://learningmanager.adobe.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://learningmanager.adobe.com/oauth/token
  name: oauth2
  source: openapi/adobe-captivate-prime-api-openapi.yml
scope_count: 4
scope_names:
- admin:read
- admin:write
- learner:read
- learner:write
scopes:
- description: Read access to admin data
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin:read
- description: Write access to admin data
  flows:
  - authorizationCode
  - clientCredentials
  scope: admin:write
- description: Read access to learner data
  flows:
  - authorizationCode
  - clientCredentials
  scope: learner:read
- description: Write access to learner data
  flows:
  - authorizationCode
  scope: learner:write
slug: adobe-captivate-scopes
source_filename: adobe-captivate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-captivate-prime-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/adobe-captivate-prime-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://learningmanager.adobe.com/oauth/o/authorize\n    tokenUrl: https://learningmanager.adobe.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://learningmanager.adobe.com/oauth/token\n  description: OAuth 2.0 authentication via Adobe IMS. Supports authorization code flow for\n    user-context access and client credentials flow for application-level access.\nscopes:\n- scope: admin:read\n  description: Read access to admin data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/adobe-captivate-prime-api-openapi.yml\n- scope: admin:write\n  description: Write access to admin data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/adobe-captivate-prime-api-openapi.yml\n\
  - scope: learner:read\n  description: Read access to learner data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/adobe-captivate-prime-api-openapi.yml\n- scope: learner:write\n  description: Write access to learner data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/adobe-captivate-prime-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/scopes/adobe-captivate-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
token_urls:
- https://learningmanager.adobe.com/oauth/token
---
