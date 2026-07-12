---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Apigee Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apigee publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apigee API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apigee
provider_slug: apigee
schemes:
- description: Google OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/apigee-api-hub-openapi.yml
- description: Google OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/apigee-api-management-openapi.yml
- description: Google OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/apigee-apim-openapi.yml
- description: Google OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/apigee-integrations-openapi.yml
- description: Google OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/apigee-registry-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Full access to Google Cloud Platform resources
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: apigee-scopes
source_filename: apigee-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apigee-api-hub-openapi.yml, openapi/apigee-api-management-openapi.yml, openapi/apigee-apim-openapi.yml,\n  openapi/apigee-integrations-openapi.yml, openapi/apigee-registry-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/apigee-api-hub-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/apigee-api-management-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/apigee-apim-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n\
  \  description: Google OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/apigee-integrations-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/apigee-registry-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 authentication\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: Full access to Google Cloud Platform resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/apigee-api-hub-openapi.yml\n  - openapi/apigee-api-management-openapi.yml\n  - openapi/apigee-apim-openapi.yml\n  - openapi/apigee-integrations-openapi.yml\n  - openapi/apigee-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apigee/refs/heads/main/scopes/apigee-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Advanced API Security
- Agentic AI
- Analytics
- API Gateway
- API Governance
- API Hub
- API Management
- Developer Portal
- Enterprise
- Generative AI
- Hybrid
- Integrations
- Microservices
- MCP
- Model Context Protocol
- Monetization
token_urls:
- https://oauth2.googleapis.com/token
---
