---
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Salesforce Experience Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Experience Cloud publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Experience Cloud API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schemes:
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-cms-connect-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-cms-delivery-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-connect-communities-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-graphql-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-rest-api-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-sites-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-templates-openapi.yml
- description: Salesforce OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  source: openapi/salesforce-experience-cloud-user-interface-openapi.yml
scope_count: 5
scope_names:
- api
- chatter_api
- content
- full
- web
scopes:
- description: Access and manage your data
  flows:
  - authorizationCode
  scope: api
- description: Manage Chatter data
  flows:
  - authorizationCode
  scope: chatter_api
- description: Manage CMS content
  flows:
  - authorizationCode
  scope: content
- description: Full access
  flows:
  - authorizationCode
  scope: full
- description: Access the web application
  flows:
  - authorizationCode
  scope: web
slug: salesforce-experience-cloud-scopes
source_filename: salesforce-experience-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-experience-cloud-cms-connect-openapi.yml, openapi/salesforce-experience-cloud-cms-delivery-openapi.yml,\n  openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml, openapi/salesforce-experience-cloud-connect-communities-openapi.yml,\n  openapi/salesforce-experience-cloud-graphql-openapi.yml, openapi/salesforce-experience-cloud-rest-api-openapi.yml,\n  openapi/salesforce-experience-cloud-sites-openapi.yml, openapi/salesforce-experience-cloud-templates-openapi.yml,\n  openapi/salesforce-experience-cloud-user-interface-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-cms-connect-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-cms-delivery-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-connect-communities-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-graphql-openapi.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-sites-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-templates-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n\
  \    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\n- name: oauth2\n  source: openapi/salesforce-experience-cloud-user-interface-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: Salesforce OAuth 2.0 authentication\nscopes:\n- scope: api\n  description: Access and manage your data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-experience-cloud-cms-connect-openapi.yml\n  - openapi/salesforce-experience-cloud-cms-delivery-openapi.yml\n  - openapi/salesforce-experience-cloud-cms-managed-content-openapi.yml\n  - openapi/salesforce-experience-cloud-connect-communities-openapi.yml\n  - openapi/salesforce-experience-cloud-graphql-openapi.yml\n  - openapi/salesforce-experience-cloud-rest-api-openapi.yml\n  - openapi/salesforce-experience-cloud-sites-openapi.yml\n\
  \  - openapi/salesforce-experience-cloud-templates-openapi.yml\n  - openapi/salesforce-experience-cloud-user-interface-openapi.yml\n- scope: chatter_api\n  description: Manage Chatter data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-experience-cloud-connect-communities-openapi.yml\n- scope: content\n  description: Manage CMS content\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-experience-cloud-cms-connect-openapi.yml\n- scope: full\n  description: Full access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-experience-cloud-rest-api-openapi.yml\n  - openapi/salesforce-experience-cloud-sites-openapi.yml\n- scope: web\n  description: Access the web application\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/salesforce-experience-cloud-sites-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/scopes/salesforce-experience-cloud-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
