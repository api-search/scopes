---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Abm Industries Scopes
name_suffix: OAuth Scopes
note: 'ABM publishes no scopes reference page. What follows is not a reconstruction — it is the authorisation configuration ABM''s own first-party client ships to every browser. ABM Connect uses a SINGLE coarse application scope across every protected resource: there is no per-resource or per-verb scoping, so a token that can read a service location can also reach finance, talent-management and safety resources. That is a real, material finding for anyone assessing delegated access.'
overview: 'ABM Industries uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ABM Industries
provider_slug: abm-industries
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: abm-industries-scopes
source_filename: abm-industries-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  MSAL protected-resource map and `environment` constant read verbatim from ABM's own production\n  bundle https://connect.abm.com/chunk-QN7SXVIA.js, cross-checked against the Azure AD B2C\n  discovery document at\n  https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/B2C_1_cft-signin/v2.0/.well-known/openid-configuration\n  (HTTP 200), 2026-08-29.\nprovider: ABM Industries\nproviderId: abm-industries\napi: ABM Connect\ndocs: null\nnote: >-\n  ABM publishes no scopes reference page. What follows is not a reconstruction — it is the\n  authorisation configuration ABM's own first-party client ships to every browser. ABM Connect\n  uses a SINGLE coarse application scope across every protected resource: there is no per-resource\n  or per-verb scoping, so a token that can read a service location can also reach finance,\n  talent-management and safety resources. That is a real, material finding for anyone assessing\n  delegated\
  \ access.\nscope_model: single coarse application scope\nscope_count: 2\nscopes:\n  - name: https://connect2ABM.onmicrosoft.com/31f16065-3479-4b3c-a3cd-e337cafc33c9/cft_client_access\n    description: >-\n      The one application scope MSAL requests for every ABM Connect protected resource. Granted\n      against ABM's Azure AD B2C application (app ID URI connect2ABM.onmicrosoft.com).\n    applies_to: all resources listed under protected_resources\n  - name: openid\n    description: >-\n      The only scope advertised in `scopes_supported` by ABM's B2C discovery document.\n    source: b2c-discovery\nprotected_resources:\n  base_url: https://connectapi.abm.com/cust-api/\n  note: >-\n    Resource paths are relative to base_url unless an absolute host is shown. Names are ABM's own\n    identifiers. `internal/*` resources are shipped in the customer bundle but are for ABM staff.\n  resources:\n    - { name: UserAccessApi, path: UserAccess/ }\n    - { name: ManageUserApi, path: ManageUser/\
  \ }\n    - { name: MyAccountApi, path: MyAccount/ }\n    - { name: PowerBiEmbedApi, path: PowerBIEmbed/ }\n    - { name: WorkOrderApi, path: WorkOrder/ }\n    - { name: QualityApi, path: Quality/ }\n    - { name: SwopApi, path: SWOP/ }\n    - { name: FinanceApi, path: Finance/ }\n    - { name: ServiceLocationApi, path: ServiceLocation/ }\n    - { name: SafetyApi, path: Safety/ }\n    - { name: TalentManagementApi, path: TalentManagement/ }\n    - { name: AbmConnectApi, path: abm-connect/ }\n    - { name: UserLog, path: abm-connect/user/ }\n    - { name: DocumentApi, path: Documents/ }\n    - { name: SurveyApi, path: survey }\n    - { name: DynamicPageApi, path: DynamicPage/ }\n    - { name: AviationServicesApi, path: AviationServices/ }\n    - { name: AviationQualityApi, path: AviationQuality/ }\n    - { name: Global_WorkOrderApi, path: Global/WorkOrder/ }\n    - { name: Global_QualityApi, path: Global/Quality/ }\n    - { name: Global_FinanceApi, path: Global/Finance/ }\n    - { name:\
  \ Global_ServiceLocationApi, path: Global/ServiceLocation/ }\n    - { name: Global_SafetyApi, path: Global/Safety/ }\n    - { name: Global_TalentManagementApi, path: Global/TalentManagement/ }\n    - { name: Global_InsightsApi, path: Global/Insights/ }\n    - { name: Global_CustomerRel, path: Global/CustomerRel/ }\n    - { name: Global_SocialSafety, path: Global/Social/ }\n    - { name: Global_EnvironmentApi, path: Global/Env/ }\n    - { name: GlobalHomeApi, path: Global/Home/ }\n    - { name: In_GlobalScoreCardApi, path: internal/globalScorecard/, audience: abm-internal }\n    - { name: In_ScoreCardApi, path: internal/scorecard/, audience: abm-internal }\n    - { name: In_FinanceApi, path: internal/finance/, audience: abm-internal }\n    - { name: In_WorkOrderApi, path: internal/workOrders/, audience: abm-internal }\n    - { name: In_SwopApi, path: internal/SWOP/, audience: abm-internal }\n    - { name: In_SafetyApi, path: internal/safety/, audience: abm-internal }\n    - { name: In_QualityApi,\
  \ path: internal/quality/, audience: abm-internal }\n    - { name: In_TalentManagementApi, path: internal/talentmanagement/, audience: abm-internal }\n    - { name: WebAssetsApi, url: https://connectapi.abm.com/web-assets/ }\n    - { name: DocumentApi.blobUrl, url: https://connectapi.abm.com/emp-documents/ }\n    - { name: InvoiceEndpoint, url: https://connectapi.abm.com/emp-invoices-clone/ }\n    - { name: TaskManagementOpsApi, url: https://appservices.abm.com/external/task-mgmt/cust-api/ }\n    - { name: OpsConnectApi, url: https://appservices.abm.com/external/task-mgmt/cust-api/ }\n    - { name: RoutesApi, url: https://appservices-uat.abm.com/external/task-mgmt/tasks-api/, note: points at a UAT host in production }\n    - { name: TaskAIManagementOpsApi, url: https://appservices-uat.abm.com/external/task-mgmt/ai-assitant/, note: points at a UAT host in production }\nresource_count: 44\nevidence:\n  - url: https://connect.abm.com/chunk-QN7SXVIA.js\n    status: 200\n  - url: https://connect2abm.b2clogin.com/connect2abm.onmicrosoft.com/B2C_1_cft-signin/v2.0/.well-known/openid-configuration\n\
  \    status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abm-industries/refs/heads/main/scopes/abm-industries-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Facilities Management
- Engineering
- Infrastructure
- Mobility
- Fortune 500
token_urls: []
---
