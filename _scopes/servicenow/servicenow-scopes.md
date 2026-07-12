---
authorization_urls:
- https://{instance}.service-now.com/oauth_auth.do
description: ''
docs: https://www.servicenow.com/docs/r/platform-security/authentication/rest-api-auth-scope.html
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Servicenow Scopes
name_suffix: OAuth Scopes
note: ServiceNow does not publish a catalog of OAuth scopes — tokens use the default useraccount scope with access governed by the user's roles and ACLs, and any granular REST API Auth Scopes are custom-defined per instance by administrators (https://www.servicenow.com/docs/r/platform-security/authentication/rest-api-auth-scope.html).
overview: 'ServiceNow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{instance}.service-now.com/oauth_token.do.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ServiceNow
provider_slug: servicenow
schemes:
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-aggregate-api-openapi.yml
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-attachment-api-openapi.yml
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-change-management-api-openapi.yml
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-cmdb-instance-api-openapi.yml
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-import-set-api-openapi.yml
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider.
  flows:
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-service-catalog-api-openapi.yml
- description: OAuth 2.0 authentication using ServiceNow's OAuth provider. Requires a registered OAuth application on the instance.
  flows:
  - authorizationUrl: https://{instance}.service-now.com/oauth_auth.do
    flow: authorizationCode
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  - flow: password
    tokenUrl: https://{instance}.service-now.com/oauth_token.do
  name: oauth2
  source: openapi/servicenow-table-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: servicenow-scopes
source_filename: servicenow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\ndocs: https://www.servicenow.com/docs/r/platform-security/authentication/rest-api-auth-scope.html\nnote: ServiceNow does not publish a catalog of OAuth scopes — tokens use the default\n  useraccount scope with access governed by the user's roles and ACLs, and any granular\n  REST API Auth Scopes are custom-defined per instance by administrators\n  (https://www.servicenow.com/docs/r/platform-security/authentication/rest-api-auth-scope.html).\nsource: openapi/servicenow-aggregate-api-openapi.yml, openapi/servicenow-attachment-api-openapi.yml,\n  openapi/servicenow-change-management-api-openapi.yml, openapi/servicenow-cmdb-instance-api-openapi.yml,\n  openapi/servicenow-import-set-api-openapi.yml, openapi/servicenow-service-catalog-api-openapi.yml,\n  openapi/servicenow-table-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/servicenow-aggregate-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n\
  \  description: OAuth 2.0 authentication using ServiceNow's OAuth provider.\n- name: oauth2\n  source: openapi/servicenow-attachment-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider.\n- name: oauth2\n  source: openapi/servicenow-change-management-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider.\n- name: oauth2\n  source: openapi/servicenow-cmdb-instance-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider.\n- name: oauth2\n  source: openapi/servicenow-import-set-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  description:\
  \ OAuth 2.0 authentication using ServiceNow's OAuth provider.\n- name: oauth2\n  source: openapi/servicenow-service-catalog-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider.\n- name: oauth2\n  source: openapi/servicenow-table-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{instance}.service-now.com/oauth_auth.do\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  - flow: password\n    tokenUrl: https://{instance}.service-now.com/oauth_token.do\n  description: OAuth 2.0 authentication using ServiceNow's OAuth provider. Requires a registered\n    OAuth application on the instance.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/scopes/servicenow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automation
- Cloud Services
- Digital Workflows
- Enterprise Platform
- IT Service Management
- ITSM
- Processes
- T1
- Workflow Automation
- Workflows
token_urls:
- https://{instance}.service-now.com/oauth_token.do
---
