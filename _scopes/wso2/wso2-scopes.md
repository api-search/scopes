---
api_specs:
- filename: wso2-publisher-api.yaml
  format: yaml
  label: WSO2 Publisher API
  slug: publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-publisher-api.yaml
- filename: wso2-devportal-api.yaml
  format: yaml
  label: WSO2 Developer Portal API
  slug: devportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-devportal-api.yaml
- filename: wso2-admin-api.yaml
  format: yaml
  label: WSO2 Admin Portal API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-admin-api.yaml
- filename: wso2-gateway-api.yaml
  format: yaml
  label: WSO2 Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-gateway-api.yaml
- filename: wso2-service-catalog-api.yaml
  format: yaml
  label: WSO2 Service Catalog API
  slug: service-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-service-catalog-api.yaml
- filename: wso2-devops-api.yaml
  format: yaml
  label: WSO2 DevOps API
  slug: devops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-devops-api.yaml
- filename: wso2-dcr-api.yaml
  format: yaml
  label: WSO2 DCR API
  slug: dcr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-dcr-api.yaml
- filename: wso2-governance-api.yaml
  format: yaml
  label: WSO2 Governance API
  slug: governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-governance-api.yaml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Wso2 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WSO2 publishes 51 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the WSO2 API on a user''s behalf.


  Tokens are issued from https://localhost:9443/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WSO2
provider_slug: wso2
schemes:
- flows:
  - flow: password
    tokenUrl: https://localhost:9443/oauth2/token
  name: OAuth2Security
  source: openapi/wso2-admin-api.yaml
- flows:
  - flow: password
    tokenUrl: https://localhost:9443/oauth2/token
  name: OAuth2Security
  source: openapi/wso2-dcr-api.yaml
- flows:
  - flow: password
    tokenUrl: https://localhost:9443/oauth2/token
  name: OAuth2Security
  source: openapi/wso2-devportal-api.yaml
- flows:
  - flow: password
    tokenUrl: https://localhost:9443/oauth2/token
  name: OAuth2Security
  source: openapi/wso2-governance-api.yaml
- flows:
  - flow: password
    tokenUrl: https://localhost:9443/oauth2/token
  name: OAuth2Security
  source: openapi/wso2-service-catalog-api.yaml
scope_count: 51
scope_names:
- apim:admin
- apim:admin_alert_manage
- apim:admin_application_view
- apim:admin_operations
- apim:admin_settings
- apim:admin_tier_manage
- apim:admin_tier_view
- apim:api_category
- apim:api_import_export
- apim:api_key
- apim:api_product_import_export
- apim:api_provider_change
- apim:api_view
- apim:api_workflow_approve
- apim:api_workflow_view
- apim:app_import_export
- apim:app_manage
- apim:app_owner_change
- apim:app_settings_change
- apim:bl_manage
- apim:bl_view
- apim:bot_data
- apim:dcr:app_manage
- apim:environment_manage
- apim:environment_read
- apim:gov_policy_manage
- apim:gov_policy_read
- apim:gov_result_read
- apim:gov_rule_manage
- apim:gov_rule_read
- apim:keymanagers_manage
- apim:llm_provider_manage
- apim:mediation_policy_create
- apim:mediation_policy_view
- apim:monetization_usage_publish
- apim:organization_manage
- apim:organization_read
- apim:policies_import_export
- apim:role_manage
- apim:scope_manage
- apim:store_settings
- apim:sub_alert_manage
- apim:sub_manage
- apim:subscribe
- apim:tenantInfo
- apim:tenant_theme_manage
- apim:tier_manage
- apim:tier_view
- openid
- service_catalog:service_view
- service_catalog:service_write
scopes:
- description: Manage all admin operations
  flows:
  - password
  scope: apim:admin
- description: Manage admin alerts
  flows:
  - password
  scope: apim:admin_alert_manage
- description: View Applications
  flows:
  - password
  scope: apim:admin_application_view
- description: Manage API categories and Key Managers related operations
  flows:
  - password
  scope: apim:admin_operations
- description: Retrieve admin settings
  flows:
  - password
  scope: apim:admin_settings
- description: Update and delete throttling policies
  flows:
  - password
  scope: apim:admin_tier_manage
- description: View throttling policies
  flows:
  - password
  scope: apim:admin_tier_view
- description: Manage API categories
  flows:
  - password
  scope: apim:api_category
- description: Import and export APIs related operations
  flows:
  - password
  scope: apim:api_import_export
- description: Generate API Keys
  flows:
  - password
  scope: apim:api_key
- description: Import and export API Products related operations
  flows:
  - password
  scope: apim:api_product_import_export
- description: Retrieve and manage applications
  flows:
  - password
  scope: apim:api_provider_change
- description: view access to services for read only users
  flows:
  - password
  scope: apim:api_view
- description: Manage workflows
  flows:
  - password
  scope: apim:api_workflow_approve
- description: Retrive workflow requests
  flows:
  - password
  scope: apim:api_workflow_view
- description: Import and export applications related operations
  flows:
  - password
  scope: apim:app_import_export
- description: Retrieve, Manage and Import, Export applications
  flows:
  - password
  scope: apim:app_manage
- description: Retrieve and manage applications
  flows:
  - password
  scope: apim:app_owner_change
- description: Change Application Settings
  flows:
  - password
  scope: apim:app_settings_change
- description: Update and delete deny policies
  flows:
  - password
  scope: apim:bl_manage
- description: View deny policies
  flows:
  - password
  scope: apim:bl_view
- description: Retrieve bot detection data
  flows:
  - password
  scope: apim:bot_data
- description: create oauth app using dcr
  flows:
  - password
  scope: apim:dcr:app_manage
- description: Manage gateway environments
  flows:
  - password
  scope: apim:environment_manage
- description: Retrieve gateway environments
  flows:
  - password
  scope: apim:environment_read
- description: Manage governance policies
  flows:
  - password
  scope: apim:gov_policy_manage
- description: Retrieve governance policies
  flows:
  - password
  scope: apim:gov_policy_read
- description: Retrieve governance results
  flows:
  - password
  scope: apim:gov_result_read
- description: Manage governance rules
  flows:
  - password
  scope: apim:gov_rule_manage
- description: Retrieve governance rules
  flows:
  - password
  scope: apim:gov_rule_read
- description: Manage Key Managers
  flows:
  - password
  scope: apim:keymanagers_manage
- description: Manage LLM Providers
  flows:
  - password
  scope: apim:llm_provider_manage
- description: Create and update mediation policies
  flows:
  - password
  scope: apim:mediation_policy_create
- description: View mediation policies
  flows:
  - password
  scope: apim:mediation_policy_view
- description: Retrieve and publish Monetization related usage records
  flows:
  - password
  scope: apim:monetization_usage_publish
- description: Manage Organizations
  flows:
  - password
  scope: apim:organization_manage
- description: Read Organizations
  flows:
  - password
  scope: apim:organization_read
- description: Export and import policies related operations
  flows:
  - password
  scope: apim:policies_import_export
- description: Manage system roles
  flows:
  - password
  scope: apim:role_manage
- description: Manage system scopes
  flows:
  - password
  scope: apim:scope_manage
- description: Retrieve Developer Portal settings
  flows:
  - password
  scope: apim:store_settings
- description: Retrieve, subscribe and configure Developer Portal alert types
  flows:
  - password
  scope: apim:sub_alert_manage
- description: Retrieve, Manage subscriptions
  flows:
  - password
  scope: apim:sub_manage
- description: Subscribe API
  flows:
  - password
  scope: apim:subscribe
- description: Retrieve tenant related information
  flows:
  - password
  scope: apim:tenantInfo
- description: Manage tenant themes
  flows:
  - password
  scope: apim:tenant_theme_manage
- description: Update and delete throttling policies
  flows:
  - password
  scope: apim:tier_manage
- description: View throttling policies
  flows:
  - password
  scope: apim:tier_view
- description: Authorize access to user details
  flows:
  - password
  scope: openid
- description: view access to services in service catalog
  flows:
  - password
  scope: service_catalog:service_view
- description: write access to services in service catalog
  flows:
  - password
  scope: service_catalog:service_write
slug: wso2-scopes
source_filename: wso2-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wso2-admin-api.yaml, openapi/wso2-dcr-api.yaml, openapi/wso2-devportal-api.yaml,\n  openapi/wso2-governance-api.yaml, openapi/wso2-service-catalog-api.yaml\nschemes:\n- name: OAuth2Security\n  source: openapi/wso2-admin-api.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://localhost:9443/oauth2/token\n- name: OAuth2Security\n  source: openapi/wso2-dcr-api.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://localhost:9443/oauth2/token\n- name: OAuth2Security\n  source: openapi/wso2-devportal-api.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://localhost:9443/oauth2/token\n- name: OAuth2Security\n  source: openapi/wso2-governance-api.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://localhost:9443/oauth2/token\n- name: OAuth2Security\n  source: openapi/wso2-service-catalog-api.yaml\n  flows:\n  - flow: password\n    tokenUrl: https://localhost:9443/oauth2/token\nscopes:\n- scope: apim:admin\n\
  \  description: Manage all admin operations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:admin_alert_manage\n  description: Manage admin alerts\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:admin_application_view\n  description: View Applications\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:admin_operations\n  description: Manage API categories and Key Managers related operations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:admin_settings\n  description: Retrieve admin settings\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:admin_tier_manage\n  description: Update and delete throttling policies\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:admin_tier_view\n  description: View throttling policies\n  flows:\n  - password\n  sources:\n\
  \  - openapi/wso2-admin-api.yaml\n- scope: apim:api_category\n  description: Manage API categories\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:api_import_export\n  description: Import and export APIs related operations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:api_key\n  description: Generate API Keys\n  flows:\n  - password\n  sources:\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:api_product_import_export\n  description: Import and export API Products related operations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:api_provider_change\n  description: Retrieve and manage applications\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:api_view\n  description: view access to services for read only users\n  flows:\n  - password\n  sources:\n  - openapi/wso2-service-catalog-api.yaml\n- scope: apim:api_workflow_approve\n  description:\
  \ Manage workflows\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:api_workflow_view\n  description: Retrive workflow requests\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:app_import_export\n  description: Import and export applications related operations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:app_manage\n  description: Retrieve, Manage and Import, Export applications\n  flows:\n  - password\n  sources:\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:app_owner_change\n  description: Retrieve and manage applications\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:app_settings_change\n  description: Change Application Settings\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:bl_manage\n  description: Update and delete deny policies\n  flows:\n  - password\n  sources:\n\
  \  - openapi/wso2-admin-api.yaml\n- scope: apim:bl_view\n  description: View deny policies\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:bot_data\n  description: Retrieve bot detection data\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:dcr:app_manage\n  description: create oauth app using dcr\n  flows:\n  - password\n  sources:\n  - openapi/wso2-dcr-api.yaml\n- scope: apim:environment_manage\n  description: Manage gateway environments\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:environment_read\n  description: Retrieve gateway environments\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:gov_policy_manage\n  description: Manage governance policies\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-governance-api.yaml\n- scope: apim:gov_policy_read\n  description: Retrieve governance policies\n  flows:\n\
  \  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-governance-api.yaml\n- scope: apim:gov_result_read\n  description: Retrieve governance results\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-governance-api.yaml\n- scope: apim:gov_rule_manage\n  description: Manage governance rules\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-governance-api.yaml\n- scope: apim:gov_rule_read\n  description: Retrieve governance rules\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-governance-api.yaml\n- scope: apim:keymanagers_manage\n  description: Manage Key Managers\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:llm_provider_manage\n  description: Manage LLM Providers\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:mediation_policy_create\n  description: Create and update mediation policies\n\
  \  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:mediation_policy_view\n  description: View mediation policies\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:monetization_usage_publish\n  description: Retrieve and publish Monetization related usage records\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:organization_manage\n  description: Manage Organizations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:organization_read\n  description: Read Organizations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:policies_import_export\n  description: Export and import policies related operations\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:role_manage\n  description: Manage system roles\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:scope_manage\n\
  \  description: Manage system scopes\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:store_settings\n  description: Retrieve Developer Portal settings\n  flows:\n  - password\n  sources:\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:sub_alert_manage\n  description: Retrieve, subscribe and configure Developer Portal alert types\n  flows:\n  - password\n  sources:\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:sub_manage\n  description: Retrieve, Manage subscriptions\n  flows:\n  - password\n  sources:\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:subscribe\n  description: Subscribe API\n  flows:\n  - password\n  sources:\n  - openapi/wso2-devportal-api.yaml\n- scope: apim:tenantInfo\n  description: Retrieve tenant related information\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:tenant_theme_manage\n  description: Manage tenant themes\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n\
  - scope: apim:tier_manage\n  description: Update and delete throttling policies\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: apim:tier_view\n  description: View throttling policies\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n- scope: openid\n  description: Authorize access to user details\n  flows:\n  - password\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-dcr-api.yaml\n  - openapi/wso2-devportal-api.yaml\n  - openapi/wso2-governance-api.yaml\n- scope: service_catalog:service_view\n  description: view access to services in service catalog\n  flows:\n  - password\n  sources:\n  - openapi/wso2-service-catalog-api.yaml\n- scope: service_catalog:service_write\n  description: write access to services in service catalog\n  flows:\n  - password\n  sources:\n  - openapi/wso2-service-catalog-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/scopes/wso2-scopes.yml
summary_line: 51 scopes · password
tags:
- API Management
- Gateways
- Open Source
- API Lifecycle
- GraphQL
- SOAP
- REST
token_urls:
- https://localhost:9443/oauth2/token
---
