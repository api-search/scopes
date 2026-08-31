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
overview: 'Sentry Insurance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sentry Insurance
provider_slug: sentry-insurance-group
schemes: []
scope_count: 0
scope_names: []
scopes: []
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
summary_line: OAuth 2.0 · no documented scopes
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
token_urls: []
---
