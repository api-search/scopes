---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sentry Insurance Group Scopes
name_suffix: OAuth Scopes
note: These are the scopes the Sentry Insurance Okta tenant (account.sentry.com) advertises in its published OIDC/OAuth 2.0 metadata. They are the stock OpenID Connect set plus Okta's myAccount self-service family and one tenant-specific scope (`interclient_access`). Sentry Insurance publishes NO scope reference page and no business-domain scopes — there is no product API for a scope to protect. Recorded verbatim from the metadata, not curated.
overview: 'Sentry Insurance publishes 25 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sentry Insurance API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sentry Insurance
provider_slug: sentry-insurance-group
schemes: []
scope_count: 25
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
- groups
- interclient_access
- okta.myAccount.manage
- okta.myAccount.read
- okta.myAccount.profile.manage
- okta.myAccount.profile.read
- okta.myAccount.email.manage
- okta.myAccount.email.read
- okta.myAccount.phone.manage
- okta.myAccount.phone.read
- okta.myAccount.authenticators.manage
- okta.myAccount.authenticators.read
- okta.myAccount.appAuthenticator.manage
- okta.myAccount.appAuthenticator.read
- okta.myAccount.appAuthenticator.maintenance.manage
- okta.myAccount.appAuthenticator.maintenance.read
- okta.myAccount.oktaApplications.read
- okta.myAccount.organization.read
scopes:
- description: OpenID Connect — request an ID token.
  flows: []
  scope: openid
- description: Basic profile claims (name, family_name, given_name, locale, zoneinfo, updated_at).
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
- description: Issue a refresh token. Observed in the live insight.sentry.com sign-in request.
  flows: []
  scope: offline_access
- description: Okta device single sign-on token.
  flows: []
  scope: device_sso
- description: Group membership claim. Advertised only by the org-level authorization server (issuer https://account.sentry.com).
  flows: []
  scope: groups
- description: Tenant-defined scope on the `default` authorization server. Sentry Insurance publishes no description of it; recorded as advertised, meaning undocumented.
  flows: []
  scope: interclient_access
- description: Manage the signed-in user's own Okta account.
  flows: []
  scope: okta.myAccount.manage
- description: Read the signed-in user's own Okta account.
  flows: []
  scope: okta.myAccount.read
- description: Manage the signed-in user's own profile.
  flows: []
  scope: okta.myAccount.profile.manage
- description: Read the signed-in user's own profile.
  flows: []
  scope: okta.myAccount.profile.read
- description: Manage the signed-in user's own email factors.
  flows: []
  scope: okta.myAccount.email.manage
- description: Read the signed-in user's own email factors.
  flows: []
  scope: okta.myAccount.email.read
- description: Manage the signed-in user's own phone factors.
  flows: []
  scope: okta.myAccount.phone.manage
- description: Read the signed-in user's own phone factors.
  flows: []
  scope: okta.myAccount.phone.read
- description: Manage the signed-in user's own authenticators.
  flows: []
  scope: okta.myAccount.authenticators.manage
- description: Read the signed-in user's own authenticators.
  flows: []
  scope: okta.myAccount.authenticators.read
- description: Manage the signed-in user's own app authenticator enrollment.
  flows: []
  scope: okta.myAccount.appAuthenticator.manage
- description: Read the signed-in user's own app authenticator enrollment.
  flows: []
  scope: okta.myAccount.appAuthenticator.read
- description: Manage app authenticator maintenance operations.
  flows: []
  scope: okta.myAccount.appAuthenticator.maintenance.manage
- description: Read app authenticator maintenance state.
  flows: []
  scope: okta.myAccount.appAuthenticator.maintenance.read
- description: Read the applications assigned to the signed-in user.
  flows: []
  scope: okta.myAccount.oktaApplications.read
- description: Read organization metadata visible to the signed-in user.
  flows: []
  scope: okta.myAccount.organization.read
slug: sentry-insurance-group-scopes
source_filename: sentry-insurance-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://account.sentry.com/oauth2/default/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes the Sentry Insurance Okta tenant (account.sentry.com) advertises in\n  its published OIDC/OAuth 2.0 metadata. They are the stock OpenID Connect set plus Okta's\n  myAccount self-service family and one tenant-specific scope (`interclient_access`).\n  Sentry Insurance publishes NO scope reference page and no business-domain scopes — there\n  is no product API for a scope to protect. Recorded verbatim from the metadata, not curated.\nissuer: https://account.sentry.com/oauth2/default\nscope_count: 25\nscopes:\n  - name: openid\n    description: OpenID Connect — request an ID token.\n    standard: OpenID Connect Core 1.0\n  - name: profile\n    description: Basic profile claims (name, family_name, given_name, locale, zoneinfo, updated_at).\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description:\
  \ email and email_verified claims.\n    standard: OpenID Connect Core 1.0\n  - name: address\n    description: address claim.\n    standard: OpenID Connect Core 1.0\n  - name: phone\n    description: phone_number and phone_number_verified claims.\n    standard: OpenID Connect Core 1.0\n  - name: offline_access\n    description: Issue a refresh token. Observed in the live insight.sentry.com sign-in request.\n    standard: OpenID Connect Core 1.0\n  - name: device_sso\n    description: Okta device single sign-on token.\n    standard: Okta\n  - name: groups\n    description: Group membership claim. Advertised only by the org-level authorization server (issuer https://account.sentry.com).\n    standard: Okta\n  - name: interclient_access\n    description: >-\n      Tenant-defined scope on the `default` authorization server. Sentry Insurance publishes\n      no description of it; recorded as advertised, meaning undocumented.\n    standard: tenant-specific\n  - name: okta.myAccount.manage\n\
  \    description: Manage the signed-in user's own Okta account.\n    standard: Okta myAccount\n  - name: okta.myAccount.read\n    description: Read the signed-in user's own Okta account.\n    standard: Okta myAccount\n  - name: okta.myAccount.profile.manage\n    description: Manage the signed-in user's own profile.\n    standard: Okta myAccount\n  - name: okta.myAccount.profile.read\n    description: Read the signed-in user's own profile.\n    standard: Okta myAccount\n  - name: okta.myAccount.email.manage\n    description: Manage the signed-in user's own email factors.\n    standard: Okta myAccount\n  - name: okta.myAccount.email.read\n    description: Read the signed-in user's own email factors.\n    standard: Okta myAccount\n  - name: okta.myAccount.phone.manage\n    description: Manage the signed-in user's own phone factors.\n    standard: Okta myAccount\n  - name: okta.myAccount.phone.read\n    description: Read the signed-in user's own phone factors.\n    standard: Okta myAccount\n\
  \  - name: okta.myAccount.authenticators.manage\n    description: Manage the signed-in user's own authenticators.\n    standard: Okta myAccount\n  - name: okta.myAccount.authenticators.read\n    description: Read the signed-in user's own authenticators.\n    standard: Okta myAccount\n  - name: okta.myAccount.appAuthenticator.manage\n    description: Manage the signed-in user's own app authenticator enrollment.\n    standard: Okta myAccount\n  - name: okta.myAccount.appAuthenticator.read\n    description: Read the signed-in user's own app authenticator enrollment.\n    standard: Okta myAccount\n  - name: okta.myAccount.appAuthenticator.maintenance.manage\n    description: Manage app authenticator maintenance operations.\n    standard: Okta myAccount\n  - name: okta.myAccount.appAuthenticator.maintenance.read\n    description: Read app authenticator maintenance state.\n    standard: Okta myAccount\n  - name: okta.myAccount.oktaApplications.read\n    description: Read the applications assigned\
  \ to the signed-in user.\n    standard: Okta myAccount\n  - name: okta.myAccount.organization.read\n    description: Read organization metadata visible to the signed-in user.\n    standard: Okta myAccount\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentry-insurance-group/refs/heads/main/scopes/sentry-insurance-group-scopes.yml
summary_line: 25 scopes
tags:
- Fortune 1000
- Insurance
- Property and Casualty Insurance
- Commercial Insurance
- Workers Compensation
- Auto Insurance
- Retirement
- Annuities
- Mutual Insurance
- Financial Services
- Trucking
- Wisconsin
- United States
token_bound: false
token_urls: []
---
