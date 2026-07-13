---
api_specs:
- filename: ariba-guided-buying-catalog-shop-api.yaml
  format: yaml
  label: Ariba Guided Buying - Public Catalogs Shop API
  slug: ariba-guided-buying-catalog-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/openapi/ariba-guided-buying-catalog-shop-api.yaml
- filename: ariba-guided-buying-asset-management-api.yaml
  format: yaml
  label: Ariba Guided Buying - Asset Management API
  slug: ariba-guided-buying-asset-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/openapi/ariba-guided-buying-asset-management-api.yaml
authorization_urls: []
description: ''
docs: https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ariba Guided Buying Scopes
name_suffix: OAuth Scopes
note: SAP Ariba APIs use two-legged OAuth (client credentials / grant_type=openapi_2lo) with a per-application OAuth client ID plus Application Key, and access is granted per API through SAP Ariba approval rather than OAuth scopes; no scopes are documented (https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication).
overview: 'Ariba Guided Buying uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.ariba.com/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ariba Guided Buying
provider_slug: ariba-guided-buying
schemes:
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  source: openapi/ariba-guided-buying-asset-management-api.yaml
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials. Include the application key in the apikey header.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  source: openapi/ariba-guided-buying-catalog-shop-api.yaml
scope_count: 0
scope_names: []
scopes: []
slug: ariba-guided-buying-scopes
source_filename: ariba-guided-buying-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ariba-guided-buying-asset-management-api.yaml, openapi/ariba-guided-buying-catalog-shop-api.yaml\ndocs: https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication\nnote: SAP Ariba APIs use two-legged OAuth (client credentials / grant_type=openapi_2lo)\n  with a per-application OAuth client ID plus Application Key, and access is granted\n  per API through SAP Ariba approval rather than OAuth scopes; no scopes are documented\n  (https://help.sap.com/docs/ariba-apis/help-for-sap-ariba-developer-portal/sap-ariba-developer-portal-authentication).\nschemes:\n- name: OAuth2\n  source: openapi/ariba-guided-buying-asset-management-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\n- name:\
  \ OAuth2\n  source: openapi/ariba-guided-buying-catalog-shop-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials. Include the application key in the apikey header.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba-guided-buying/refs/heads/main/scopes/ariba-guided-buying-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- B2B
- Catalog
- ERP
- Procurement
- Requisitions
- SAP
- Supply Chain
token_urls:
- https://api.ariba.com/v2/oauth/token
---
