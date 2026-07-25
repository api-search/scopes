---
api_specs:
- filename: sap-event-mesh-asyncapi.yml
  format: yaml
  label: SAP Event Mesh API
  slug: sap-event-mesh-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/asyncapi/sap-event-mesh-asyncapi.yml
- filename: sap-addresses-api-openapi.yml
  format: yaml
  label: SAP Addresses API
  slug: sap-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-addresses-api-openapi.yml
- filename: sap-artifacts-api-openapi.yml
  format: yaml
  label: SAP Artifacts API
  slug: sap-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-artifacts-api-openapi.yml
- filename: sap-authentication-api-openapi.yml
  format: yaml
  label: SAP Authentication API
  slug: sap-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-authentication-api-openapi.yml
- filename: sap-bank-accounts-api-openapi.yml
  format: yaml
  label: SAP Bank Accounts API
  slug: sap-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-bank-accounts-api-openapi.yml
- filename: sap-business-partners-api-openapi.yml
  format: yaml
  label: SAP Business Partners API
  slug: sap-business-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-business-partners-api-openapi.yml
- filename: sap-configurations-api-openapi.yml
  format: yaml
  label: SAP Configurations API
  slug: sap-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-configurations-api-openapi.yml
- filename: sap-deployments-api-openapi.yml
  format: yaml
  label: SAP Deployments API
  slug: sap-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-deployments-api-openapi.yml
- filename: sap-executions-api-openapi.yml
  format: yaml
  label: SAP Executions API
  slug: sap-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-executions-api-openapi.yml
- filename: sap-invoices-api-openapi.yml
  format: yaml
  label: SAP Invoices API
  slug: sap-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-invoices-api-openapi.yml
- filename: sap-items-api-openapi.yml
  format: yaml
  label: SAP Items API
  slug: sap-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-items-api-openapi.yml
- filename: sap-journal-entries-api-openapi.yml
  format: yaml
  label: SAP Journal Entries API
  slug: sap-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-journal-entries-api-openapi.yml
- filename: sap-orders-api-openapi.yml
  format: yaml
  label: SAP Orders API
  slug: sap-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-orders-api-openapi.yml
- filename: sap-roles-api-openapi.yml
  format: yaml
  label: SAP Roles API
  slug: sap-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-roles-api-openapi.yml
- filename: sap-scenarios-api-openapi.yml
  format: yaml
  label: SAP Scenarios API
  slug: sap-scenarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-scenarios-api-openapi.yml
- filename: sap-tax-numbers-api-openapi.yml
  format: yaml
  label: SAP Tax Numbers API
  slug: sap-tax-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/openapi/sap-tax-numbers-api-openapi.yml
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
