---
api_specs:
- filename: sap-hana-cloud-rest-api.yml
  format: yaml
  label: SAP HANA Cloud REST API
  slug: sap-hana-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/openapi/sap-hana-cloud-rest-api.yml
authorization_urls: []
description: ''
docs: https://developers.sap.com/tutorials/hana-cloud-automation-rest..html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sap Hana Scopes
name_suffix: OAuth Scopes
note: SAP HANA Cloud REST APIs do not publish a named OAuth scope catalog; access tokens are obtained via the OAuth 2.0 client_credentials grant using SAP BTP service key credentials, with no scope parameter, and authorization is governed by BTP roles and service bindings (https://developers.sap.com/tutorials/hana-cloud-automation-rest..html).
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
  source: openapi/sap-hana-cloud-rest-api.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-hana-scopes
source_filename: sap-hana-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-hana-cloud-rest-api.yml\ndocs: https://developers.sap.com/tutorials/hana-cloud-automation-rest..html\nnote: SAP HANA Cloud REST APIs do not publish a named OAuth scope catalog; access\n  tokens are obtained via the OAuth 2.0 client_credentials grant using SAP BTP service\n  key credentials, with no scope parameter, and authorization is governed by BTP\n  roles and service bindings (https://developers.sap.com/tutorials/hana-cloud-automation-rest..html).\nschemes:\n- name: oauth2\n  source: openapi/sap-hana-cloud-rest-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using SAP Business Technology Platform credentials.\n    Obtain an access token using client credentials flow with the UAA service URL, client ID,\n    and client secret from your SAP HANA Cloud service key. Access tokens expire\
  \ after approximately\n    1799 seconds (30 minutes) and must be refreshed.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/scopes/sap-hana-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
token_urls:
- https://{subdomain}.authentication.{region}.hana.ondemand.com/oauth/token
---
