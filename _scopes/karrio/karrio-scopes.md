---
api_specs:
- filename: karrio-addresses-api-openapi.yml
  format: yaml
  label: Karrio Addresses API
  slug: karrio-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-addresses-api-openapi.yml
- filename: karrio-api-api-openapi.yml
  format: yaml
  label: Karrio API
  slug: karrio-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-api-api-openapi.yml
- filename: karrio-auth-api-openapi.yml
  format: yaml
  label: Karrio Auth API
  slug: karrio-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-auth-api-openapi.yml
- filename: karrio-batches-api-openapi.yml
  format: yaml
  label: Karrio Batches API
  slug: karrio-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-batches-api-openapi.yml
- filename: karrio-carriers-api-openapi.yml
  format: yaml
  label: Karrio Carriers API
  slug: karrio-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-carriers-api-openapi.yml
- filename: karrio-connections-api-openapi.yml
  format: yaml
  label: Karrio Connections API
  slug: karrio-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-connections-api-openapi.yml
- filename: karrio-documents-api-openapi.yml
  format: yaml
  label: Karrio Documents API
  slug: karrio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-documents-api-openapi.yml
- filename: karrio-manifests-api-openapi.yml
  format: yaml
  label: Karrio Manifests API
  slug: karrio-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-manifests-api-openapi.yml
- filename: karrio-orders-api-openapi.yml
  format: yaml
  label: Karrio Orders API
  slug: karrio-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-orders-api-openapi.yml
- filename: karrio-parcels-api-openapi.yml
  format: yaml
  label: Karrio Parcels API
  slug: karrio-parcels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-parcels-api-openapi.yml
- filename: karrio-pickups-api-openapi.yml
  format: yaml
  label: Karrio Pickups API
  slug: karrio-pickups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-pickups-api-openapi.yml
- filename: karrio-products-api-openapi.yml
  format: yaml
  label: Karrio Products API
  slug: karrio-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-products-api-openapi.yml
- filename: karrio-proxy-api-openapi.yml
  format: yaml
  label: Karrio Proxy API
  slug: karrio-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-proxy-api-openapi.yml
- filename: karrio-shipments-api-openapi.yml
  format: yaml
  label: Karrio Shipments API
  slug: karrio-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-shipments-api-openapi.yml
- filename: karrio-trackers-api-openapi.yml
  format: yaml
  label: Karrio Trackers API
  slug: karrio-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-trackers-api-openapi.yml
- filename: karrio-webhooks-api-openapi.yml
  format: yaml
  label: Karrio Webhooks API
  slug: karrio-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/openapi/karrio-webhooks-api-openapi.yml
authorization_urls:
- /oauth/authorize/
description: ''
docs: https://karrio.io/docs/api-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Karrio Scopes
name_suffix: OAuth Scopes
note: 'Karrio publishes no scopes or permissions reference page. The three scopes below are the complete set declared in the contract and the only ones documented anywhere. They are coarse: read and write are org-wide, with no per-resource scoping, so an OAuth application granted `write` can purchase labels, cancel shipments and create manifests. No incremental or step-up authorization is offered. No /.well-known/oauth-authorization-server is served (probed 2026-08-27, HTTP 404 on karrio.io), so the endpoints below are only discoverable from the OpenAPI itself, and they are relative paths against the caller''s own instance.'
overview: 'Karrio publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Karrio API on a user''s behalf.


  Tokens are issued from /oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Karrio
provider_slug: karrio
schemes:
- description: 'Authorization: Bearer xxxxxxxx'
  flows:
  - authorizationUrl: /oauth/authorize/
    flow: authorizationCode
    tokenUrl: /oauth/token/
  name: OAuth2
  source: openapi/karrio-api-openapi.yml
scope_count: 3
scope_names:
- openid
- read
- write
scopes:
- description: OpenID connect
  flows:
  - authorizationCode
  scope: openid
- description: Read access to Karrio data
  flows:
  - authorizationCode
  scope: read
- description: Write access to Karrio data
  flows:
  - authorizationCode
  scope: write
slug: karrio-scopes
source_filename: karrio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/karrio-api-openapi.yml securitySchemes.OAuth2, cross-read against the Authentication\n  section of https://karrio.io/docs/api-reference.\nschemes:\n- name: OAuth2\n  source: openapi/karrio-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize/\n    tokenUrl: /oauth/token/\n  description: 'Authorization: Bearer xxxxxxxx'\nscopes:\n- scope: openid\n  description: OpenID connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/karrio-api-openapi.yml\n- scope: read\n  description: Read access to Karrio data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/karrio-api-openapi.yml\n- scope: write\n  description: Write access to Karrio data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/karrio-api-openapi.yml\ndocs: https://karrio.io/docs/api-reference\nnote: 'Karrio publishes no scopes or permissions reference page. The three scopes below are the complete\n\
  \  set declared in the contract and the only ones documented anywhere. They are coarse: read and write\n  are org-wide, with no per-resource scoping, so an OAuth application granted `write` can purchase\n  labels, cancel shipments and create manifests. No incremental or step-up authorization is offered.\n  No /.well-known/oauth-authorization-server is served (probed 2026-08-27, HTTP 404 on karrio.io),\n  so the endpoints below are only discoverable from the OpenAPI itself, and they are relative paths\n  against the caller''s own instance.'\ngranularity: coarse\nper_resource_scopes: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karrio/refs/heads/main/scopes/karrio-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Shipping
- Logistics
- Label Generation
- Package Tracking
- Carriers
- Fulfillment
- Open-Source
- Multi-Carrier
- Rating
- Webhook
token_urls:
- /oauth/token/
---
