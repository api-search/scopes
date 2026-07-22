---
api_specs:
- filename: spaceship-openapi-original.json
  format: json
  label: Spaceship API
  slug: spaceship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/openapi/spaceship-openapi-original.json
authorization_urls: []
description: ''
docs: https://www.spaceship.com/application/api-manager/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Spaceship Scopes
name_suffix: OAuth Scopes
note: Spaceship does not use OAuth2. Scopes (permissions) are attached to an API key/secret pair at creation time in the API Manager. The scopes below are the documented permission set.
overview: 'Spaceship publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spaceship API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spaceship
provider_slug: spaceship
schemes:
- headers:
  - X-API-Key
  - X-API-Secret
  name: apiKey+apiSecret
  source: openapi/spaceship-openapi-original.json
  type: apiKey
scope_count: 11
scope_names:
- domains:read
- domains:write
- domains:transfer
- domains:billing
- contacts:read
- contacts:write
- dnsrecords:read
- dnsrecords:write
- asyncoperations:read
- sellerhub:read
- sellerhub:write
scopes:
- description: Read domain information and check configuration.
  flows: []
  scope: domains:read
- description: Manage domains and domain settings.
  flows: []
  scope: domains:write
- description: Transfer domains in and out.
  flows: []
  scope: domains:transfer
- description: Manage domains billing operations.
  flows: []
  scope: domains:billing
- description: Read contact details.
  flows: []
  scope: contacts:read
- description: Save contact details.
  flows: []
  scope: contacts:write
- description: Read DNS resource records.
  flows: []
  scope: dnsrecords:read
- description: Write DNS resource records.
  flows: []
  scope: dnsrecords:write
- description: Read async operations details.
  flows: []
  scope: asyncoperations:read
- description: Read SellerHub domains.
  flows: []
  scope: sellerhub:read
- description: Write SellerHub domains.
  flows: []
  scope: sellerhub:write
slug: spaceship-scopes
source_filename: spaceship-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.spaceship.dev/ (Permissions section of the API description)\ndocs: https://www.spaceship.com/application/api-manager/\nmodel: api-key-scopes\nnote: Spaceship does not use OAuth2. Scopes (permissions) are attached to an API key/secret pair at creation\n  time in the API Manager. The scopes below are the documented permission set.\nschemes:\n- name: apiKey+apiSecret\n  type: apiKey\n  headers:\n  - X-API-Key\n  - X-API-Secret\n  source: openapi/spaceship-openapi-original.json\nscopes:\n- scope: domains:read\n  description: Read domain information and check configuration.\n- scope: domains:write\n  description: Manage domains and domain settings.\n- scope: domains:transfer\n  description: Transfer domains in and out.\n- scope: domains:billing\n  description: Manage domains billing operations.\n- scope: contacts:read\n  description: Read contact details.\n- scope: contacts:write\n  description: Save contact details.\n\
  - scope: dnsrecords:read\n  description: Read DNS resource records.\n- scope: dnsrecords:write\n  description: Write DNS resource records.\n- scope: asyncoperations:read\n  description: Read async operations details.\n- scope: sellerhub:read\n  description: Read SellerHub domains.\n- scope: sellerhub:write\n  description: Write SellerHub domains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spaceship/refs/heads/main/scopes/spaceship-scopes.yml
summary_line: 11 scopes
tags:
- Company
- Domains
- Domain Registrar
- DNS
- Domain Marketplace
- Nameservers
- WHOIS
- Developer Tools
- API
token_urls: []
---
