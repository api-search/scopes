---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: derived
name: Sap Commerce Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP Commerce Cloud publishes 3 OAuth 2.0 scopes via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP Commerce Cloud API on a user''s behalf.


  Tokens are issued from https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce-cloud
schemes:
- description: OAuth 2.0 authentication for SAP Commerce Cloud Admin API
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  source: openapi/sap-commerce-cloud-admin-openapi.yml
- description: OAuth 2.0 authentication for SAP Commerce Cloud
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  source: openapi/sap-commerce-cloud-assisted-service-openapi.yml
- description: OAuth 2.0 authentication for SAP Commerce Cloud
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  - flow: password
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  source: openapi/sap-commerce-cloud-commerce-web-services-openapi.yml
- description: OAuth 2.0 authentication for SAP Commerce Cloud Integration API
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  source: openapi/sap-commerce-cloud-integration-openapi.yml
- description: OAuth 2.0 authentication for SAP Commerce Cloud
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
  name: oauth2
  source: openapi/sap-commerce-cloud-product-content-management-openapi.yml
scope_count: 3
scope_names:
- admin
- assistedservicegroup
- basic
scopes:
- description: Administrative access
  flows:
  - clientCredentials
  scope: admin
- description: Assisted service agent access
  flows:
  - clientCredentials
  scope: assistedservicegroup
- description: Basic access
  flows:
  - clientCredentials
  - password
  scope: basic
slug: sap-commerce-cloud-scopes
source_filename: sap-commerce-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-commerce-cloud-admin-openapi.yml, openapi/sap-commerce-cloud-assisted-service-openapi.yml,\n  openapi/sap-commerce-cloud-commerce-web-services-openapi.yml, openapi/sap-commerce-cloud-integration-openapi.yml,\n  openapi/sap-commerce-cloud-product-content-management-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-commerce-cloud-admin-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n  description: OAuth 2.0 authentication for SAP Commerce Cloud Admin API\n- name: oauth2\n  source: openapi/sap-commerce-cloud-assisted-service-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n  description: OAuth 2.0 authentication for SAP Commerce Cloud\n- name: oauth2\n  source: openapi/sap-commerce-cloud-commerce-web-services-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n  - flow: password\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n  description: OAuth 2.0 authentication for SAP Commerce Cloud\n- name: oauth2\n  source: openapi/sap-commerce-cloud-integration-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n  description: OAuth 2.0 authentication for SAP Commerce Cloud Integration API\n- name: oauth2\n  source: openapi/sap-commerce-cloud-product-content-management-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token\n  description: OAuth 2.0 authentication for SAP Commerce Cloud\nscopes:\n- scope: admin\n  description: Administrative access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-commerce-cloud-admin-openapi.yml\n\
  - scope: assistedservicegroup\n  description: Assisted service agent access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-commerce-cloud-assisted-service-openapi.yml\n- scope: basic\n  description: Basic access\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/sap-commerce-cloud-assisted-service-openapi.yml\n  - openapi/sap-commerce-cloud-commerce-web-services-openapi.yml\n  - openapi/sap-commerce-cloud-integration-openapi.yml\n  - openapi/sap-commerce-cloud-product-content-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce-cloud/refs/heads/main/scopes/sap-commerce-cloud-scopes.yml
summary_line: 3 scopes · clientCredentials/password
tags:
- B2B
- B2C
- Commerce
- Customer Experience
- Ecommerce
- Omnichannel
- Retail
token_urls:
- https://{tenant}.{region}.commercecloud.sap/authorizationserver/oauth/token
---
