---
api_specs:
- filename: sap-business-one-service-layer-openapi.yml
  format: yaml
  label: SAP Business One Service Layer API
  slug: sap-business-one-service-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-business-one-service-layer-openapi.yml
- filename: sap-s4hana-cloud-business-partner-openapi.yml
  format: yaml
  label: SAP S/4HANA Cloud API
  slug: sap-s4hana-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-s4hana-cloud-business-partner-openapi.yml
- filename: sap-event-mesh-asyncapi.yml
  format: yaml
  label: SAP Event Mesh API
  slug: sap-event-mesh-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/asyncapi/sap-event-mesh-asyncapi.yml
- filename: sap-ai-core-openapi.yml
  format: yaml
  label: SAP AI Core API
  slug: sap-ai-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-ai-core-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP API on a user''s behalf.


  Tokens are issued from https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP
provider_slug: sap
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-ai-core-openapi.yml
- description: OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://{host}/oauth/token
  name: oauth2
  source: openapi/sap-s4hana-cloud-business-partner-openapi.yml
scope_count: 1
scope_names:
- API_BUSINESS_PARTNER
scopes:
- description: Access to Business Partner API
  flows:
  - clientCredentials
  scope: API_BUSINESS_PARTNER
slug: sap-scopes
source_filename: sap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-ai-core-openapi.yml, openapi/sap-s4hana-cloud-business-partner-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-ai-core-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n- name: oauth2\n  source: openapi/sap-s4hana-cloud-business-partner-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{host}/oauth/token\n  description: OAuth 2.0 authentication\nscopes:\n- scope: API_BUSINESS_PARTNER\n  description: Access to Business Partner API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sap-s4hana-cloud-business-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/scopes/sap-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
token_urls:
- https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
- https://{host}/oauth/token
---
