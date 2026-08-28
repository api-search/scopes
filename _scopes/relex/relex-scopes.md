---
api_specs:
- filename: relex-data-api-openapi.json
  format: json
  label: RELEX Data API
  slug: relex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-data-api-openapi.json
- filename: relex-monitoring-api-openapi.json
  format: json
  label: RELEX Monitoring API
  slug: relex-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-monitoring-api-openapi.json
authorization_urls: []
description: ''
docs: https://www.relexsolutions.com/api/retail-restapi-example-customer.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Relex Scopes
name_suffix: OAuth Scopes
note: 'RELEX publishes no scopes/permissions reference page. The authoritative public list is the `scopes_supported` array of RELEX Identity''s own OpenID Connect discovery documents, which are served anonymously and are identical across all three authorities (root, /login/restapi_prod, /monitoring_api_prod) and both regions. That list is far richer than the contracts: the Data API declares ONE scope, the Monitoring API declares NONE, while RELEX Identity advertises 51. Scopes are granted per client during provisioning; there is no self-service consent screen for the client-credentials clients these APIs use.'
overview: 'RELEX Solutions publishes 51 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the RELEX Solutions API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RELEX Solutions
provider_slug: relex
schemes:
- api: RELEX Data API
  declared_scopes:
  - openid_api
  description: The RELEX Data API uses OAuth 2 with the client credentials flow.
  flow: clientCredentials
  name: OAuth2
  source: openapi/relex-data-api-openapi.json
  tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_prod/connect/token
  tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/login/restapi_prod/connect/token
- api: RELEX Monitoring API
  declared_scopes: []
  flow: clientCredentials
  gap: The Monitoring API's securityScheme declares an EMPTY scopes map, so the contract alone does not tell a client what to request. RELEX Identity advertises four environment-scoped monitoring scopes (restapi_prod_monitoring, restapi_uat_monitoring, restapi_test_monitoring, restapi_dev_monitoring) that are almost certainly the ones this API expects.
  name: oauth2
  source: openapi/relex-monitoring-api-openapi.json
  tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token
  tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token
scope_count: 51
scope_names:
- openid_api
- restapi_prod_monitoring
- restapi_uat_monitoring
- restapi_test_monitoring
- restapi_dev_monitoring
- openid
- profile
- email
- offline_access
- roles
- tenant
- groups
- email-relex-saas
- automation
- healthcheck
- scimhost
- users:read
- tenants:read
- tenants:write
- tenants:list
- serviceproviders:read
- serviceproviders:write
- clients:read
- clients:write
- reports:read
- AccountSettingsView
- MasterDataView
- SystemSettingsView
- ReportView
- ScmView
- PerformanceDataEdit
- ManualOrdersView
- ManualOrdersEdit
- StoreVersionView
- FloorPlanView
- FloorPlanEdit
- FloorPlanAutomationView
- FloorPlanDeliveryView
- FloorPlanDeliveryEdit
- PlanogramView
- PlanogramEdit
- PlanogramAssignmentView
- PlanogramDeliverySpaceView
- PlanogrammingDataIntegrationEdit
- LocationLedAssignmentsView
- MicroSpaceView
- MicroSpaceEdit
- MicroSpaceReviewsView
- MicroSpaceWorkflowsView
- GridEdit
- PDREQ-7480
scopes:
- description: Internal use
  flows:
  - clientCredentials
  scope: openid_api
- description: Monitoring access to the production REST API environment (inferred from the name; RELEX publishes no description).
  flows: []
  scope: restapi_prod_monitoring
- description: ''
  flows: []
  scope: restapi_uat_monitoring
- description: ''
  flows: []
  scope: restapi_test_monitoring
- description: ''
  flows: []
  scope: restapi_dev_monitoring
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: roles
- description: ''
  flows: []
  scope: tenant
- description: ''
  flows: []
  scope: groups
- description: ''
  flows: []
  scope: email-relex-saas
- description: ''
  flows: []
  scope: automation
- description: ''
  flows: []
  scope: healthcheck
- description: ''
  flows: []
  scope: scimhost
- description: ''
  flows: []
  scope: users:read
- description: ''
  flows: []
  scope: tenants:read
- description: ''
  flows: []
  scope: tenants:write
- description: ''
  flows: []
  scope: tenants:list
- description: ''
  flows: []
  scope: serviceproviders:read
- description: ''
  flows: []
  scope: serviceproviders:write
- description: ''
  flows: []
  scope: clients:read
- description: ''
  flows: []
  scope: clients:write
- description: ''
  flows: []
  scope: reports:read
- description: ''
  flows: []
  scope: AccountSettingsView
- description: ''
  flows: []
  scope: MasterDataView
- description: ''
  flows: []
  scope: SystemSettingsView
- description: ''
  flows: []
  scope: ReportView
- description: ''
  flows: []
  scope: ScmView
- description: ''
  flows: []
  scope: PerformanceDataEdit
- description: ''
  flows: []
  scope: ManualOrdersView
- description: ''
  flows: []
  scope: ManualOrdersEdit
- description: ''
  flows: []
  scope: StoreVersionView
- description: ''
  flows: []
  scope: FloorPlanView
- description: ''
  flows: []
  scope: FloorPlanEdit
- description: ''
  flows: []
  scope: FloorPlanAutomationView
- description: ''
  flows: []
  scope: FloorPlanDeliveryView
- description: ''
  flows: []
  scope: FloorPlanDeliveryEdit
- description: ''
  flows: []
  scope: PlanogramView
- description: ''
  flows: []
  scope: PlanogramEdit
- description: ''
  flows: []
  scope: PlanogramAssignmentView
- description: ''
  flows: []
  scope: PlanogramDeliverySpaceView
- description: ''
  flows: []
  scope: PlanogrammingDataIntegrationEdit
- description: ''
  flows: []
  scope: LocationLedAssignmentsView
- description: ''
  flows: []
  scope: MicroSpaceView
- description: ''
  flows: []
  scope: MicroSpaceEdit
- description: ''
  flows: []
  scope: MicroSpaceReviewsView
- description: ''
  flows: []
  scope: MicroSpaceWorkflowsView
- description: ''
  flows: []
  scope: GridEdit
- description: ''
  flows: []
  scope: PDREQ-7480
slug: relex-scopes
source_filename: relex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://identity.prod-eu.prod.cc.relexsolutions.com/.well-known/openid-configuration\ndocs: https://www.relexsolutions.com/api/retail-restapi-example-customer.html\nderived_from:\n- openapi/relex-data-api-openapi.json\n- openapi/relex-monitoring-api-openapi.json\n- well-known/relex-identity-eu-openid-configuration.json\nnote: >-\n  RELEX publishes no scopes/permissions reference page. The authoritative public list is the\n  `scopes_supported` array of RELEX Identity's own OpenID Connect discovery documents, which are\n  served anonymously and are identical across all three authorities (root, /login/restapi_prod,\n  /monitoring_api_prod) and both regions. That list is far richer than the contracts: the Data API\n  declares ONE scope, the Monitoring API declares NONE, while RELEX Identity advertises 51.\n  Scopes are granted per client during provisioning; there is no self-service consent screen for\n  the client-credentials\
  \ clients these APIs use.\nschemes:\n- name: OAuth2\n  api: RELEX Data API\n  source: openapi/relex-data-api-openapi.json\n  flow: clientCredentials\n  tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_prod/connect/token\n  tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/login/restapi_prod/connect/token\n  declared_scopes:\n  - openid_api\n  description: The RELEX Data API uses OAuth 2 with the client credentials flow.\n- name: oauth2\n  api: RELEX Monitoring API\n  source: openapi/relex-monitoring-api-openapi.json\n  flow: clientCredentials\n  tokenUrl: https://identity.prod-eu.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token\n  tokenUrl_us: https://identity.prod-us.prod.cc.relexsolutions.com/monitoring_api_prod/connect/token\n  declared_scopes: []\n  gap: >-\n    The Monitoring API's securityScheme declares an EMPTY scopes map, so the contract alone does\n    not tell a client what to request. RELEX Identity advertises four environment-scoped\
  \ monitoring\n    scopes (restapi_prod_monitoring, restapi_uat_monitoring, restapi_test_monitoring,\n    restapi_dev_monitoring) that are almost certainly the ones this API expects.\nscope_count: 51\nscopes:\n- scope: openid_api\n  description: Internal use\n  declared_in: openapi/relex-data-api-openapi.json\n  flows:\n  - clientCredentials\n  note: The only scope either OpenAPI names. RELEX's own description of it is literally\n    \"Internal use\", which tells an integrator nothing.\n- scope: restapi_prod_monitoring\n  group: monitoring\n  description: Monitoring access to the production REST API environment (inferred from the name;\n    RELEX publishes no description).\n- scope: restapi_uat_monitoring\n  group: monitoring\n- scope: restapi_test_monitoring\n  group: monitoring\n- scope: restapi_dev_monitoring\n  group: monitoring\n- scope: openid\n  group: oidc-standard\n- scope: profile\n  group: oidc-standard\n- scope: email\n  group: oidc-standard\n- scope: offline_access\n  group:\
  \ oidc-standard\n- scope: roles\n  group: identity\n- scope: tenant\n  group: identity\n- scope: groups\n  group: identity\n- scope: email-relex-saas\n  group: identity\n- scope: automation\n  group: identity\n- scope: healthcheck\n  group: platform\n- scope: scimhost\n  group: provisioning\n  note: >-\n    Indicates a SCIM user-provisioning surface exists inside the platform. No SCIM base URL,\n    /ServiceProviderConfig, /Schemas or urn:ietf:params:scim:schemas:* URN is published anywhere\n    public — see conformance/relex-conformance.yml.\n- scope: users:read\n  group: administration\n- scope: tenants:read\n  group: administration\n- scope: tenants:write\n  group: administration\n- scope: tenants:list\n  group: administration\n- scope: serviceproviders:read\n  group: administration\n- scope: serviceproviders:write\n  group: administration\n- scope: clients:read\n  group: administration\n- scope: clients:write\n  group: administration\n- scope: reports:read\n  group: administration\n\
  - scope: AccountSettingsView\n  group: application-permission\n- scope: MasterDataView\n  group: application-permission\n- scope: SystemSettingsView\n  group: application-permission\n- scope: ReportView\n  group: application-permission\n- scope: ScmView\n  group: application-permission\n- scope: PerformanceDataEdit\n  group: application-permission\n- scope: ManualOrdersView\n  group: application-permission\n- scope: ManualOrdersEdit\n  group: application-permission\n- scope: StoreVersionView\n  group: application-permission\n- scope: FloorPlanView\n  group: space-planning\n- scope: FloorPlanEdit\n  group: space-planning\n- scope: FloorPlanAutomationView\n  group: space-planning\n- scope: FloorPlanDeliveryView\n  group: space-planning\n- scope: FloorPlanDeliveryEdit\n  group: space-planning\n- scope: PlanogramView\n  group: space-planning\n- scope: PlanogramEdit\n  group: space-planning\n- scope: PlanogramAssignmentView\n  group: space-planning\n- scope: PlanogramDeliverySpaceView\n  group:\
  \ space-planning\n- scope: PlanogrammingDataIntegrationEdit\n  group: space-planning\n- scope: LocationLedAssignmentsView\n  group: space-planning\n- scope: MicroSpaceView\n  group: space-planning\n- scope: MicroSpaceEdit\n  group: space-planning\n- scope: MicroSpaceReviewsView\n  group: space-planning\n- scope: MicroSpaceWorkflowsView\n  group: space-planning\n- scope: GridEdit\n  group: space-planning\n- scope: PDREQ-7480\n  group: unknown\n  note: An internal ticket reference leaked into the public scope list. Recorded verbatim because\n    it is genuinely advertised; it is not a scope an integrator should request.\nidentity_provider:\n  product: RELEX Identity (Duende/IdentityServer-family)\n  issuers:\n  - https://identity.prod-eu.prod.cc.relexsolutions.com\n  - https://identity.prod-eu.prod.cc.relexsolutions.com/login/restapi_prod\n  - https://identity.prod-eu.prod.cc.relexsolutions.com/monitoring_api_prod\n  - https://identity.prod-us.prod.cc.relexsolutions.com\n  - https://identity.prod-us.prod.cc.relexsolutions.com/login/restapi_prod\n\
  \  - https://identity.prod-us.prod.cc.relexsolutions.com/monitoring_api_prod\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  note: >-\n    The discovery documents advertise the full IdentityServer grant surface, including implicit and\n    resource-owner password, which are discouraged by OAuth 2.1. That is the IdP's capability list,\n    not what these two APIs use — both APIs use client_credentials only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/scopes/relex-scopes.yml
summary_line: 51 scopes
tags:
- Supply Chain
- Retail
- Demand Planning
- Inventory Management
- Forecasting
- Pricing
- Enterprise Software
- Data Integration
- Company
token_urls: []
---
