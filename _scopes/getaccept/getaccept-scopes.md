---
api_specs:
- filename: getaccept-archive-api-openapi.yml
  format: yaml
  label: GetAccept Archive API
  slug: getaccept-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-archive-api-openapi.yml
- filename: getaccept-attachments-api-openapi.yml
  format: yaml
  label: GetAccept Attachments API
  slug: getaccept-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-attachments-api-openapi.yml
- filename: getaccept-authentication-api-openapi.yml
  format: yaml
  label: GetAccept Authentication API
  slug: getaccept-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-authentication-api-openapi.yml
- filename: getaccept-communication-templates-api-openapi.yml
  format: yaml
  label: GetAccept Communication Templates API
  slug: getaccept-communication-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-communication-templates-api-openapi.yml
- filename: getaccept-contacts-api-openapi.yml
  format: yaml
  label: GetAccept Contacts API
  slug: getaccept-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-contacts-api-openapi.yml
- filename: getaccept-custom-data-api-openapi.yml
  format: yaml
  label: GetAccept Custom Data API
  slug: getaccept-custom-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-custom-data-api-openapi.yml
- filename: getaccept-documents-api-openapi.yml
  format: yaml
  label: GetAccept Documents API
  slug: getaccept-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-documents-api-openapi.yml
- filename: getaccept-others-api-openapi.yml
  format: yaml
  label: GetAccept Others API
  slug: getaccept-others-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-others-api-openapi.yml
- filename: getaccept-subscriptions-api-openapi.yml
  format: yaml
  label: GetAccept Subscriptions API
  slug: getaccept-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-subscriptions-api-openapi.yml
- filename: getaccept-templates-api-openapi.yml
  format: yaml
  label: GetAccept Templates API
  slug: getaccept-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-templates-api-openapi.yml
- filename: getaccept-users-api-openapi.yml
  format: yaml
  label: GetAccept Users API
  slug: getaccept-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-users-api-openapi.yml
- filename: getaccept-videos-api-openapi.yml
  format: yaml
  label: GetAccept Videos API
  slug: getaccept-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/openapi/getaccept-videos-api-openapi.yml
authorization_urls:
- https://app.getaccept.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Getaccept Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'GetAccept publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the GetAccept API on a user''s behalf.


  Tokens are issued from https://app.getaccept.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GetAccept
provider_slug: getaccept
schemes:
- description: For testing purpose, use client_id **api** and client_secret **app**
  flows:
  - authorizationUrl: https://app.getaccept.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.getaccept.com/oauth2/token
  name: Oauth2
  source: openapi/getaccept-openapi-original.json
scope_count: 1
scope_names:
- basic
scopes:
- description: Grants basic access to operations
  flows:
  - authorizationCode
  scope: basic
slug: getaccept-scopes
source_filename: getaccept-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/getaccept-openapi-original.json\nschemes:\n- name: Oauth2\n  source: openapi/getaccept-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getaccept.com/oauth2/authorize\n    tokenUrl: https://app.getaccept.com/oauth2/token\n  description: For testing purpose, use client_id **api** and client_secret **app**\nscopes:\n- scope: basic\n  description: Grants basic access to operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/getaccept-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getaccept/refs/heads/main/scopes/getaccept-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Cloud
- Sales Enablement
- Electronic Signature
- E-Signature
- Digital Sales Room
- Document-Management
- Contract Management
- Proposals
- Software-as-a-Service
token_urls:
- https://app.getaccept.com/oauth2/token
---
