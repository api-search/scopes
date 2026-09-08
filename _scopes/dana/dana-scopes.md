---
api_specs:
- filename: dana-availability-api-openapi.yml
  format: yaml
  label: Dana Availability API
  slug: dana-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-availability-api-openapi.yml
- filename: dana-orders-api-openapi.yml
  format: yaml
  label: Dana Orders API
  slug: dana-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-orders-api-openapi.yml
- filename: dana-parts-api-openapi.yml
  format: yaml
  label: Dana Parts API
  slug: dana-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-parts-api-openapi.yml
- filename: dana-pricing-api-openapi.yml
  format: yaml
  label: Dana Pricing API
  slug: dana-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-pricing-api-openapi.yml
- filename: dana-shipping-api-openapi.yml
  format: yaml
  label: Dana Shipping API
  slug: dana-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/openapi/dana-shipping-api-openapi.yml
authorization_urls: []
description: Every scope below is read verbatim from the scopes_supported array of the OpenID Connect discovery document Dana serves at www.dana.com. The epi_* scopes are Optimizely (Episerver) CMS scopes — this is the content-delivery/forms surface of dana.com, not the Dana Aftermarket product API. Descriptions are the standard meanings of those scope names; nothing here is invented and no scope was added that the document does not list.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Dana Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dana uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dana
provider_slug: dana
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: dana-scopes
source_filename: dana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Dana Incorporated\nproviderId: dana-incorporated\ngenerated: '2026-09-07'\nmethod: probed\nsource: https://www.dana.com/.well-known/openid-configuration\ndescription: >-\n  Every scope below is read verbatim from the scopes_supported array of the OpenID Connect\n  discovery document Dana serves at www.dana.com. The epi_* scopes are Optimizely (Episerver)\n  CMS scopes — this is the content-delivery/forms surface of dana.com, not the Dana Aftermarket\n  product API. Descriptions are the standard meanings of those scope names; nothing here is\n  invented and no scope was added that the document does not list.\ndocs: null\ndocs_note: >-\n  Dana publishes no scope or permissions reference page. Searched dana.com (sitemap walked)\n  and danaaftermarket.com; neither carries developer documentation.\nscope_count: 8\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope requesting an\
  \ ID token for the authenticated subject.\n    standard: true\n  - name: offline_access\n    description: Requests a refresh token so the client can renew access without user interaction.\n    standard: true\n  - name: profile\n    description: Standard OIDC scope releasing basic profile claims.\n    standard: true\n  - name: email\n    description: Standard OIDC scope releasing the email claim.\n    standard: true\n  - name: roles\n    description: Releases the role claim for the authenticated subject.\n    standard: false\n  - name: epi_content_delivery\n    description: Optimizely (Episerver) Content Delivery API — read published CMS content.\n    standard: false\n  - name: epi_content_definitions\n    description: Optimizely (Episerver) Content Definitions API — read/manage content type definitions.\n    standard: false\n  - name: epi_forms_api\n    description: Optimizely (Episerver) Forms API — read form submissions.\n    standard: false\nmaintainers:\n  - FN: Kin Lane\n    email:\
  \ kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dana/refs/heads/main/scopes/dana-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Aftermarket
- Auto Parts
- Drivetrain
- E-Commerce
- Supply Chain
- Fortune 500
token_urls: []
---
