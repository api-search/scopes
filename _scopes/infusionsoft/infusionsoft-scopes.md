---
api_specs:
- filename: infusionsoft-rest-v2-openapi.json
  format: json
  label: Keap REST API v2
  slug: rest-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/openapi/infusionsoft-rest-v2-openapi.json
- filename: infusionsoft-rest-v1-openapi.json
  format: json
  label: Keap REST API v1
  slug: rest-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/openapi/infusionsoft-rest-v1-openapi.json
- filename: infusionsoft-pipelines-openapi.yml
  format: yaml
  label: Keap Pipelines API
  slug: pipelines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/openapi/infusionsoft-pipelines-openapi.yml
authorization_urls:
- https://accounts.infusionsoft.com/app/oauth/authorize
description: ''
docs: https://developer.keap.com/getting-started-oauth-keys/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Infusionsoft Scopes
name_suffix: OAuth Scopes
note: 'Keap runs OAuth 2.0 with NO granular scope model. The authorize endpoint accepts a scope parameter whose only valid value is `full`, and every spec declares the oauth2 scheme with an empty scopes object - so a user authorising an integration grants complete access to their CRM, and there is no way for an application to request less. There is no read-only grant, no per-resource scope, and no incremental consent. Service Account Keys are worse: they carry administrator access to all stored data by construction. For an agent this is the single highest-risk property of the Keap API - a token that can list contacts can also delete orders and cancel subscriptions.'
overview: 'Infusionsoft (Keap) uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.infusionsoft.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Infusionsoft (Keap)
provider_slug: infusionsoft
schemes:
- flows:
  - authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize
    declared_scopes: 0
    flow: authorizationCode
    tokenUrl: https://api.infusionsoft.com/token
  name: oauth2
  source: openapi/infusionsoft-rest-v1-openapi.json
- flows:
  - authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize
    declared_scopes: 0
    flow: authorizationCode
    tokenUrl: https://api.infusionsoft.com/token
  name: oauth2
  source: openapi/infusionsoft-rest-v2-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: infusionsoft-scopes
source_filename: infusionsoft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.keap.com/getting-started-oauth-keys/, https://developer.keap.com/pat-and-sak/,\n  openapi/infusionsoft-rest-v1-openapi.json, openapi/infusionsoft-rest-v2-openapi.json\ndocs: https://developer.keap.com/getting-started-oauth-keys/\nnote: 'Keap runs OAuth 2.0 with NO granular scope model. The authorize endpoint accepts a scope parameter\n  whose only valid value is `full`, and every spec declares the oauth2 scheme with an empty scopes object\n  - so a user authorising an integration grants complete access to their CRM, and there is no way for\n  an application to request less. There is no read-only grant, no per-resource scope, and no incremental\n  consent. Service Account Keys are worse: they carry administrator access to all stored data by construction.\n  For an agent this is the single highest-risk property of the Keap API - a token that can list contacts\n  can also delete orders and cancel subscriptions.'\n\
  model: all-or-nothing\nscope_count: 1\nscopes:\n- name: full\n  description: 'Complete access to the authorising Keap application: read and write across contacts, companies,\n    tags, opportunities, orders, products, subscriptions, emails, automations, affiliates and settings.'\n  source: https://developer.keap.com/getting-started-oauth-keys/\ngranular_scopes: false\nleast_privilege_alternative: A Personal Access Token created by a limited (non-admin) user is the ONLY\n  way to narrow effective access, because a PAT inherits that user visibility and editing permissions.\n  This is a user-permission workaround, not an API scope.\nschemes:\n- name: oauth2\n  source: openapi/infusionsoft-rest-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize\n    tokenUrl: https://api.infusionsoft.com/token\n    declared_scopes: 0\n- name: oauth2\n  source: openapi/infusionsoft-rest-v2-openapi.json\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize\n    tokenUrl: https://api.infusionsoft.com/token\n    declared_scopes: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infusionsoft/refs/heads/main/scopes/infusionsoft-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CRM
- Marketing Automation
- Sales Automation
- Email Marketing
- E-Commerce
- Small Business
- Contacts
- Subscription
- Webhook
- Authentication
token_urls:
- https://api.infusionsoft.com/token
---
