---
authorization_urls: []
description: The 35 scopes advertised by the Troy Medicare provider-portal authorization server's OpenID Connect discovery document. Troy Medicare publishes no scope reference page, so descriptions below are left empty rather than invented; only the six standard OIDC scopes and offline_access carry their specification-defined meaning. The remainder are resource scopes of the underlying health-plan administration platform and their semantics are not publicly documented.
docs: none
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Troy Medicare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Troy Medicare publishes 35 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Troy Medicare API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Troy Medicare
provider_slug: troy-medicare
schemes: []
scope_count: 35
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- role
- McAppUserProfile
- BenefitAdminResource
- NhCommercial
- IdentityManager
- nh_web_resource
- nh_pcmweb_resource
- CustomerService
- BrokerPortal
- MemberPortal
- BrokerComm
- Correspondence
- EnrFileProcess
- Enrollment
- BillingAndPayments
- PriorAuth
- AdminPortal
- AdministrationService
- AuthServer
- SaasService
- NirvanaHealth
- IdentityService
- FaxQueue
- NhCore
- DMR
- M3P
- ClaimCore
- ProductService
- MedicalPayment
scopes:
- description: Request an ID token (OpenID Connect authentication).
  flows: []
  scope: openid
- description: End-user profile claims (name, family_name, given_name, picture, preferred_username, and similar).
  flows: []
  scope: profile
- description: email and email_verified claims.
  flows: []
  scope: email
- description: address claim.
  flows: []
  scope: address
- description: phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Issue a refresh token for access when the end user is not present.
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: role
- description: ''
  flows: []
  scope: McAppUserProfile
- description: ''
  flows: []
  scope: BenefitAdminResource
- description: ''
  flows: []
  scope: NhCommercial
- description: ''
  flows: []
  scope: IdentityManager
- description: ''
  flows: []
  scope: nh_web_resource
- description: ''
  flows: []
  scope: nh_pcmweb_resource
- description: ''
  flows: []
  scope: CustomerService
- description: ''
  flows: []
  scope: BrokerPortal
- description: ''
  flows: []
  scope: MemberPortal
- description: ''
  flows: []
  scope: BrokerComm
- description: ''
  flows: []
  scope: Correspondence
- description: ''
  flows: []
  scope: EnrFileProcess
- description: ''
  flows: []
  scope: Enrollment
- description: ''
  flows: []
  scope: BillingAndPayments
- description: ''
  flows: []
  scope: PriorAuth
- description: ''
  flows: []
  scope: AdminPortal
- description: ''
  flows: []
  scope: AdministrationService
- description: ''
  flows: []
  scope: AuthServer
- description: ''
  flows: []
  scope: SaasService
- description: ''
  flows: []
  scope: NirvanaHealth
- description: ''
  flows: []
  scope: IdentityService
- description: ''
  flows: []
  scope: FaxQueue
- description: ''
  flows: []
  scope: NhCore
- description: ''
  flows: []
  scope: DMR
- description: ''
  flows: []
  scope: M3P
- description: ''
  flows: []
  scope: ClaimCore
- description: ''
  flows: []
  scope: ProductService
- description: ''
  flows: []
  scope: MedicalPayment
slug: troy-medicare-scopes
source_filename: troy-medicare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Troy Medicare OAuth Scopes\ngenerated: '2026-08-30'\nmethod: probed\nsource: https://provider.troymedicare.com/.well-known/openid-configuration (HTTP 200, fetched 2026-08-30)\ndescription: >-\n  The 35 scopes advertised by the Troy Medicare provider-portal authorization server's OpenID\n  Connect discovery document. Troy Medicare publishes no scope reference page, so descriptions\n  below are left empty rather than invented; only the six standard OIDC scopes and offline_access\n  carry their specification-defined meaning. The remainder are resource scopes of the underlying\n  health-plan administration platform and their semantics are not publicly documented.\nauthorization_server: https://provider.troymedicare.com\ndocs: none\nscope_count: 35\nscopes:\n- name: openid\n  standard: OIDC Core 1.0\n  description: Request an ID token (OpenID Connect authentication).\n- name: profile\n  standard: OIDC Core 1.0\n  description: End-user profile claims (name, family_name, given_name,\
  \ picture, preferred_username, and similar).\n- name: email\n  standard: OIDC Core 1.0\n  description: email and email_verified claims.\n- name: address\n  standard: OIDC Core 1.0\n  description: address claim.\n- name: phone\n  standard: OIDC Core 1.0\n  description: phone_number and phone_number_verified claims.\n- name: offline_access\n  standard: OIDC Core 1.0\n  description: Issue a refresh token for access when the end user is not present.\n- name: role\n  description: ''\n- name: McAppUserProfile\n  description: ''\n- name: BenefitAdminResource\n  description: ''\n- name: NhCommercial\n  description: ''\n- name: IdentityManager\n  description: ''\n- name: nh_web_resource\n  description: ''\n- name: nh_pcmweb_resource\n  description: ''\n- name: CustomerService\n  description: ''\n- name: BrokerPortal\n  description: ''\n- name: MemberPortal\n  description: ''\n- name: BrokerComm\n  description: ''\n- name: Correspondence\n  description: ''\n- name: EnrFileProcess\n  description:\
  \ ''\n- name: Enrollment\n  description: ''\n- name: BillingAndPayments\n  description: ''\n- name: PriorAuth\n  description: ''\n- name: AdminPortal\n  description: ''\n- name: AdministrationService\n  description: ''\n- name: AuthServer\n  description: ''\n- name: SaasService\n  description: ''\n- name: NirvanaHealth\n  description: ''\n- name: IdentityService\n  description: ''\n- name: FaxQueue\n  description: ''\n- name: NhCore\n  description: ''\n- name: DMR\n  description: ''\n- name: M3P\n  description: ''\n- name: ClaimCore\n  description: ''\n- name: ProductService\n  description: ''\n- name: MedicalPayment\n  description: ''\nclaims_supported:\n- sub\n- ChildBusinessWithLob\n- MemberAuth\n- PasswordPolicy\n- birthdate\n- family_name\n- gender\n- given_name\n- locale\n- middle_name\n- ChildBusiness\n- name\n- zoneinfo\n- website\n- updated_at\n- profile\n- nickname\n- picture\n- preferred_username\n- email\n- email_verified\n- address\n- phone_number\n- phone_number_verified\n\
  - BusinessId\n- ApplicationId\n- BusinessName\n- validation_rule\n- role\n- UserId\n- LOB\n- CapitationAdminRights\n- BusinessTrackerCode\n- CommunicationPrefrence\n- MemberId\n- PayerId\n- FaxCategories\nnotes:\n- >-\n  The FHIR authorization surface at https://fhir.troymedicare.com omits scopes_supported from its\n  discovery document, so no SMART on FHIR scope vocabulary (patient/*.read and similar) could be\n  observed. It is not recorded here rather than being assumed.\nevidence:\n- url: https://provider.troymedicare.com/.well-known/openid-configuration\n  status: 200\n- url: https://fhir.troymedicare.com/.well-known/openid-configuration\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/troy-medicare/refs/heads/main/scopes/troy-medicare-scopes.yml
summary_line: 35 scopes
tags:
- Health Insurance
- Medicare
- Medicare Advantage
- Health Plans
- Healthcare
- Pharmacy
- Care Management
- Insurance
- Identity
token_bound: false
token_urls: []
---
