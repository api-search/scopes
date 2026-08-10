---
authorization_urls:
- https://www.employeenavigator.com/identity/connect/authorize
description: ''
docs: https://www.employeenavigator.com/security/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Employeenavigator Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Employee Navigator publishes 66 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Employee Navigator API on a user''s behalf.


  Tokens are issued from https://www.employeenavigator.com/identity/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Employee Navigator
provider_slug: employeenavigator
schemes:
- flows:
  - authorizationUrl: https://www.employeenavigator.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://www.employeenavigator.com/identity/connect/token
  - flow: clientCredentials
    tokenUrl: https://www.employeenavigator.com/identity/connect/token
  issuer: https://www.employeenavigator.com/identity
  name: OAuth2
  source: well-known/employeenavigator-openid-configuration.json
scope_count: 66
scope_names:
- openid
- profile
- email
- EnApi
- MasterCompanyIntegrationApi
- MasterConfigurationApi
- MasterNotificationApi
- MasterPushNotificationApi
- MasterDataAuditApi
- MasterDataSyncApi
- CobraConfigurationApi
- CobraNotificationApi
- CarrierCompanyIntegrationApi
- CarrierCompanyIntegrationConnectionApi
- CarrierConfigurationApi
- CarrierNotificationApi
- CarrierPushNotificationApi
- CarrierDataAuditApi
- CarrierDataSyncApi
- QuoteCensusApi
- AgencyManagementApi
- QuotingCompanyIntegrationApi
- QuotingConfigurationApi
- QuotingNotificationApi
- QuotingPushNotificationApi
- AgencyConfigurationApi
- AgencyNotificationApi
- PayrollCompanyIntegrationApi
- PayrollEmployeeNotificationApi
- PayrollNotificationApi
- CarrierMemberBenefitApi
- EvidenceOfInsurabilityApi
- EvidenceOfInsurabilityNotificationApi
- EmployeeBenefitsManagementApi
- RatesServiceApi
- WebhookApi
- CompanyManagementApi
- CompanyConfigurationApi
- PlanListConfigurationApi
- PlanListManagementApi
- HealthPlanConfigurationApi
- SupplementalPlanConfigurationApi
- MedicalSavingsPlanConfigurationApi
- VoluntaryLifePlanConfigurationApi
- VoluntaryDisabilityPlanConfigurationApi
- EmployeeProfileApi
- EmployeeProfileConfigurationApi
- EmployeeProfileManagementApi
- EmployeeProfilePayrollApi
- EmployeeProfilePayrollConfigurationApi
- EmployeeProfilePayrollManagementApi
- HealthPlanManagementApi
- SupplementalPlanManagementApi
- GroupLifePlanConfigurationApi
- EaseMigrationApi
- GroupDisabilityPlanConfigurationApi
- GroupLifePlanManagementApi
- VoluntaryLifePlanManagementApi
- GroupDisabilityPlanManagementApi
- CafeteriaPlanManagementApi
- CafeteriaPlanConfigurationApi
- VoluntaryDisabilityPlanManagementApi
- PaycorCompanyIntegrationApi
- CarrierListManagementApi
- CompanyIdentifierReplacementApi
- offline_access
scopes:
- description: OpenID Connect standard scope; requests an ID token for the authenticated subject.
  flows: []
  scope: openid
- description: OpenID Connect standard scope; requests the profile claim set (name, family_name, given_name, nickname, birthdate, locale and related claims).
  flows: []
  scope: profile
- description: OpenID Connect standard scope; requests the email and email_verified claims.
  flows: []
  scope: email
- description: Access to the Employee Navigator En API service.
  flows: []
  scope: EnApi
- description: Access to the Employee Navigator Master Company Integration API service.
  flows: []
  scope: MasterCompanyIntegrationApi
- description: Access to the Employee Navigator Master Configuration API service.
  flows: []
  scope: MasterConfigurationApi
- description: Access to the Employee Navigator Master Notification API service.
  flows: []
  scope: MasterNotificationApi
- description: Access to the Employee Navigator Master Push Notification API service.
  flows: []
  scope: MasterPushNotificationApi
- description: Access to the Employee Navigator Master Data Audit API service.
  flows: []
  scope: MasterDataAuditApi
- description: Access to the Employee Navigator Master Data Sync API service.
  flows: []
  scope: MasterDataSyncApi
- description: Access to the Employee Navigator Cobra Configuration API service.
  flows: []
  scope: CobraConfigurationApi
- description: Access to the Employee Navigator Cobra Notification API service.
  flows: []
  scope: CobraNotificationApi
- description: Access to the Employee Navigator Carrier Company Integration API service.
  flows: []
  scope: CarrierCompanyIntegrationApi
- description: Access to the Employee Navigator Carrier Company Integration Connection API service.
  flows: []
  scope: CarrierCompanyIntegrationConnectionApi
- description: Access to the Employee Navigator Carrier Configuration API service.
  flows: []
  scope: CarrierConfigurationApi
- description: Access to the Employee Navigator Carrier Notification API service.
  flows: []
  scope: CarrierNotificationApi
- description: Access to the Employee Navigator Carrier Push Notification API service.
  flows: []
  scope: CarrierPushNotificationApi
- description: Access to the Employee Navigator Carrier Data Audit API service.
  flows: []
  scope: CarrierDataAuditApi
- description: Access to the Employee Navigator Carrier Data Sync API service.
  flows: []
  scope: CarrierDataSyncApi
- description: Access to the Employee Navigator Quote Census API service.
  flows: []
  scope: QuoteCensusApi
- description: Access to the Employee Navigator Agency Management API service.
  flows: []
  scope: AgencyManagementApi
- description: Access to the Employee Navigator Quoting Company Integration API service.
  flows: []
  scope: QuotingCompanyIntegrationApi
- description: Access to the Employee Navigator Quoting Configuration API service.
  flows: []
  scope: QuotingConfigurationApi
- description: Access to the Employee Navigator Quoting Notification API service.
  flows: []
  scope: QuotingNotificationApi
- description: Access to the Employee Navigator Quoting Push Notification API service.
  flows: []
  scope: QuotingPushNotificationApi
- description: Access to the Employee Navigator Agency Configuration API service.
  flows: []
  scope: AgencyConfigurationApi
- description: Access to the Employee Navigator Agency Notification API service.
  flows: []
  scope: AgencyNotificationApi
- description: Access to the Employee Navigator Payroll Company Integration API service.
  flows: []
  scope: PayrollCompanyIntegrationApi
- description: Access to the Employee Navigator Payroll Employee Notification API service.
  flows: []
  scope: PayrollEmployeeNotificationApi
- description: Access to the Employee Navigator Payroll Notification API service.
  flows: []
  scope: PayrollNotificationApi
- description: Access to the Employee Navigator Carrier Member Benefit API service.
  flows: []
  scope: CarrierMemberBenefitApi
- description: Access to the Employee Navigator Evidence Of Insurability API service.
  flows: []
  scope: EvidenceOfInsurabilityApi
- description: Access to the Employee Navigator Evidence Of Insurability Notification API service.
  flows: []
  scope: EvidenceOfInsurabilityNotificationApi
- description: Access to the Employee Navigator Employee Benefits Management API service.
  flows: []
  scope: EmployeeBenefitsManagementApi
- description: Access to the Employee Navigator Rates Service API service.
  flows: []
  scope: RatesServiceApi
- description: Access to the Employee Navigator Webhook API service.
  flows: []
  scope: WebhookApi
- description: Access to the Employee Navigator Company Management API service.
  flows: []
  scope: CompanyManagementApi
- description: Access to the Employee Navigator Company Configuration API service.
  flows: []
  scope: CompanyConfigurationApi
- description: Access to the Employee Navigator Plan List Configuration API service.
  flows: []
  scope: PlanListConfigurationApi
- description: Access to the Employee Navigator Plan List Management API service.
  flows: []
  scope: PlanListManagementApi
- description: Access to the Employee Navigator Health Plan Configuration API service.
  flows: []
  scope: HealthPlanConfigurationApi
- description: Access to the Employee Navigator Supplemental Plan Configuration API service.
  flows: []
  scope: SupplementalPlanConfigurationApi
- description: Access to the Employee Navigator Medical Savings Plan Configuration API service.
  flows: []
  scope: MedicalSavingsPlanConfigurationApi
- description: Access to the Employee Navigator Voluntary Life Plan Configuration API service.
  flows: []
  scope: VoluntaryLifePlanConfigurationApi
- description: Access to the Employee Navigator Voluntary Disability Plan Configuration API service.
  flows: []
  scope: VoluntaryDisabilityPlanConfigurationApi
- description: Access to the Employee Navigator Employee Profile API service.
  flows: []
  scope: EmployeeProfileApi
- description: Access to the Employee Navigator Employee Profile Configuration API service.
  flows: []
  scope: EmployeeProfileConfigurationApi
- description: Access to the Employee Navigator Employee Profile Management API service.
  flows: []
  scope: EmployeeProfileManagementApi
- description: Access to the Employee Navigator Employee Profile Payroll API service.
  flows: []
  scope: EmployeeProfilePayrollApi
- description: Access to the Employee Navigator Employee Profile Payroll Configuration API service.
  flows: []
  scope: EmployeeProfilePayrollConfigurationApi
- description: Access to the Employee Navigator Employee Profile Payroll Management API service.
  flows: []
  scope: EmployeeProfilePayrollManagementApi
- description: Access to the Employee Navigator Health Plan Management API service.
  flows: []
  scope: HealthPlanManagementApi
- description: Access to the Employee Navigator Supplemental Plan Management API service.
  flows: []
  scope: SupplementalPlanManagementApi
- description: Access to the Employee Navigator Group Life Plan Configuration API service.
  flows: []
  scope: GroupLifePlanConfigurationApi
- description: Access to the Employee Navigator Ease Migration API service.
  flows: []
  scope: EaseMigrationApi
- description: Access to the Employee Navigator Group Disability Plan Configuration API service.
  flows: []
  scope: GroupDisabilityPlanConfigurationApi
- description: Access to the Employee Navigator Group Life Plan Management API service.
  flows: []
  scope: GroupLifePlanManagementApi
- description: Access to the Employee Navigator Voluntary Life Plan Management API service.
  flows: []
  scope: VoluntaryLifePlanManagementApi
- description: Access to the Employee Navigator Group Disability Plan Management API service.
  flows: []
  scope: GroupDisabilityPlanManagementApi
- description: Access to the Employee Navigator Cafeteria Plan Management API service.
  flows: []
  scope: CafeteriaPlanManagementApi
- description: Access to the Employee Navigator Cafeteria Plan Configuration API service.
  flows: []
  scope: CafeteriaPlanConfigurationApi
- description: Access to the Employee Navigator Voluntary Disability Plan Management API service.
  flows: []
  scope: VoluntaryDisabilityPlanManagementApi
- description: Access to the Employee Navigator Paycor Company Integration API service.
  flows: []
  scope: PaycorCompanyIntegrationApi
- description: Access to the Employee Navigator Carrier List Management API service.
  flows: []
  scope: CarrierListManagementApi
- description: Access to the Employee Navigator Company Identifier Replacement API service.
  flows: []
  scope: CompanyIdentifierReplacementApi
- description: OpenID Connect standard scope; requests a refresh token for long-lived unattended access.
  flows: []
  scope: offline_access
slug: employeenavigator-scopes
source_filename: employeenavigator-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://www.employeenavigator.com/identity/.well-known/openid-configuration\ndocs: https://www.employeenavigator.com/security/\nnotes: >-\n  The 66 scopes below are the complete scopes_supported array published\n  anonymously by Employee Navigator's OpenID Connect discovery document. They are\n  recorded verbatim; the human-readable descriptions are API Evangelist\n  expansions of the scope name, not provider copy — Employee Navigator publishes\n  no public scope reference page. Each non-standard scope names a distinct\n  Employee Navigator API service, which is the clearest public map of the\n  partner API surface available without partner credentials.\nschemes:\n- name: OAuth2\n  source: well-known/employeenavigator-openid-configuration.json\n  issuer: https://www.employeenavigator.com/identity\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.employeenavigator.com/identity/connect/authorize\n    tokenUrl:\
  \ https://www.employeenavigator.com/identity/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://www.employeenavigator.com/identity/connect/token\ngroups:\n- id: agency\n  description: \"Agency management system services — agency management, configuration and notifications.\"\n  scope_count: 3\n- id: carrier\n  description: \"Insurance carrier partner services — company integration and connection, configuration, notifications, push notifications, data audit, data sync, member benefit and carrier list management.\"\n  scope_count: 9\n- id: cobra\n  description: \"COBRA administration configuration and notification services.\"\n  scope_count: 2\n- id: company\n  description: \"Company management, company configuration and company identifier replacement services.\"\n  scope_count: 3\n- id: employee-benefits\n  description: \"Employee benefits management service.\"\n  scope_count: 1\n- id: employee-profile\n  description: \"Employee profile read, configuration, management and\
  \ the payroll-facing employee profile services.\"\n  scope_count: 6\n- id: evidence-of-insurability\n  description: \"Evidence of Insurability (EOI) services and their notifications.\"\n  scope_count: 2\n- id: master\n  description: \"Master (Employee Navigator platform tenant) services — company integration, configuration, notification, push notification, data audit and data sync.\"\n  scope_count: 6\n- id: migration\n  description: \"Ease platform migration service.\"\n  scope_count: 1\n- id: oidc-standard\n  description: \"OpenID Connect standard scopes.\"\n  scope_count: 4\n- id: payroll\n  description: \"Payroll partner services — company integration, employee notification and payroll notifications, including the named Paycor company integration.\"\n  scope_count: 4\n- id: plan\n  description: \"Plan list, health, supplemental, medical savings, cafeteria, group life, group disability, voluntary life and voluntary disability plan configuration and management services.\"\n  scope_count:\
  \ 17\n- id: platform\n  description: \"General Employee Navigator platform API scope.\"\n  scope_count: 1\n- id: quoting\n  description: \"Quoting engine services — quote census, company integration, configuration, notifications and push notifications.\"\n  scope_count: 5\n- id: rates\n  description: \"Benefit rates service.\"\n  scope_count: 1\n- id: webhooks\n  description: \"Webhook subscription and delivery management service.\"\n  scope_count: 1\nscope_count: 66\nscopes:\n- scope: openid\n  description: \"OpenID Connect standard scope; requests an ID token for the authenticated subject.\"\n  group: oidc-standard\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: profile\n  description: \"OpenID Connect standard scope; requests the profile claim set (name, family_name, given_name, nickname, birthdate, locale and related claims).\"\n  group: oidc-standard\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: email\n  description:\
  \ \"OpenID Connect standard scope; requests the email and email_verified claims.\"\n  group: oidc-standard\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EnApi\n  description: \"Access to the Employee Navigator En API service.\"\n  group: platform\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MasterCompanyIntegrationApi\n  description: \"Access to the Employee Navigator Master Company Integration API service.\"\n  group: master\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MasterConfigurationApi\n  description: \"Access to the Employee Navigator Master Configuration API service.\"\n  group: master\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MasterNotificationApi\n  description: \"Access to the Employee Navigator Master Notification API service.\"\n  group: master\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MasterPushNotificationApi\n\
  \  description: \"Access to the Employee Navigator Master Push Notification API service.\"\n  group: master\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MasterDataAuditApi\n  description: \"Access to the Employee Navigator Master Data Audit API service.\"\n  group: master\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MasterDataSyncApi\n  description: \"Access to the Employee Navigator Master Data Sync API service.\"\n  group: master\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CobraConfigurationApi\n  description: \"Access to the Employee Navigator Cobra Configuration API service.\"\n  group: cobra\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CobraNotificationApi\n  description: \"Access to the Employee Navigator Cobra Notification API service.\"\n  group: cobra\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierCompanyIntegrationApi\n\
  \  description: \"Access to the Employee Navigator Carrier Company Integration API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierCompanyIntegrationConnectionApi\n  description: \"Access to the Employee Navigator Carrier Company Integration Connection API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierConfigurationApi\n  description: \"Access to the Employee Navigator Carrier Configuration API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierNotificationApi\n  description: \"Access to the Employee Navigator Carrier Notification API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierPushNotificationApi\n  description: \"Access to the Employee Navigator Carrier Push Notification API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n\
  - scope: CarrierDataAuditApi\n  description: \"Access to the Employee Navigator Carrier Data Audit API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierDataSyncApi\n  description: \"Access to the Employee Navigator Carrier Data Sync API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: QuoteCensusApi\n  description: \"Access to the Employee Navigator Quote Census API service.\"\n  group: quoting\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: AgencyManagementApi\n  description: \"Access to the Employee Navigator Agency Management API service.\"\n  group: agency\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: QuotingCompanyIntegrationApi\n  description: \"Access to the Employee Navigator Quoting Company Integration API service.\"\n  group: quoting\n  sources: [well-known/employeenavigator-openid-configuration.json]\n\
  - scope: QuotingConfigurationApi\n  description: \"Access to the Employee Navigator Quoting Configuration API service.\"\n  group: quoting\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: QuotingNotificationApi\n  description: \"Access to the Employee Navigator Quoting Notification API service.\"\n  group: quoting\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: QuotingPushNotificationApi\n  description: \"Access to the Employee Navigator Quoting Push Notification API service.\"\n  group: quoting\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: AgencyConfigurationApi\n  description: \"Access to the Employee Navigator Agency Configuration API service.\"\n  group: agency\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: AgencyNotificationApi\n  description: \"Access to the Employee Navigator Agency Notification API service.\"\n  group: agency\n  sources: [well-known/employeenavigator-openid-configuration.json]\n\
  - scope: PayrollCompanyIntegrationApi\n  description: \"Access to the Employee Navigator Payroll Company Integration API service.\"\n  group: payroll\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: PayrollEmployeeNotificationApi\n  description: \"Access to the Employee Navigator Payroll Employee Notification API service.\"\n  group: payroll\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: PayrollNotificationApi\n  description: \"Access to the Employee Navigator Payroll Notification API service.\"\n  group: payroll\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierMemberBenefitApi\n  description: \"Access to the Employee Navigator Carrier Member Benefit API service.\"\n  group: carrier\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EvidenceOfInsurabilityApi\n  description: \"Access to the Employee Navigator Evidence Of Insurability API service.\"\n  group: evidence-of-insurability\n\
  \  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EvidenceOfInsurabilityNotificationApi\n  description: \"Access to the Employee Navigator Evidence Of Insurability Notification API service.\"\n  group: evidence-of-insurability\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EmployeeBenefitsManagementApi\n  description: \"Access to the Employee Navigator Employee Benefits Management API service.\"\n  group: employee-benefits\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: RatesServiceApi\n  description: \"Access to the Employee Navigator Rates Service API service.\"\n  group: rates\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: WebhookApi\n  description: \"Access to the Employee Navigator Webhook API service.\"\n  group: webhooks\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CompanyManagementApi\n  description: \"Access to the Employee\
  \ Navigator Company Management API service.\"\n  group: company\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CompanyConfigurationApi\n  description: \"Access to the Employee Navigator Company Configuration API service.\"\n  group: company\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: PlanListConfigurationApi\n  description: \"Access to the Employee Navigator Plan List Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: PlanListManagementApi\n  description: \"Access to the Employee Navigator Plan List Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: HealthPlanConfigurationApi\n  description: \"Access to the Employee Navigator Health Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: SupplementalPlanConfigurationApi\n\
  \  description: \"Access to the Employee Navigator Supplemental Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: MedicalSavingsPlanConfigurationApi\n  description: \"Access to the Employee Navigator Medical Savings Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: VoluntaryLifePlanConfigurationApi\n  description: \"Access to the Employee Navigator Voluntary Life Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: VoluntaryDisabilityPlanConfigurationApi\n  description: \"Access to the Employee Navigator Voluntary Disability Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EmployeeProfileApi\n  description: \"Access to the Employee Navigator Employee Profile API service.\"\n  group:\
  \ employee-profile\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EmployeeProfileConfigurationApi\n  description: \"Access to the Employee Navigator Employee Profile Configuration API service.\"\n  group: employee-profile\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EmployeeProfileManagementApi\n  description: \"Access to the Employee Navigator Employee Profile Management API service.\"\n  group: employee-profile\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EmployeeProfilePayrollApi\n  description: \"Access to the Employee Navigator Employee Profile Payroll API service.\"\n  group: employee-profile\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EmployeeProfilePayrollConfigurationApi\n  description: \"Access to the Employee Navigator Employee Profile Payroll Configuration API service.\"\n  group: employee-profile\n  sources: [well-known/employeenavigator-openid-configuration.json]\n\
  - scope: EmployeeProfilePayrollManagementApi\n  description: \"Access to the Employee Navigator Employee Profile Payroll Management API service.\"\n  group: employee-profile\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: HealthPlanManagementApi\n  description: \"Access to the Employee Navigator Health Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: SupplementalPlanManagementApi\n  description: \"Access to the Employee Navigator Supplemental Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: GroupLifePlanConfigurationApi\n  description: \"Access to the Employee Navigator Group Life Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: EaseMigrationApi\n  description: \"Access to the Employee Navigator Ease Migration API service.\"\n \
  \ group: migration\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: GroupDisabilityPlanConfigurationApi\n  description: \"Access to the Employee Navigator Group Disability Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: GroupLifePlanManagementApi\n  description: \"Access to the Employee Navigator Group Life Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: VoluntaryLifePlanManagementApi\n  description: \"Access to the Employee Navigator Voluntary Life Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: GroupDisabilityPlanManagementApi\n  description: \"Access to the Employee Navigator Group Disability Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CafeteriaPlanManagementApi\n\
  \  description: \"Access to the Employee Navigator Cafeteria Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CafeteriaPlanConfigurationApi\n  description: \"Access to the Employee Navigator Cafeteria Plan Configuration API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: VoluntaryDisabilityPlanManagementApi\n  description: \"Access to the Employee Navigator Voluntary Disability Plan Management API service.\"\n  group: plan\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: PaycorCompanyIntegrationApi\n  description: \"Access to the Employee Navigator Paycor Company Integration API service.\"\n  group: payroll\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: CarrierListManagementApi\n  description: \"Access to the Employee Navigator Carrier List Management API service.\"\n  group: carrier\n  sources:\
  \ [well-known/employeenavigator-openid-configuration.json]\n- scope: CompanyIdentifierReplacementApi\n  description: \"Access to the Employee Navigator Company Identifier Replacement API service.\"\n  group: company\n  sources: [well-known/employeenavigator-openid-configuration.json]\n- scope: offline_access\n  description: \"OpenID Connect standard scope; requests a refresh token for long-lived unattended access.\"\n  group: oidc-standard\n  sources: [well-known/employeenavigator-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://www.employeenavigator.com/identity/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employeenavigator/refs/heads/main/scopes/employeenavigator-scopes.yml
summary_line: 66 scopes · authorizationCode/clientCredentials
tags:
- Company
- Benefits Administration
- Human Resources
- Insurance
- Employee Benefits
- Payroll
- Health Insurance
- HRIS
- Open Enrollment
- ACA Compliance
- Identity
- OpenID Connect
token_urls:
- https://www.employeenavigator.com/identity/connect/token
---
