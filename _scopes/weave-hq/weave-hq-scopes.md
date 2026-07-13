---
api_specs:
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Messaging API
  slug: weave-hq-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Phone & Calls API
  slug: weave-hq-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Contacts API
  slug: weave-hq-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Scheduling & Appointments API
  slug: weave-hq-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Payments API
  slug: weave-hq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Digital Forms API
  slug: weave-hq-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Reviews API
  slug: weave-hq-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Events & Subscriptions API
  slug: weave-hq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
authorization_urls:
- https://auth.weaveconnect.com/oauth2/default/v1/authorize
description: ''
docs: https://oidc.weaveconnect.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Weave Hq Scopes
name_suffix: OAuth Scopes
note: Weave does not publish API-permission OAuth scopes - the developer portal (https://dp.getweave.com) is behind a login, and the live OIDC discovery document at https://oidc.weaveconnect.com/.well-known/openid-configuration lists only the standard OIDC scopes openid, offline, and offline_access, with access governed by the developer application rather than granular scopes.
overview: 'Weave uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.weaveconnect.com/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Weave
provider_slug: weave-hq
schemes:
- description: 'OAuth 2.0 access token issued by Weave''s OIDC provider. Authorization and token endpoints are served under https://auth.weaveconnect.com/oauth2/default (issuer https://oidc.weaveconnect.com). Present as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - authorizationUrl: https://auth.weaveconnect.com/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://auth.weaveconnect.com/oauth2/default/v1/token
  name: oauth2
  source: openapi/weave-hq-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: weave-hq-scopes
source_filename: weave-hq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weave-hq-openapi.yml\ndocs: https://oidc.weaveconnect.com/.well-known/openid-configuration\nnote: Weave does not publish API-permission OAuth scopes - the developer portal (https://dp.getweave.com)\n  is behind a login, and the live OIDC discovery document at https://oidc.weaveconnect.com/.well-known/openid-configuration\n  lists only the standard OIDC scopes openid, offline, and offline_access, with access\n  governed by the developer application rather than granular scopes.\nschemes:\n- name: oauth2\n  source: openapi/weave-hq-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.weaveconnect.com/oauth2/default/v1/authorize\n    tokenUrl: https://auth.weaveconnect.com/oauth2/default/v1/token\n  description: 'OAuth 2.0 access token issued by Weave''s OIDC provider. Authorization and token\n    endpoints are served under https://auth.weaveconnect.com/oauth2/default (issuer https://oidc.weaveconnect.com).\n\
  \    Present as `Authorization: Bearer ACCESS_TOKEN`.'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/scopes/weave-hq-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Communication
- Healthcare
- VoIP
- Messaging
- SMS
- Scheduling
- Payments
- Reviews
- Dental
- Veterinary
token_urls:
- https://auth.weaveconnect.com/oauth2/default/v1/token
---
