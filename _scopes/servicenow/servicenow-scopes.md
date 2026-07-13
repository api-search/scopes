---
api_specs:
- filename: servicenow-table-api-openapi.yml
  format: yaml
  label: ServiceNow Table API
  slug: servicenow-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-table-api-openapi.yml
- filename: servicenow-aggregate-api-openapi.yml
  format: yaml
  label: ServiceNow Aggregate API
  slug: servicenow-aggregate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-aggregate-api-openapi.yml
- filename: servicenow-attachment-api-openapi.yml
  format: yaml
  label: ServiceNow Attachment API
  slug: servicenow-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-attachment-api-openapi.yml
- filename: servicenow-import-set-api-openapi.yml
  format: yaml
  label: ServiceNow Import Set API
  slug: servicenow-import-set-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-import-set-api-openapi.yml
- filename: servicenow-change-management-api-openapi.yml
  format: yaml
  label: ServiceNow Change Management API
  slug: servicenow-change-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-change-management-api-openapi.yml
- filename: servicenow-service-catalog-api-openapi.yml
  format: yaml
  label: ServiceNow Service Catalog API
  slug: servicenow-service-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-service-catalog-api-openapi.yml
- filename: servicenow-cmdb-instance-api-openapi.yml
  format: yaml
  label: ServiceNow CMDB Instance API
  slug: servicenow-cmdb-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/servicenow-cmdb-instance-api-openapi.yml
- filename: contact-api-openapi.yaml
  format: yaml
  label: ServiceNow Contact API
  slug: servicenow-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/contact-api-openapi.yaml
- filename: trouble-ticket-openapi.yaml
  format: yaml
  label: ServiceNow Trouble Ticket Open API
  slug: servicenow-trouble-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/openapi/trouble-ticket-openapi.yaml
- filename: servicenow-events-asyncapi.yml
  format: yaml
  label: ServiceNow Event Management Topic Open API
  slug: servicenow-event-management-topic-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicenow/refs/heads/main/asyncapi/servicenow-events-asyncapi.yml
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
