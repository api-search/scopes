---
api_specs:
- filename: sap-hana-alerts-api-openapi.yml
  format: yaml
  label: SAP HANA Alerts API
  slug: sap-hana-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-alerts-api-openapi.yml
- filename: sap-hana-instance-mappings-api-openapi.yml
  format: yaml
  label: SAP HANA Instance Mappings API
  slug: sap-hana-instance-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-instance-mappings-api-openapi.yml
- filename: sap-hana-instances-api-openapi.yml
  format: yaml
  label: SAP HANA Instances API
  slug: sap-hana-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-instances-api-openapi.yml
- filename: sap-hana-metering-api-openapi.yml
  format: yaml
  label: SAP HANA Metering API
  slug: sap-hana-metering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-metering-api-openapi.yml
- filename: sap-hana-metrics-api-openapi.yml
  format: yaml
  label: SAP HANA Metrics API
  slug: sap-hana-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-metrics-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Sap Hana Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'SAP HANA uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP HANA
provider_slug: sap-hana
schemes:
- description: OAuth 2.0 authentication using SAP Business Technology Platform credentials. Obtain an access token using client credentials flow with the UAA service URL, client ID, and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately 1799 seconds (30 minutes) and must be refreshed.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-hana-alerts-api-openapi.yml
- description: OAuth 2.0 authentication using SAP Business Technology Platform credentials. Obtain an access token using client credentials flow with the UAA service URL, client ID, and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately 1799 seconds (30 minutes) and must be refreshed.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-hana-instance-mappings-api-openapi.yml
- description: OAuth 2.0 authentication using SAP Business Technology Platform credentials. Obtain an access token using client credentials flow with the UAA service URL, client ID, and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately 1799 seconds (30 minutes) and must be refreshed.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-hana-instances-api-openapi.yml
- description: OAuth 2.0 authentication using SAP Business Technology Platform credentials. Obtain an access token using client credentials flow with the UAA service URL, client ID, and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately 1799 seconds (30 minutes) and must be refreshed.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-hana-metering-api-openapi.yml
- description: OAuth 2.0 authentication using SAP Business Technology Platform credentials. Obtain an access token using client credentials flow with the UAA service URL, client ID, and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately 1799 seconds (30 minutes) and must be refreshed.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-hana-metrics-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-hana-scopes
source_filename: sap-hana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/sap-hana-alerts-api-openapi.yml, openapi/sap-hana-instance-mappings-api-openapi.yml,\n  openapi/sap-hana-instances-api-openapi.yml, openapi/sap-hana-metering-api-openapi.yml, openapi/sap-hana-metrics-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/sap-hana-alerts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately\n    1799 seconds (30 minutes) and must be refreshed.\n- name: oauth2\n  source: openapi/sap-hana-instance-mappings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n\
  \  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately\n    1799 seconds (30 minutes) and must be refreshed.\n- name: oauth2\n  source: openapi/sap-hana-instances-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately\n    1799 seconds (30 minutes) and must be refreshed.\n- name: oauth2\n  source: openapi/sap-hana-metering-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately\n    1799 seconds (30 minutes) and must be refreshed.\n- name: oauth2\n  source: openapi/sap-hana-metrics-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire after approximately\n    1799 seconds (30 minutes) and must be refreshed.\nscopes: []\nnote: The OAuth2 security scheme(s)\
  \ in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/scopes/sap-hana-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
token_bound: false
token_urls:
- https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
---
