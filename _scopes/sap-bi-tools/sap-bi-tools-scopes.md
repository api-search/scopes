---
api_specs:
- filename: sap-bi-tools-administration-api-openapi.yml
  format: yaml
  label: SAP BI Tools Administration API
  slug: sap-bi-tools-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-administration-api-openapi.yml
- filename: sap-bi-tools-authentication-api-openapi.yml
  format: yaml
  label: SAP BI Tools Authentication API
  slug: sap-bi-tools-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-authentication-api-openapi.yml
- filename: sap-bi-tools-calendars-api-openapi.yml
  format: yaml
  label: SAP BI Tools Calendars API
  slug: sap-bi-tools-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-calendars-api-openapi.yml
- filename: sap-bi-tools-cms-query-api-openapi.yml
  format: yaml
  label: SAP BI Tools CMS Query API
  slug: sap-bi-tools-cms-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-cms-query-api-openapi.yml
- filename: sap-bi-tools-content-items-api-openapi.yml
  format: yaml
  label: SAP BI Tools Content Items API
  slug: sap-bi-tools-content-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-content-items-api-openapi.yml
- filename: sap-bi-tools-fact-data-api-openapi.yml
  format: yaml
  label: SAP BI Tools Fact Data API
  slug: sap-bi-tools-fact-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-fact-data-api-openapi.yml
- filename: sap-bi-tools-import-api-openapi.yml
  format: yaml
  label: SAP BI Tools Import API
  slug: sap-bi-tools-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-import-api-openapi.yml
- filename: sap-bi-tools-inbox-api-openapi.yml
  format: yaml
  label: SAP BI Tools Inbox API
  slug: sap-bi-tools-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-inbox-api-openapi.yml
- filename: sap-bi-tools-infostore-api-openapi.yml
  format: yaml
  label: SAP BI Tools InfoStore API
  slug: sap-bi-tools-infostore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-infostore-api-openapi.yml
- filename: sap-bi-tools-master-data-api-openapi.yml
  format: yaml
  label: SAP BI Tools Master Data API
  slug: sap-bi-tools-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-master-data-api-openapi.yml
- filename: sap-bi-tools-metadata-api-openapi.yml
  format: yaml
  label: SAP BI Tools Metadata API
  slug: sap-bi-tools-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-metadata-api-openapi.yml
- filename: sap-bi-tools-resources-api-openapi.yml
  format: yaml
  label: SAP BI Tools Resources API
  slug: sap-bi-tools-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-resources-api-openapi.yml
- filename: sap-bi-tools-scheduling-api-openapi.yml
  format: yaml
  label: SAP BI Tools Scheduling API
  slug: sap-bi-tools-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-scheduling-api-openapi.yml
- filename: sap-bi-tools-stories-api-openapi.yml
  format: yaml
  label: SAP BI Tools Stories API
  slug: sap-bi-tools-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-stories-api-openapi.yml
- filename: sap-bi-tools-teams-api-openapi.yml
  format: yaml
  label: SAP BI Tools Teams API
  slug: sap-bi-tools-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-teams-api-openapi.yml
- filename: sap-bi-tools-users-api-openapi.yml
  format: yaml
  label: SAP BI Tools Users API
  slug: sap-bi-tools-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-bi-tools-users-api-openapi.yml
authorization_urls:
- https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize
description: ''
docs: https://help.sap.com/docs/SAP_ANALYTICS_CLOUD/00f68c2e08b941f081002fd3691d86a7/4f43b54398fc4acaa5efa32badfe3df6.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sap Bi Tools Scopes
name_suffix: OAuth Scopes
note: SAP Analytics Cloud does not publish OAuth scope strings; access is governed by tenant-configured OAuth client purposes (Interactive Usage or API Access) and Access options such as Story Listing and User Provisioning, per the Manage OAuth Clients documentation (https://help.sap.com/docs/SAP_ANALYTICS_CLOUD/00f68c2e08b941f081002fd3691d86a7/4f43b54398fc4acaa5efa32badfe3df6.html).
overview: 'SAP BI Tools uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP BI Tools
provider_slug: sap-bi-tools
schemes:
- description: OAuth 2.0 authentication using SAML bearer assertion or authorization code grant flow.
  flows:
  - authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-analytics-cloud-api-openapi.yml
- description: OAuth 2.0 authentication using authorization code grant flow.
  flows:
  - authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-analytics-cloud-content-network-api-openapi.yml
- description: OAuth 2.0 authentication using SAML bearer assertion or authorization code grant flow.
  flows:
  - authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  source: openapi/sap-analytics-cloud-data-export-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: sap-bi-tools-scopes
source_filename: sap-bi-tools-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-analytics-cloud-api-openapi.yml, openapi/sap-analytics-cloud-content-network-api-openapi.yml,\n  openapi/sap-analytics-cloud-data-export-api-openapi.yml\ndocs: https://help.sap.com/docs/SAP_ANALYTICS_CLOUD/00f68c2e08b941f081002fd3691d86a7/4f43b54398fc4acaa5efa32badfe3df6.html\nnote: SAP Analytics Cloud does not publish OAuth scope strings; access is governed by\n  tenant-configured OAuth client purposes (Interactive Usage or API Access) and Access\n  options such as Story Listing and User Provisioning, per the Manage OAuth Clients\n  documentation (https://help.sap.com/docs/SAP_ANALYTICS_CLOUD/00f68c2e08b941f081002fd3691d86a7/4f43b54398fc4acaa5efa32badfe3df6.html).\nschemes:\n- name: oauth2\n  source: openapi/sap-analytics-cloud-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize\n    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token\n\
  \  description: OAuth 2.0 authentication using SAML bearer assertion or authorization code grant\n    flow.\n- name: oauth2\n  source: openapi/sap-analytics-cloud-content-network-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize\n    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using authorization code grant flow.\n- name: oauth2\n  source: openapi/sap-analytics-cloud-data-export-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize\n    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token\n  description: OAuth 2.0 authentication using SAML bearer assertion or authorization code grant\n    flow.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/scopes/sap-bi-tools-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
token_urls:
- https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
---
