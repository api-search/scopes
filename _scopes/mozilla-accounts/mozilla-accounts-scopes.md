---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mozilla Accounts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mozilla accounts publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mozilla accounts API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mozilla accounts
provider_slug: mozilla-accounts
schemes: []
scope_count: 16
scope_names:
- profile
- profile:uid
- profile:email
- profile:additionalEmails
- profile:locale
- profile:avatar
- profile:display_name
- profile:amr
- openid
- email
- clients
- oauth
- basket
- https://identity.mozilla.com/apps/oldsync
- https://identity.mozilla.com/apps/notes
- https://identity.mozilla.com/account/subscriptions
scopes:
- description: access the user's profile data.
  flows: []
  scope: profile
- description: access the user's opaque user id.
  flows: []
  scope: profile:uid
- description: access the user's email address.
  flows: []
  scope: profile:email
- description: access the user's verified secondary email addresses.
  flows: []
  scope: profile:additionalEmails
- description: access the user's locale.
  flows: []
  scope: profile:locale
- description: access the user's avatar picture.
  flows: []
  scope: profile:avatar
- description: access the user's human-readable display name.
  flows: []
  scope: profile:display_name
- description: access information about the user's authentication methods and 2FA status.
  flows: []
  scope: profile:amr
- description: request an OpenID Connect id_token.
  flows: []
  scope: openid
- description: synonym for profile:email, defined by OIDC.
  flows: []
  scope: email
- description: access the list of OAuth clients connected to a user's account.
  flows: []
  scope: clients
- description: register a new OAuth client record.
  flows: []
  scope: oauth
- description: access the user's subscription data in Basket.
  flows: []
  scope: basket
- description: access to data in Firefox Sync.
  flows: []
  scope: https://identity.mozilla.com/apps/oldsync
- description: access to data in Firefox Notes.
  flows: []
  scope: https://identity.mozilla.com/apps/notes
- description: access subscription data from Subscription Platform.
  flows: []
  scope: https://identity.mozilla.com/account/subscriptions
slug: mozilla-accounts-scopes
source_filename: mozilla-accounts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://raw.githubusercontent.com/mozilla/ecosystem-platform/master/docs/reference/oauth-details.md\nscopes:\n  - name: profile\n    description: access the user's profile data.\n  - name: profile:uid\n    description: access the user's opaque user id.\n  - name: profile:email\n    description: access the user's email address.\n  - name: profile:additionalEmails\n    description: access the user's verified secondary email addresses.\n  - name: profile:locale\n    description: access the user's locale.\n  - name: profile:avatar\n    description: access the user's avatar picture.\n  - name: profile:display_name\n    description: access the user's human-readable display name.\n  - name: profile:amr\n    description: access information about the user's authentication methods and 2FA status.\n  - name: openid\n    description: request an OpenID Connect id_token.\n  - name: email\n    description: synonym for profile:email, defined\
  \ by OIDC.\n  - name: clients\n    description: access the list of OAuth clients connected to a user's account.\n  - name: oauth\n    description: register a new OAuth client record.\n  - name: basket\n    description: access the user's subscription data in Basket.\n  - name: https://identity.mozilla.com/apps/oldsync\n    description: access to data in Firefox Sync.\n  - name: https://identity.mozilla.com/apps/notes\n    description: access to data in Firefox Notes.\n  - name: https://identity.mozilla.com/account/subscriptions\n    description: access subscription data from Subscription Platform.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mozilla-accounts/refs/heads/main/scopes/mozilla-accounts-scopes.yml
summary_line: 16 scopes
tags:
- Company
- Identity
- Authentication
- Mozilla
- Firefox
token_bound: false
token_urls: []
---
