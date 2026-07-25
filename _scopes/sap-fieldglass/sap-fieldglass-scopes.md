---
api_specs:
- filename: sap-fieldglass-approval-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Approval API
  slug: sap-fieldglass-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-approval-api-openapi.yml
- filename: sap-fieldglass-audit-trail-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Audit Trail API
  slug: sap-fieldglass-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-audit-trail-api-openapi.yml
- filename: sap-fieldglass-get-data-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Data API
  slug: sap-fieldglass-get-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-data-api-openapi.yml
- filename: sap-fieldglass-get-entities-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Entities API
  slug: sap-fieldglass-get-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-entities-api-openapi.yml
- filename: sap-fieldglass-get-metadata-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Metadata API
  slug: sap-fieldglass-get-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-metadata-api-openapi.yml
- filename: sap-fieldglass-get-providers-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Get Providers API
  slug: sap-fieldglass-get-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-get-providers-api-openapi.yml
- filename: sap-fieldglass-order-confirmation-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Order Confirmation API
  slug: sap-fieldglass-order-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-order-confirmation-api-openapi.yml
- filename: sap-fieldglass-reports-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Reports API
  slug: sap-fieldglass-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-reports-api-openapi.yml
- filename: sap-fieldglass-results-api-openapi.yml
  format: yaml
  label: SAP Fieldglass Results API
  slug: sap-fieldglass-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-results-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Fieldglass Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP Fieldglass publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP Fieldglass API on a user''s behalf.


  Tokens are issued from  .


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Fieldglass
provider_slug: sap-fieldglass
schemes:
- description: To use this REST API, you need to get OAuth client credentials (user credentials and client-specific application key) from an SAP Fieldglass account representative. After that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint to obtain an access token.
  flows:
  - flow: clientCredentials
    tokenUrl: ' '
  name: OAuth2
  source: openapi/sap-fieldglass-approval-openapi.yaml
- description: To use this REST API, you need to get OAuth client credentials (user credentials and client-specific application key) from an SAP Fieldglass account representative. After that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint to obtain an access token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials
  name: OAuth2
  source: openapi/sap-fieldglass-audit-trail-openapi.json
- description: To use this REST API, you need to get OAuth client credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials
  name: OAuth2
  source: openapi/sap-fieldglass-background-check-openapi.json
- description: To use this REST API, you need to get OAuth client credentials (user credentials and client-specific application key) from an SAP Fieldglass account representative. After that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint to obtain an access token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials
  name: OAuth2
  source: openapi/sap-fieldglass-business-analytics-openapi.json
- description: To use this REST API, you need to get OAuth client credentials (user credentials and client-specific application key) from an SAP Fieldglass account representative. After that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint to obtain an access token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{host}/api/oauth2/v2.0/token?grant_type=client_credentials&response_type=token
  name: OAuth2
  source: openapi/sap-fieldglass-odata-analytic-openapi.json
scope_count: 1
scope_names:
- user
scopes:
- description: approve work items
  flows:
  - clientCredentials
  scope: user
slug: sap-fieldglass-scopes
source_filename: sap-fieldglass-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-fieldglass-approval-openapi.yaml, openapi/sap-fieldglass-audit-trail-openapi.json,\n  openapi/sap-fieldglass-background-check-openapi.json, openapi/sap-fieldglass-business-analytics-openapi.json,\n  openapi/sap-fieldglass-odata-analytic-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/sap-fieldglass-approval-openapi.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: ' '\n  description: To use this REST API, you need to get OAuth client credentials (user credentials\n    and client-specific application key) from an SAP Fieldglass account representative. After\n    that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint\n    to obtain an access token.\n- name: OAuth2\n  source: openapi/sap-fieldglass-audit-trail-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials\n  description:\
  \ To use this REST API, you need to get OAuth client credentials (user credentials\n    and client-specific application key) from an SAP Fieldglass account representative. After\n    that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint\n    to obtain an access token.\n- name: OAuth2\n  source: openapi/sap-fieldglass-background-check-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials\n  description: To use this REST API, you need to get OAuth client credentials\n- name: OAuth2\n  source: openapi/sap-fieldglass-business-analytics-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials\n  description: To use this REST API, you need to get OAuth client credentials (user credentials\n    and client-specific application key) from an SAP Fieldglass account representative. After\n\
  \    that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint\n    to obtain an access token.\n- name: OAuth2\n  source: openapi/sap-fieldglass-odata-analytic-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{host}/api/oauth2/v2.0/token?grant_type=client_credentials&response_type=token\n  description: To use this REST API, you need to get OAuth client credentials (user credentials\n    and client-specific application key) from an SAP Fieldglass account representative. After\n    that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint\n    to obtain an access token.\nscopes:\n- scope: user\n  description: approve work items\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-fieldglass-approval-openapi.yaml\n  - openapi/sap-fieldglass-audit-trail-openapi.json\n  - openapi/sap-fieldglass-background-check-openapi.json\n  - openapi/sap-fieldglass-business-analytics-openapi.json\n  - openapi/sap-fieldglass-odata-analytic-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/scopes/sap-fieldglass-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Contingent Workforce
- External Talent
- Human Capital Management
- Services Procurement
- Statements of Work
- Vendor Management
- Workforce Management
token_urls:
- ' '
- https://api1.fgvms.com/api/oauth2/v2.0/token?grant_type=client_credentials
- https://{host}/api/oauth2/v2.0/token?grant_type=client_credentials&response_type=token
---
