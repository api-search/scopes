---
api_specs:
- filename: sap-api-management-portal-openapi.yml
  format: yaml
  label: SAP API Management API Portal API
  slug: sap-api-management-api-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-api-management/refs/heads/main/openapi/sap-api-management-portal-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Api Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP API Management publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP API Management API on a user''s behalf.


  Tokens are issued from https://{tenantUrl}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP API Management
provider_slug: sap-api-management
schemes:
- description: OAuth 2.0 authentication using SAP BTP service key credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenantUrl}/oauth/token
  name: OAuth2
  source: openapi/sap-api-management-portal-openapi.yml
scope_count: 1
scope_names:
- apiportal.access
scopes:
- description: Full access to API Management portal
  flows:
  - clientCredentials
  scope: apiportal.access
slug: sap-api-management-scopes
source_filename: sap-api-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-api-management-portal-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/sap-api-management-portal-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenantUrl}/oauth/token\n  description: OAuth 2.0 authentication using SAP BTP service key credentials\nscopes:\n- scope: apiportal.access\n  description: Full access to API Management portal\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-api-management-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-api-management/refs/heads/main/scopes/sap-api-management-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- API Management
- Developer Portal
- Enterprise
- SAP
token_urls:
- https://{tenantUrl}/oauth/token
---
