---
api_specs:
- filename: microsoft-azure-data-lake-accounts-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Accounts API
  slug: microsoft-azure-data-lake-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-accounts-api-openapi.yml
- filename: microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Azure Data Lake Storage REST API
  slug: microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml
- filename: microsoft-azure-data-lake-locations-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Locations API
  slug: microsoft-azure-data-lake-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-locations-api-openapi.yml
- filename: microsoft-azure-data-lake-locationusage-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Location Usage API
  slug: microsoft-azure-data-lake-locationusage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-locationusage-api-openapi.yml
- filename: microsoft-azure-data-lake-operations-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Operations API
  slug: microsoft-azure-data-lake-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-operations-api-openapi.yml
- filename: microsoft-azure-data-lake-trustedidproviders-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Trusted ID Providers API
  slug: microsoft-azure-data-lake-trustedidproviders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-trustedidproviders-api-openapi.yml
- filename: microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Virtual Network Rules API
  slug: microsoft-azure-data-lake-virtualnetworkrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml
- filename: microsoft-azure-data-lake-firewall-rules-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Firewall Rules API
  slug: microsoft-azure-data-lake-firewall-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-firewall-rules-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Data Lake Storage Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Data Lake Storage publishes 2 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Data Lake Storage API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Data Lake Storage
provider_slug: microsoft-azure-data-lake
schemes:
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-accounts-api-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-firewall-rules-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-locations-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-locationusage-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-operations-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-trustedidproviders-api-openapi.yml
- description: Azure Active Directory OAuth2 Flow
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml
scope_count: 2
scope_names:
- https://storage.azure.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - implicit
  scope: https://storage.azure.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-azure-data-lake-scopes
source_filename: microsoft-azure-data-lake-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/microsoft-azure-data-lake-accounts-api-openapi.yml, openapi/microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml,\n  openapi/microsoft-azure-data-lake-firewall-rules-api-openapi.yml, openapi/microsoft-azure-data-lake-locations-api-openapi.yml,\n  openapi/microsoft-azure-data-lake-locationusage-api-openapi.yml, openapi/microsoft-azure-data-lake-operations-api-openapi.yml,\n  openapi/microsoft-azure-data-lake-trustedidproviders-api-openapi.yml, openapi/microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml\nschemes:\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-accounts-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: OAuth2Auth\n  source: openapi/microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml\n  flows:\n  -\
  \ flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-firewall-rules-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-locations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-locationusage-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-operations-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl:\
  \ https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-trustedidproviders-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\n- name: azure_auth\n  source: openapi/microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow\nscopes:\n- scope: https://storage.azure.com/.default\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-azure-data-lake-accounts-api-openapi.yml\n  - openapi/microsoft-azure-data-lake-firewall-rules-api-openapi.yml\n\
  \  - openapi/microsoft-azure-data-lake-locations-api-openapi.yml\n  - openapi/microsoft-azure-data-lake-locationusage-api-openapi.yml\n  - openapi/microsoft-azure-data-lake-operations-api-openapi.yml\n  - openapi/microsoft-azure-data-lake-trustedidproviders-api-openapi.yml\n  - openapi/microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-data-lake/scopes/microsoft-azure-data-lake-scopes.yml
summary_line: 2 scopes · implicit
tags:
- Analytics
- Big Data
- Data Lake
- Hierarchical Storage
token_bound: false
token_urls: []
---
