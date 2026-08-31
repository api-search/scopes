---
api_specs:
- filename: landgate-datasets-api-openapi.yml
  format: yaml
  label: Landgate Datasets API
  slug: landgate-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-datasets-api-openapi.yml
- filename: landgate-discovery-api-openapi.yml
  format: yaml
  label: Landgate Discovery API
  slug: landgate-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-discovery-api-openapi.yml
- filename: landgate-organizations-api-openapi.yml
  format: yaml
  label: Landgate Organizations API
  slug: landgate-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-organizations-api-openapi.yml
- filename: landgate-query-api-openapi.yml
  format: yaml
  label: Landgate Query API
  slug: landgate-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-query-api-openapi.yml
- filename: landgate-server-api-openapi.yml
  format: yaml
  label: Landgate Server API
  slug: landgate-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-server-api-openapi.yml
- filename: landgate-services-api-openapi.yml
  format: yaml
  label: Landgate Services API
  slug: landgate-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-services-api-openapi.yml
- filename: landgate-site-api-openapi.yml
  format: yaml
  label: Landgate Site API
  slug: landgate-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-site-api-openapi.yml
- filename: landgate-wfs-api-openapi.yml
  format: yaml
  label: Landgate WFS API
  slug: landgate-wfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-wfs-api-openapi.yml
- filename: landgate-wms-api-openapi.yml
  format: yaml
  label: Landgate WMS API
  slug: landgate-wms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-wms-api-openapi.yml
authorization_urls:
- https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Landgate Scopes
name_suffix: OAuth Scopes
note: Landgate publishes no scopes/permissions reference page. This scope catalogue is taken verbatim from the `scopes_supported` array of the MyLandgate PingFederate discovery documents (both the OIDC discovery doc and the RFC 8414 authorization-server metadata advertise the same six values, fetched HTTP 200 anonymously on 2026-07-26). The public SLIP and Data WA CKAN surfaces carry NO OAuth scopes — they are anonymous. These scopes govern MyLandgate / Land Enquiry Services sign-on only.
overview: 'Landgate publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Landgate API on a user''s behalf.


  Tokens are issued from https://sign-on.app.landgate.wa.gov.au/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Landgate
provider_slug: landgate
schemes:
- flows:
  - authorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2
  issuer: https://sign-on.app.landgate.wa.gov.au
  name: MyLandgateOAuth2
  source: well-known/landgate-oauth-authorization-server.json
scope_count: 6
scope_names:
- openid
- profile
- email
- address
- phone
- ATO
scopes:
- description: Standard OpenID Connect scope — requests an ID token for the signed-in MyLandgate user.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Standard OIDC claim set — name and profile claims for the MyLandgate user.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Standard OIDC email claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Standard OIDC address claim.
  flows:
  - authorizationCode
  - implicit
  scope: address
- description: Standard OIDC phone-number claim.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Non-standard Landgate-specific scope advertised by the authorization server. No published definition was found; not documented on any Landgate page located on 2026-07-26. Recorded verbatim without interpretation.
  flows:
  - authorizationCode
  scope: ATO
slug: landgate-scopes
source_filename: landgate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://sign-on.app.landgate.wa.gov.au/.well-known/openid-configuration\ndocs: null\nnote: |\n  Landgate publishes no scopes/permissions reference page. This scope catalogue is taken\n  verbatim from the `scopes_supported` array of the MyLandgate PingFederate discovery\n  documents (both the OIDC discovery doc and the RFC 8414 authorization-server metadata\n  advertise the same six values, fetched HTTP 200 anonymously on 2026-07-26).\n\n  The public SLIP and Data WA CKAN surfaces carry NO OAuth scopes — they are anonymous.\n  These scopes govern MyLandgate / Land Enquiry Services sign-on only.\nschemes:\n  - name: MyLandgateOAuth2\n    source: well-known/landgate-oauth-authorization-server.json\n    issuer: https://sign-on.app.landgate.wa.gov.au\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2\n        tokenUrl: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2\n\
  scopes:\n  - scope: openid\n    description: Standard OpenID Connect scope — requests an ID token for the signed-in\n      MyLandgate user.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/landgate-openid-configuration.json]\n  - scope: profile\n    description: Standard OIDC claim set — name and profile claims for the MyLandgate user.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/landgate-openid-configuration.json]\n  - scope: email\n    description: Standard OIDC email claim.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/landgate-openid-configuration.json]\n  - scope: address\n    description: Standard OIDC address claim.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/landgate-openid-configuration.json]\n  - scope: phone\n    description: Standard OIDC phone-number claim.\n    flows: [authorizationCode, implicit]\n    sources: [well-known/landgate-openid-configuration.json]\n  - scope: ATO\n    description:\
  \ Non-standard Landgate-specific scope advertised by the authorization server.\n      No published definition was found; not documented on any Landgate page located on\n      2026-07-26. Recorded verbatim without interpretation.\n    flows: [authorizationCode]\n    sources: [well-known/landgate-oauth-authorization-server.json]\nsummary:\n  scope_count: 6\n  standard_oidc: 5\n  provider_specific: 1\n  documented_by_provider: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/scopes/landgate-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Real-Estate
- Australia
- Land Registry
- Title
- Valuation
- Property Data
- Open Data
- Geospatial
- Government
- Conveyancing
- PropTech
token_urls:
- https://sign-on.app.landgate.wa.gov.au/as/token.oauth2
---
