---
api_specs:
- filename: umbra-client-credentials-api-openapi.yml
  format: yaml
  label: Umbra Client Credentials API
  slug: umbra-client-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-client-credentials-api-openapi.yml
- filename: umbra-collections-api-openapi.yml
  format: yaml
  label: Umbra Collections API
  slug: umbra-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collections-api-openapi.yml
- filename: umbra-collectmetadata-api-openapi.yml
  format: yaml
  label: Umbra Collect Metadata API
  slug: umbra-collectmetadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collectmetadata-api-openapi.yml
- filename: umbra-collects-api-openapi.yml
  format: yaml
  label: Umbra Collects API
  slug: umbra-collects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collects-api-openapi.yml
- filename: umbra-deliveryconfig-api-openapi.yml
  format: yaml
  label: Umbra Delivery Config API
  slug: umbra-deliveryconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-deliveryconfig-api-openapi.yml
- filename: umbra-feasibility-api-openapi.yml
  format: yaml
  label: Umbra Feasibility API
  slug: umbra-feasibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-feasibility-api-openapi.yml
- filename: umbra-organizations-api-openapi.yml
  format: yaml
  label: Umbra Organizations API
  slug: umbra-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-organizations-api-openapi.yml
- filename: umbra-preview-api-openapi.yml
  format: yaml
  label: Umbra Preview API
  slug: umbra-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-preview-api-openapi.yml
- filename: umbra-preview-image-api-openapi.yml
  format: yaml
  label: Umbra Preview Image API
  slug: umbra-preview-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-preview-image-api-openapi.yml
- filename: umbra-product-constraints-api-openapi.yml
  format: yaml
  label: Umbra Product Constraints API
  slug: umbra-product-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-product-constraints-api-openapi.yml
- filename: umbra-restricted-access-areas-api-openapi.yml
  format: yaml
  label: Umbra Restricted Access Areas API
  slug: umbra-restricted-access-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-restricted-access-areas-api-openapi.yml
- filename: umbra-search-api-openapi.yml
  format: yaml
  label: Umbra Search API
  slug: umbra-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-search-api-openapi.yml
- filename: umbra-tasks-api-openapi.yml
  format: yaml
  label: Umbra Tasks API
  slug: umbra-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-tasks-api-openapi.yml
- filename: umbra-thumbnail-api-openapi.yml
  format: yaml
  label: Umbra Thumbnail API
  slug: umbra-thumbnail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-thumbnail-api-openapi.yml
authorization_urls:
- https://auth.canopy.umbra.space/authorize
description: ''
docs: https://docs.canopy.umbra.space/docs/authentication-via-client-credentials
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Umbra Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Umbra uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.canopy.umbra.space/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Umbra
provider_slug: umbra
schemes:
- flows:
  - audience_required: true
    flow: clientCredentials
    scopes_declared: none
    tokenUrl: https://auth.canopy.umbra.space/oauth/token
  - authorizationUrl: https://auth.canopy.umbra.space/authorize
    flow: authorizationCode
    note: used by the Canopy web application for interactive login
    tokenUrl: https://auth.canopy.umbra.space/oauth/token
  issuer: https://auth.canopy.umbra.space/
  name: Canopy OAuth2 (Auth0 tenant)
  source: well-known/umbra-oauth-authorization-server.json
scope_count: 0
scope_names: []
scopes: []
slug: umbra-scopes
source_filename: umbra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: well-known/umbra-oauth-authorization-server.json + well-known/umbra-openid-configuration.json\ndocs: https://docs.canopy.umbra.space/docs/authentication-via-client-credentials\nfinding: >-\n  Canopy runs a real OAuth2 client-credentials flow, but it publishes NO API-specific scope\n  vocabulary. Not one of the six OpenAPI documents declares an oauth2 securityScheme or any\n  scope on any operation — every operation is protected by the flat `bearerAuth` bearer token.\n  Authorization is resolved from the organization the credential belongs to and that\n  organization's contract and product constraints, not from scopes on the token. The scopes\n  listed below are the standard OIDC claim scopes advertised by the Auth0 tenant's discovery\n  documents; they govern the identity token, not access to Canopy tasking, archive, delivery or\n  admin resources. Recorded so the distinction is explicit rather than absent.\nschemes:\n- name:\
  \ Canopy OAuth2 (Auth0 tenant)\n  source: well-known/umbra-oauth-authorization-server.json\n  issuer: https://auth.canopy.umbra.space/\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.canopy.umbra.space/oauth/token\n    audience_required: true\n    scopes_declared: none\n  - flow: authorizationCode\n    authorizationUrl: https://auth.canopy.umbra.space/authorize\n    tokenUrl: https://auth.canopy.umbra.space/oauth/token\n    note: used by the Canopy web application for interactive login\nidp_scopes_supported:\n- scope: openid\n  description: OpenID Connect — request an ID token\n- scope: profile\n  description: Standard OIDC profile claims\n- scope: offline_access\n  description: Request a refresh token\n- scope: name\n- scope: given_name\n- scope: family_name\n- scope: nickname\n- scope: email\n- scope: email_verified\n- scope: picture\n- scope: created_at\n- scope: identities\n- scope: phone\n- scope: address\napi_scopes: []\nauthorization_axes:\n- axis: audience\n\
  \  values:\n  - https://api.canopy.umbra.space\n  - https://api.canopy.prod.umbra-sandbox.space\n  note: >-\n    The `audience` parameter on the token request is what selects the live or sandbox environment.\n    This is the closest thing Canopy has to a scope — it partitions access, and the two\n    environments are entirely isolated from each other.\n- axis: organization\n  note: >-\n    Client credentials are issued per organization; every request resolves to that organization's\n    Tasks, Collects, DeliveryConfigs and STAC collections.\n- axis: product constraints\n  note: >-\n    What an organization may actually task is bounded by contract-level product constraints,\n    readable via get_constraints_for_contract_or_org_default and\n    list_all_product_constraints_for_logged_in_org on the Admin API.\n- axis: restricted access areas\n  note: >-\n    A per-organization geofence of locations where tasking is disallowed, readable as a GeoJSON\n    FeatureCollection via get_restricted_access_areas.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/scopes/umbra-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Satellite Imagery
- Synthetic Aperture Radar
- Earth Observation
- Geospatial
- Space
- STAC
- Remote Sensing
- Tasking
- Defense and Intelligence
- Company
token_urls:
- https://auth.canopy.umbra.space/oauth/token
---
