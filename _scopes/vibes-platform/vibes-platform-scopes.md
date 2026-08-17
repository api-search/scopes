---
api_specs:
- filename: vibes-platform-api-openapi.json
  format: json
  label: Vibes Platform API
  slug: vibes-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-api-openapi.json
- filename: vibes-platform-rcs-business-messaging-openapi.json
  format: json
  label: Vibes RCS Business Messaging API
  slug: vibes-rcs-business-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-rcs-business-messaging-openapi.json
- filename: vibes-platform-acquisition-campaigns-api-openapi.yml
  format: yaml
  label: Vibes Platform Acquisition Campaigns API
  slug: vibes-platform-acquisition-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-acquisition-campaigns-api-openapi.yml
- filename: vibes-platform-broadcasts-api-openapi.yml
  format: yaml
  label: Vibes Platform Broadcasts API
  slug: vibes-platform-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-broadcasts-api-openapi.yml
- filename: vibes-platform-callbacks-api-openapi.yml
  format: yaml
  label: Vibes Platform Callbacks API
  slug: vibes-platform-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-callbacks-api-openapi.yml
- filename: vibes-platform-carrier-lookup-api-openapi.yml
  format: yaml
  label: Vibes Platform Carrier Lookup API
  slug: vibes-platform-carrier-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-carrier-lookup-api-openapi.yml
- filename: vibes-platform-events-api-openapi.yml
  format: yaml
  label: Vibes Platform Events API
  slug: vibes-platform-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-events-api-openapi.yml
- filename: vibes-platform-inbound-messages-api-openapi.yml
  format: yaml
  label: Vibes Platform Inbound Messages API
  slug: vibes-platform-inbound-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-inbound-messages-api-openapi.yml
- filename: vibes-platform-messages-api-openapi.yml
  format: yaml
  label: Vibes Platform Messages API
  slug: vibes-platform-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-messages-api-openapi.yml
- filename: vibes-platform-persons-api-openapi.yml
  format: yaml
  label: Vibes Platform Persons API
  slug: vibes-platform-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-persons-api-openapi.yml
- filename: vibes-platform-subscription-lists-api-openapi.yml
  format: yaml
  label: Vibes Platform Subscription Lists API
  slug: vibes-platform-subscription-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-subscription-lists-api-openapi.yml
- filename: vibes-platform-wallet-passes-api-openapi.yml
  format: yaml
  label: Vibes Platform Wallet Passes API
  slug: vibes-platform-wallet-passes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/openapi/vibes-platform-wallet-passes-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Vibes Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vibes Platform publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vibes Platform API on a user''s behalf.


  Tokens are issued from https://vibes-rbm-prd.auth.us-west-2.amazoncognito.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vibes Platform
provider_slug: vibes-platform
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://vibes-rbm-prd.auth.us-west-2.amazoncognito.com/oauth2/token
  name: OAuth2Auth
  source: openapi/vibes-platform-rcs-business-messaging-openapi.json
scope_count: 1
scope_names:
- https://rbm.vibes.com/rbm.agents
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: https://rbm.vibes.com/rbm.agents
slug: vibes-platform-scopes
source_filename: vibes-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/vibes-platform-rcs-business-messaging-openapi.json\nschemes:\n- name: OAuth2Auth\n  source: openapi/vibes-platform-rcs-business-messaging-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://vibes-rbm-prd.auth.us-west-2.amazoncognito.com/oauth2/token\nscopes:\n- scope: https://rbm.vibes.com/rbm.agents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/vibes-platform-rcs-business-messaging-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vibes-platform/refs/heads/main/scopes/vibes-platform-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Mobile Marketing
- Mobile Messaging
- Push Notifications
- SMS
- MMS
- Broadcast Messaging
- Acquisition Campaigns
- Subscription Management
- Wallet Passes
- RCS
token_urls:
- https://vibes-rbm-prd.auth.us-west-2.amazoncognito.com/oauth2/token
---
