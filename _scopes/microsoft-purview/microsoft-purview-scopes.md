---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Purview Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Purview publishes 8 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Purview API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schemes:
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-account-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-catalog-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-data-map-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-data-quality-openapi.yml
- description: Microsoft Identity Platform OAuth2
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-data-security-governance-openapi.yml
- description: Microsoft Identity Platform OAuth2
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-ediscovery-openapi.yml
- description: Microsoft Identity Platform OAuth2
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-information-protection-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-metadata-policies-openapi.yml
- description: Microsoft Identity Platform OAuth2
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-records-management-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-scanning-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-unified-catalog-openapi.yml
- description: Azure Active Directory OAuth2 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/microsoft-purview-workflow-openapi.yml
scope_count: 8
scope_names:
- InformationProtectionPolicy.Read
- InformationProtectionPolicy.Read.All
- RecordsManagement.Read.All
- RecordsManagement.ReadWrite.All
- eDiscovery.Read.All
- eDiscovery.ReadWrite.All
- https://management.azure.com/.default
- https://purview.azure.net/.default
scopes:
- description: Read information protection policies
  flows:
  - authorizationCode
  scope: InformationProtectionPolicy.Read
- description: Read all information protection policies
  flows:
  - authorizationCode
  - clientCredentials
  scope: InformationProtectionPolicy.Read.All
- description: Read records management settings
  flows:
  - clientCredentials
  scope: RecordsManagement.Read.All
- description: Read and write records management settings
  flows:
  - clientCredentials
  scope: RecordsManagement.ReadWrite.All
- description: Read eDiscovery data
  flows:
  - authorizationCode
  scope: eDiscovery.Read.All
- description: Read and write eDiscovery data
  flows:
  - authorizationCode
  scope: eDiscovery.ReadWrite.All
- description: Access Azure Resource Manager
  flows:
  - clientCredentials
  scope: https://management.azure.com/.default
- description: Access Microsoft Purview
  flows:
  - clientCredentials
  scope: https://purview.azure.net/.default
slug: microsoft-purview-scopes
source_filename: microsoft-purview-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-purview-account-openapi.yml, openapi/microsoft-purview-catalog-openapi.yml,\n  openapi/microsoft-purview-data-map-openapi.yml, openapi/microsoft-purview-data-quality-openapi.yml,\n  openapi/microsoft-purview-data-security-governance-openapi.yml, openapi/microsoft-purview-ediscovery-openapi.yml,\n  openapi/microsoft-purview-information-protection-openapi.yml, openapi/microsoft-purview-metadata-policies-openapi.yml,\n  openapi/microsoft-purview-records-management-openapi.yml, openapi/microsoft-purview-scanning-openapi.yml,\n  openapi/microsoft-purview-unified-catalog-openapi.yml, openapi/microsoft-purview-workflow-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/microsoft-purview-account-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source:\
  \ openapi/microsoft-purview-catalog-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source: openapi/microsoft-purview-data-map-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source: openapi/microsoft-purview-data-quality-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source: openapi/microsoft-purview-data-security-governance-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Identity Platform OAuth2\n- name:\
  \ oauth2\n  source: openapi/microsoft-purview-ediscovery-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Identity Platform OAuth2\n- name: oauth2\n  source: openapi/microsoft-purview-information-protection-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: Microsoft Identity Platform OAuth2\n- name: oauth2\n  source: openapi/microsoft-purview-metadata-policies-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source: openapi/microsoft-purview-records-management-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Identity Platform OAuth2\n- name: oauth2\n  source: openapi/microsoft-purview-scanning-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source: openapi/microsoft-purview-unified-catalog-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\n- name: oauth2\n  source: openapi/microsoft-purview-workflow-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Azure Active Directory OAuth2 authentication\nscopes:\n- scope: InformationProtectionPolicy.Read\n  description: Read\
  \ information protection policies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-purview-information-protection-openapi.yml\n- scope: InformationProtectionPolicy.Read.All\n  description: Read all information protection policies\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/microsoft-purview-data-security-governance-openapi.yml\n  - openapi/microsoft-purview-information-protection-openapi.yml\n- scope: RecordsManagement.Read.All\n  description: Read records management settings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-purview-records-management-openapi.yml\n- scope: RecordsManagement.ReadWrite.All\n  description: Read and write records management settings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-purview-records-management-openapi.yml\n- scope: eDiscovery.Read.All\n  description: Read eDiscovery data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-purview-ediscovery-openapi.yml\n\
  - scope: eDiscovery.ReadWrite.All\n  description: Read and write eDiscovery data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/microsoft-purview-ediscovery-openapi.yml\n- scope: https://management.azure.com/.default\n  description: Access Azure Resource Manager\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-purview-account-openapi.yml\n- scope: https://purview.azure.net/.default\n  description: Access Microsoft Purview\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/microsoft-purview-catalog-openapi.yml\n  - openapi/microsoft-purview-data-map-openapi.yml\n  - openapi/microsoft-purview-data-quality-openapi.yml\n  - openapi/microsoft-purview-metadata-policies-openapi.yml\n  - openapi/microsoft-purview-scanning-openapi.yml\n  - openapi/microsoft-purview-unified-catalog-openapi.yml\n  - openapi/microsoft-purview-workflow-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/scopes/microsoft-purview-scopes.yml
summary_line: 8 scopes · clientCredentials/authorizationCode
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
