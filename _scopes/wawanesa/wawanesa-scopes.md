---
authorization_urls:
- https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize
- https://brokerplatform.wawanesa.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Wawanesa Scopes
name_suffix: OAuth Scopes
note: Wawanesa publishes no OpenAPI and no scope/permission reference, so there is no insurance-business scope vocabulary to harvest. Every scope below was read verbatim from the `scopes_supported` array of a live discovery document on a Wawanesa host. They are STOCK IDENTITY-PLATFORM scopes — standard OIDC claims scopes on the Okta broker issuer, Okta org-management scopes on the Okta org authorization server, and stock Salesforce Experience Cloud platform scopes on the Broker Platform. None of them grants access to a quote, bind, policy, billing or claims capability; they govern broker sign-in and the vendor platforms underneath it. Recorded here so the gap is explicit rather than implied. Wawanesa's real API authorization model is defined by CSIO's API Security Standards (certified 2024-10-29), which is member-gated and does not publish its scope vocabulary publicly.
overview: 'Wawanesa Insurance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://login.brokerplatform.wawanesa.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wawanesa Insurance
provider_slug: wawanesa
schemes:
- flows:
  - authorizationUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token
  kind: openid-connect
  name: BrokerPlatformOkta
  source: well-known/wawanesa-brokerplatform-login-openid-configuration.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token
  - authorizationUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token
  kind: oauth2
  name: BrokerPlatformOktaOrgAuthorizationServer
  source: well-known/wawanesa-brokerplatform-login-oauth-authorization-server.json
- flows:
  - authorizationUrl: https://brokerplatform.wawanesa.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://brokerplatform.wawanesa.com/services/oauth2/token
  kind: openid-connect
  name: BrokerPlatformSalesforce
  source: well-known/wawanesa-brokerplatform-openid-configuration.json
scope_count: 0
scope_names: []
scopes: []
slug: wawanesa-scopes
source_filename: wawanesa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  live anonymous fetch of the OAuth 2.0 / OpenID Connect discovery documents on\n  the Wawanesa Broker Platform hosts (2026-07-25)\ndocs: null\nnote: >-\n  Wawanesa publishes no OpenAPI and no scope/permission reference, so there is\n  no insurance-business scope vocabulary to harvest. Every scope below was read\n  verbatim from the `scopes_supported` array of a live discovery document on a\n  Wawanesa host. They are STOCK IDENTITY-PLATFORM scopes — standard OIDC claims\n  scopes on the Okta broker issuer, Okta org-management scopes on the Okta org\n  authorization server, and stock Salesforce Experience Cloud platform scopes on\n  the Broker Platform. None of them grants access to a quote, bind, policy,\n  billing or claims capability; they govern broker sign-in and the vendor\n  platforms underneath it. Recorded here so the gap is explicit rather than\n  implied. Wawanesa's real API authorization model is defined by CSIO's\
  \ API\n  Security Standards (certified 2024-10-29), which is member-gated and does not\n  publish its scope vocabulary publicly.\nschemes:\n- name: BrokerPlatformOkta\n  source: well-known/wawanesa-brokerplatform-login-openid-configuration.json\n  kind: openid-connect\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize\n    tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token\n- name: BrokerPlatformOktaOrgAuthorizationServer\n  source: well-known/wawanesa-brokerplatform-login-oauth-authorization-server.json\n  kind: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token\n  - flow: authorizationCode\n    authorizationUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/authorize\n    tokenUrl: https://login.brokerplatform.wawanesa.com/oauth2/v1/token\n- name: BrokerPlatformSalesforce\n  source: well-known/wawanesa-brokerplatform-openid-configuration.json\n\
  \  kind: openid-connect\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://brokerplatform.wawanesa.com/services/oauth2/authorize\n    tokenUrl: https://brokerplatform.wawanesa.com/services/oauth2/token\nscope_groups:\n- group: oidc-standard\n  class: identity\n  description: Standard OpenID Connect scopes advertised by the Okta broker issuer.\n  schemes: [BrokerPlatformOkta]\n  scopes:\n  - {scope: openid, description: OpenID Connect authentication}\n  - {scope: profile, description: Basic profile claims}\n  - {scope: email, description: Email address claim}\n  - {scope: address, description: Address claim}\n  - {scope: phone, description: Phone number claim}\n  - {scope: groups, description: Group membership claims}\n  - {scope: offline_access, description: Refresh-token issuance}\n- group: okta-org-management\n  class: vendor-platform\n  description: >-\n    Okta org-administration scopes advertised by the RFC 8414 authorization\n    server metadata. These administer\
  \ the identity tenant itself, not insurance\n    data.\n  schemes: [BrokerPlatformOktaOrgAuthorizationServer]\n  scope_count: 76\n  scopes:\n  - okta.accessRequests.tasks.manage\n  - okta.accessRequests.tasks.read\n  - okta.agentPools.manage\n  - okta.agentPools.read\n  - okta.apiTokens.manage\n  - okta.apiTokens.read\n  - okta.appGrants.manage\n  - okta.appGrants.read\n  - okta.apps.manage\n  - okta.apps.read\n  - okta.behaviors.manage\n  - okta.behaviors.read\n  - okta.brands.manage\n  - okta.brands.read\n  - okta.certificateAuthorities.manage\n  - okta.certificateAuthorities.read\n  - okta.clients.manage\n  - okta.clients.read\n  - okta.clients.register\n  - okta.directories.groups.manage\n  - okta.directories.manage\n  - okta.domains.manage\n  - okta.domains.read\n  - okta.eventHooks.manage\n  - okta.eventHooks.read\n  - okta.events.read\n  - okta.factors.manage\n  - okta.factors.read\n  - okta.features.manage\n  - okta.features.read\n  - okta.governance.assignmentCandidates.read\n\
  \  - okta.groups.manage\n  - okta.groups.read\n  - okta.idps.manage\n  - okta.idps.read\n  - okta.inlineHooks.manage\n  - okta.inlineHooks.read\n  - okta.linkedObjects.manage\n  - okta.linkedObjects.read\n  - okta.logs.read\n  - okta.networkZones.manage\n  - okta.networkZones.read\n  - okta.orgs.manage\n  - okta.orgs.read\n  - okta.personal.adminSettings.manage\n  - okta.personal.adminSettings.read\n  - okta.policies.manage\n  - okta.policies.read\n  - okta.principalRateLimits.manage\n  - okta.principalRateLimits.read\n  - okta.profileMappings.manage\n  - okta.profileMappings.read\n  - okta.rateLimits.manage\n  - okta.rateLimits.read\n  - okta.reports.manage\n  - okta.reports.read\n  - okta.riskProviders.manage\n  - okta.riskProviders.read\n  - okta.roles.manage\n  - okta.roles.read\n  - okta.schemas.manage\n  - okta.schemas.read\n  - okta.sessions.manage\n  - okta.sessions.read\n  - okta.templates.manage\n  - okta.templates.read\n  - okta.threatInsights.manage\n  - okta.threatInsights.read\n\
  \  - okta.trustedOrigins.manage\n  - okta.trustedOrigins.read\n  - okta.userTypes.manage\n  - okta.userTypes.read\n  - okta.users.manage\n  - okta.users.manage.self\n  - okta.users.read\n  - okta.users.read.self\n- group: salesforce-platform\n  class: vendor-platform\n  description: >-\n    Stock Salesforce Experience Cloud scopes advertised by the Broker Platform\n    OIDC document. Generic platform capabilities (API access, Chatter, Data\n    Cloud, Einstein), not Wawanesa insurance permissions.\n  schemes: [BrokerPlatformSalesforce]\n  scope_count: 36\n  scopes:\n  - address\n  - api\n  - cdp_api\n  - cdp_calculated_insight_api\n  - cdp_identityresolution_api\n  - cdp_ingest_api\n  - cdp_profile_api\n  - cdp_query_api\n  - cdp_segment_api\n  - chatbot_api\n  - chatter_api\n  - content\n  - custom_permissions\n  - data_cloud_user_claims\n  - eclair_api\n  - einstein_gpt_api\n  - email\n  - forgot_password\n  - full\n  - id\n  - interaction_api\n  - lightning\n  - mcp_api\n  - offline_access\n\
  \  - openid\n  - pardot_api\n  - phone\n  - profile\n  - pwdless_login_api\n  - refresh_token\n  - scrt_api\n  - sfap_api\n  - user_registration_api\n  - visualforce\n  - wave_api\n  - web\nbusiness_scopes:\n  published: false\n  note: >-\n    No quote/bind/policy/billing/claims scope vocabulary is published by\n    Wawanesa or reachable anonymously. Insurance-capability authorization is\n    governed by CSIO's API Security Standards inside the broker channel.\nrelated:\n  authentication: authentication/wawanesa-authentication.yml\n  well_known: well-known/wawanesa-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wawanesa/refs/heads/main/scopes/wawanesa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Canada
- Property and Casualty
- Carrier
- Mutual Insurer
- Brokers
- Commercial Lines
- Personal Lines
- Underwriting
- Claims
- Policy Administration
- CSIO
- Partner Gated
token_urls:
- https://login.brokerplatform.wawanesa.com/oauth2/v1/token
- https://brokerplatform.wawanesa.com/services/oauth2/token
---
