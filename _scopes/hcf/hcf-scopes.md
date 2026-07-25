---
authorization_urls:
- https://id.hcf.com.au/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Hcf Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HCF publishes 83 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the HCF API on a user''s behalf.


  Tokens are issued from https://id.hcf.com.au/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HCF
provider_slug: hcf
schemes:
- flows:
  - authorizationUrl: https://id.hcf.com.au/oauth2/v1/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://id.hcf.com.au/oauth2/v1/token
  issuer: https://id.hcf.com.au
  name: HCF member sign-in (OIDC)
  scope_count: 7
  source: well-known/hcf-openid-configuration.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.hcf.com.au/oauth2/v1/token
  issuer: https://id.hcf.com.au
  name: Okta org authorization server
  scope_count: 76
  source: well-known/hcf-oauth-authorization-server.json
scope_count: 83
scope_names:
- openid
- email
- profile
- address
- phone
- offline_access
- groups
- okta.users.manage
- okta.users.manage.self
- okta.users.read
- okta.users.read.self
- okta.linkedObjects.manage
- okta.linkedObjects.read
- okta.profileMappings.manage
- okta.profileMappings.read
- okta.userTypes.manage
- okta.userTypes.read
- okta.clients.manage
- okta.clients.register
- okta.clients.read
- okta.appGrants.manage
- okta.appGrants.read
- okta.policies.manage
- okta.policies.read
- okta.groups.manage
- okta.groups.read
- okta.inlineHooks.manage
- okta.inlineHooks.read
- okta.eventHooks.manage
- okta.eventHooks.read
- okta.events.read
- okta.logs.read
- okta.apps.manage
- okta.apps.read
- okta.governance.assignmentCandidates.read
- okta.accessRequests.tasks.manage
- okta.accessRequests.tasks.read
- okta.schemas.manage
- okta.schemas.read
- okta.idps.manage
- okta.idps.read
- okta.factors.manage
- okta.factors.read
- okta.riskProviders.manage
- okta.riskProviders.read
- okta.roles.manage
- okta.roles.read
- okta.orgs.manage
- okta.orgs.read
- okta.domains.manage
- okta.domains.read
- okta.brands.manage
- okta.brands.read
- okta.sessions.manage
- okta.sessions.read
- okta.templates.manage
- okta.templates.read
- okta.trustedOrigins.manage
- okta.trustedOrigins.read
- okta.threatInsights.manage
- okta.threatInsights.read
- okta.behaviors.manage
- okta.behaviors.read
- okta.networkZones.manage
- okta.networkZones.read
- okta.agentPools.manage
- okta.agentPools.read
- okta.reports.manage
- okta.reports.read
- okta.features.manage
- okta.features.read
- okta.certificateAuthorities.manage
- okta.certificateAuthorities.read
- okta.principalRateLimits.manage
- okta.principalRateLimits.read
- okta.rateLimits.manage
- okta.rateLimits.read
- okta.directories.manage
- okta.directories.groups.manage
- okta.apiTokens.manage
- okta.apiTokens.read
- okta.personal.adminSettings.manage
- okta.personal.adminSettings.read
scopes:
- description: Required OIDC scope; requests an ID token for the signed-in member.
  flows: []
  scope: openid
- description: Access to the member email address and email_verified claim.
  flows: []
  scope: email
- description: Access to standard OIDC profile claims (name, given_name, family_name, locale, updated_at and similar).
  flows: []
  scope: profile
- description: Access to the address claim.
  flows: []
  scope: address
- description: Access to the phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Issues a refresh token so the session can be renewed without re-authentication.
  flows: []
  scope: offline_access
- description: Includes the member group memberships as a claim.
  flows: []
  scope: groups
- description: ''
  flows: []
  scope: okta.users.manage
- description: ''
  flows: []
  scope: okta.users.manage.self
- description: ''
  flows: []
  scope: okta.users.read
- description: ''
  flows: []
  scope: okta.users.read.self
- description: ''
  flows: []
  scope: okta.linkedObjects.manage
- description: ''
  flows: []
  scope: okta.linkedObjects.read
- description: ''
  flows: []
  scope: okta.profileMappings.manage
- description: ''
  flows: []
  scope: okta.profileMappings.read
- description: ''
  flows: []
  scope: okta.userTypes.manage
- description: ''
  flows: []
  scope: okta.userTypes.read
- description: ''
  flows: []
  scope: okta.clients.manage
- description: ''
  flows: []
  scope: okta.clients.register
- description: ''
  flows: []
  scope: okta.clients.read
- description: ''
  flows: []
  scope: okta.appGrants.manage
- description: ''
  flows: []
  scope: okta.appGrants.read
- description: ''
  flows: []
  scope: okta.policies.manage
- description: ''
  flows: []
  scope: okta.policies.read
- description: ''
  flows: []
  scope: okta.groups.manage
- description: ''
  flows: []
  scope: okta.groups.read
- description: ''
  flows: []
  scope: okta.inlineHooks.manage
- description: ''
  flows: []
  scope: okta.inlineHooks.read
- description: ''
  flows: []
  scope: okta.eventHooks.manage
- description: ''
  flows: []
  scope: okta.eventHooks.read
- description: ''
  flows: []
  scope: okta.events.read
- description: ''
  flows: []
  scope: okta.logs.read
- description: ''
  flows: []
  scope: okta.apps.manage
- description: ''
  flows: []
  scope: okta.apps.read
- description: ''
  flows: []
  scope: okta.governance.assignmentCandidates.read
- description: ''
  flows: []
  scope: okta.accessRequests.tasks.manage
- description: ''
  flows: []
  scope: okta.accessRequests.tasks.read
- description: ''
  flows: []
  scope: okta.schemas.manage
- description: ''
  flows: []
  scope: okta.schemas.read
- description: ''
  flows: []
  scope: okta.idps.manage
- description: ''
  flows: []
  scope: okta.idps.read
- description: ''
  flows: []
  scope: okta.factors.manage
- description: ''
  flows: []
  scope: okta.factors.read
- description: ''
  flows: []
  scope: okta.riskProviders.manage
- description: ''
  flows: []
  scope: okta.riskProviders.read
- description: ''
  flows: []
  scope: okta.roles.manage
- description: ''
  flows: []
  scope: okta.roles.read
- description: ''
  flows: []
  scope: okta.orgs.manage
- description: ''
  flows: []
  scope: okta.orgs.read
- description: ''
  flows: []
  scope: okta.domains.manage
- description: ''
  flows: []
  scope: okta.domains.read
- description: ''
  flows: []
  scope: okta.brands.manage
- description: ''
  flows: []
  scope: okta.brands.read
- description: ''
  flows: []
  scope: okta.sessions.manage
- description: ''
  flows: []
  scope: okta.sessions.read
- description: ''
  flows: []
  scope: okta.templates.manage
- description: ''
  flows: []
  scope: okta.templates.read
- description: ''
  flows: []
  scope: okta.trustedOrigins.manage
- description: ''
  flows: []
  scope: okta.trustedOrigins.read
- description: ''
  flows: []
  scope: okta.threatInsights.manage
- description: ''
  flows: []
  scope: okta.threatInsights.read
- description: ''
  flows: []
  scope: okta.behaviors.manage
- description: ''
  flows: []
  scope: okta.behaviors.read
- description: ''
  flows: []
  scope: okta.networkZones.manage
- description: ''
  flows: []
  scope: okta.networkZones.read
- description: ''
  flows: []
  scope: okta.agentPools.manage
- description: ''
  flows: []
  scope: okta.agentPools.read
- description: ''
  flows: []
  scope: okta.reports.manage
- description: ''
  flows: []
  scope: okta.reports.read
- description: ''
  flows: []
  scope: okta.features.manage
- description: ''
  flows: []
  scope: okta.features.read
- description: ''
  flows: []
  scope: okta.certificateAuthorities.manage
- description: ''
  flows: []
  scope: okta.certificateAuthorities.read
- description: ''
  flows: []
  scope: okta.principalRateLimits.manage
- description: ''
  flows: []
  scope: okta.principalRateLimits.read
- description: ''
  flows: []
  scope: okta.rateLimits.manage
- description: ''
  flows: []
  scope: okta.rateLimits.read
- description: ''
  flows: []
  scope: okta.directories.manage
- description: ''
  flows: []
  scope: okta.directories.groups.manage
- description: ''
  flows: []
  scope: okta.apiTokens.manage
- description: ''
  flows: []
  scope: okta.apiTokens.read
- description: ''
  flows: []
  scope: okta.personal.adminSettings.manage
- description: ''
  flows: []
  scope: okta.personal.adminSettings.read
slug: hcf-scopes
source_filename: hcf-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://id.hcf.com.au/.well-known/openid-configuration + https://id.hcf.com.au/.well-known/oauth-authorization-server\ndocs: null\nwarning: 'HCF publishes NO scope catalog for any insurance or business API, because it publishes no API.\n  Every scope below is advertised by the Okta identity tenant at id.hcf.com.au: the first group is the\n  standard OpenID Connect scope set used for member sign-in, and the second group is Okta''s stock org-management\n  scope set that every Okta org authorization server advertises whether or not the tenant grants any of\n  them. These describe the identity platform, not HCF product capabilities, and must not be read as an\n  HCF API scope catalog.'\nschemes:\n- name: HCF member sign-in (OIDC)\n  issuer: https://id.hcf.com.au\n  source: well-known/hcf-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.hcf.com.au/oauth2/v1/authorize\n    tokenUrl:\
  \ https://id.hcf.com.au/oauth2/v1/token\n    pkce: S256\n  scope_count: 7\n- name: Okta org authorization server\n  issuer: https://id.hcf.com.au\n  source: well-known/hcf-oauth-authorization-server.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.hcf.com.au/oauth2/v1/token\n  scope_count: 76\nsummary:\n  total: 83\n  oidc: 7\n  okta_org_management: 76\n  hcf_product_scopes: 0\nscopes:\n- scope: openid\n  description: Required OIDC scope; requests an ID token for the signed-in member.\n  family: oidc\n  audience: member sign-in\n  sources:\n  - well-known/hcf-openid-configuration.json\n- scope: email\n  description: Access to the member email address and email_verified claim.\n  family: oidc\n  audience: member sign-in\n  sources:\n  - well-known/hcf-openid-configuration.json\n- scope: profile\n  description: Access to standard OIDC profile claims (name, given_name, family_name, locale, updated_at\n    and similar).\n  family: oidc\n  audience: member sign-in\n  sources:\n\
  \  - well-known/hcf-openid-configuration.json\n- scope: address\n  description: Access to the address claim.\n  family: oidc\n  audience: member sign-in\n  sources:\n  - well-known/hcf-openid-configuration.json\n- scope: phone\n  description: Access to the phone_number and phone_number_verified claims.\n  family: oidc\n  audience: member sign-in\n  sources:\n  - well-known/hcf-openid-configuration.json\n- scope: offline_access\n  description: Issues a refresh token so the session can be renewed without re-authentication.\n  family: oidc\n  audience: member sign-in\n  sources:\n  - well-known/hcf-openid-configuration.json\n- scope: groups\n  description: Includes the member group memberships as a claim.\n  family: oidc\n  audience: member sign-in\n  sources:\n  - well-known/hcf-openid-configuration.json\n- scope: okta.users.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.users.manage.self\n\
  \  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.users.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.users.read.self\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.linkedObjects.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.linkedObjects.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.profileMappings.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.profileMappings.read\n\
  \  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.userTypes.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.userTypes.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.clients.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.clients.register\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.clients.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.appGrants.manage\n  family:\
  \ okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.appGrants.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.policies.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.policies.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.groups.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.groups.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.inlineHooks.manage\n  family: okta-org-management\n\
  \  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.inlineHooks.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.eventHooks.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.eventHooks.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.events.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.logs.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.apps.manage\n  family: okta-org-management\n  audience: Okta\
  \ tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.apps.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.governance.assignmentCandidates.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.accessRequests.tasks.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.accessRequests.tasks.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.schemas.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.schemas.read\n  family: okta-org-management\n\
  \  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.idps.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.idps.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.factors.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.factors.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.riskProviders.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.riskProviders.read\n  family: okta-org-management\n  audience:\
  \ Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.roles.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.roles.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.orgs.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.orgs.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.domains.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.domains.read\n  family: okta-org-management\n  audience: Okta tenant administration\n\
  \  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.brands.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.brands.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.sessions.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.sessions.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.templates.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.templates.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n\
  \  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.trustedOrigins.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.trustedOrigins.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.threatInsights.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.threatInsights.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.behaviors.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.behaviors.read\n  family: okta-org-management\n  audience: Okta tenant administration\n\
  \  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.networkZones.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.networkZones.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.agentPools.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.agentPools.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.reports.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.reports.read\n  family: okta-org-management\n  audience: Okta tenant administration\n\
  \  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.features.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.features.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.certificateAuthorities.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.certificateAuthorities.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.principalRateLimits.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.principalRateLimits.read\n  family: okta-org-management\n\
  \  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.rateLimits.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.rateLimits.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.directories.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.directories.groups.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.apiTokens.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.apiTokens.read\n  family: okta-org-management\n\
  \  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.personal.adminSettings.manage\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n- scope: okta.personal.adminSettings.read\n  family: okta-org-management\n  audience: Okta tenant administration\n  sources:\n  - well-known/hcf-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcf/refs/heads/main/scopes/hcf-scopes.yml
summary_line: 83 scopes · authorizationCode/clientCredentials
tags:
- Insurance
- Australia
- Health Insurance
- Life Insurance
- Travel Insurance
- Pet Insurance
- Carrier
- Not-for-Profit
- Claims
- Member Services
- Partner Gated
- No Public API
token_urls:
- https://id.hcf.com.au/oauth2/v1/token
---
