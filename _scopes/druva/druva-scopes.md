---
api_specs:
- filename: druva-authentication-openapi.json
  format: json
  label: Druva Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-authentication-openapi.json
- filename: druva-msp-authentication-openapi.json
  format: json
  label: Druva MSP Authentication API
  slug: msp-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-msp-authentication-openapi.json
- filename: druva-govcloud-authentication-openapi.json
  format: json
  label: Druva GovCloud Authentication API
  slug: govcloud-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-govcloud-authentication-openapi.json
- filename: druva-hybrid-workload-govcloud-authentication-openapi.json
  format: json
  label: Druva Hybrid Workloads GovCloud Authentication API
  slug: hybrid-workload-govcloud-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-hybrid-workload-govcloud-authentication-openapi.json
- filename: druva-insync-cloud-openapi.json
  format: json
  label: Druva Endpoints and Data Governance API
  slug: endpoints-data-governance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-insync-cloud-openapi.json
- filename: druva-insync-govcloud-openapi.json
  format: json
  label: Druva Endpoints and Data Governance GovCloud API
  slug: insync-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-insync-govcloud-openapi.json
- filename: druva-enterprise-workloads-openapi.json
  format: json
  label: Druva Enterprise Workloads API
  slug: enterprise-workloads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-enterprise-workloads-openapi.json
- filename: druva-enterprise-workloads-govcloud-openapi.json
  format: json
  label: Druva Enterprise Workloads GovCloud API
  slug: enterprise-workloads-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-enterprise-workloads-govcloud-openapi.json
- filename: druva-cyber-resilience-openapi.json
  format: json
  label: Druva Cyber Resilience API
  slug: cyber-resilience
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-openapi.json
- filename: druva-cyber-resilience-govcloud-openapi.json
  format: json
  label: Druva Cyber Resilience GovCloud API
  slug: cyber-resilience-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-govcloud-openapi.json
- filename: druva-cyber-resilience-govcloud-authorization-openapi.json
  format: json
  label: Druva GovCloud Cyber Resilience Authorization API
  slug: cyber-resilience-govcloud-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-govcloud-authorization-openapi.json
- filename: druva-cloudranger-openapi.json
  format: json
  label: Druva CloudRanger Native Workloads API
  slug: cloudranger
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cloudranger-openapi.json
- filename: druva-aws-native-openapi.json
  format: json
  label: Druva AWS Native Workloads API
  slug: aws-native
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-aws-native-openapi.json
- filename: druva-msp-openapi.json
  format: json
  label: Druva MSP API
  slug: msp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-msp-openapi.json
- filename: druva-platform-openapi.json
  format: json
  label: Druva Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-platform-openapi.json
- filename: druva-microsoft-365-openapi.json
  format: json
  label: Druva Microsoft 365 API
  slug: microsoft-365
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-microsoft-365-openapi.json
- filename: druva-google-workspace-openapi.json
  format: json
  label: Druva Google Workspace API
  slug: google-workspace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-google-workspace-openapi.json
- filename: druva-job-management-cloud-openapi.json
  format: json
  label: Druva Job Management API for Cloud Workloads
  slug: job-management-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-job-management-cloud-openapi.json
- filename: druva-job-management-govcloud-openapi.json
  format: json
  label: Druva Job Management API for GovCloud Workloads
  slug: job-management-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-job-management-govcloud-openapi.json
- filename: druva-insync-cloud-openapi.json
  format: json
  label: Druva Legal Hold Targeted Download API
  slug: legal-hold
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-insync-cloud-openapi.json
authorization_urls: []
description: ''
docs: https://developer.druva.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Druva Scopes
name_suffix: OAuth Scopes
note: 'Druva declares exactly ONE OAuth scope across its whole 970-operation estate: ''read'', on the client-credentials flow, in 11 of 19 specifications. The documentation is explicit that this is not an oversight but the design - ''The Client Credentials have access to all the OAuth Scopes by default'' - so scope is not the authorization boundary. The real boundary is the Druva console role attached to the API credential (Cloud Administrator, or the newer Cloud Admin Read Only role for the inSync Cloud and Platform APIs), which is not expressed in any contract. An agent therefore cannot request least privilege at the token endpoint; least privilege has to be provisioned by a human when the credential is minted. The separate MCP server at mcp.druva.com does scope properly - mcp:tools and mcp:resources - and is the only Druva surface where scope carries meaning.'
overview: 'Druva uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://apis.druva.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Druva
provider_slug: druva
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-aws-native-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://govapis.druva.com/token
  name: OAuth2
  source: openapi/druva-cyber-resilience-govcloud-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-cyber-resilience-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-enterprise-workloads-govcloud-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-enterprise-workloads-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-insync-cloud-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-insync-govcloud-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-job-management-cloud-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  source: openapi/druva-job-management-govcloud-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/msp/auth/v1/token
  name: OAuth2
  source: openapi/druva-msp-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://apis.druva.com/token
  name: BearerAuth
  source: openapi/druva-platform-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: druva-scopes
source_filename: druva-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: openapi/druva-aws-native-openapi.json, openapi/druva-cyber-resilience-govcloud-openapi.json, openapi/druva-cyber-resilience-openapi.json,\n  openapi/druva-enterprise-workloads-govcloud-openapi.json, openapi/druva-enterprise-workloads-openapi.json,\n  openapi/druva-insync-cloud-openapi.json, openapi/druva-insync-govcloud-openapi.json, openapi/druva-job-management-cloud-openapi.json,\n  openapi/druva-job-management-govcloud-openapi.json, openapi/druva-msp-openapi.json, openapi/druva-platform-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/druva-aws-native-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-cyber-resilience-govcloud-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://govapis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-cyber-resilience-openapi.json\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-enterprise-workloads-govcloud-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-enterprise-workloads-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-insync-cloud-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-insync-govcloud-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-job-management-cloud-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name: OAuth2\n  source: openapi/druva-job-management-govcloud-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n- name:\
  \ OAuth2\n  source: openapi/druva-msp-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/msp/auth/v1/token\n- name: BearerAuth\n  source: openapi/druva-platform-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\nscopes:\n- name: read\n  description: Grants read access. The only scope declared in any Druva specification.\n  source: securitySchemes.OAuth2.flows.clientCredentials.scopes in 11 of 19 specs\ndocs: https://developer.druva.com/docs/authentication\nnote: 'Druva declares exactly ONE OAuth scope across its whole 970-operation estate: ''read'', on the\n  client-credentials flow, in 11 of 19 specifications. The documentation is explicit that this is not\n  an oversight but the design - ''The Client Credentials have access to all the OAuth Scopes by default''\n  - so scope is not the authorization boundary. The real boundary is the Druva console role attached to\n  the API credential (Cloud Administrator,\
  \ or the newer Cloud Admin Read Only role for the inSync Cloud\n  and Platform APIs), which is not expressed in any contract. An agent therefore cannot request least\n  privilege at the token endpoint; least privilege has to be provisioned by a human when the credential\n  is minted. The separate MCP server at mcp.druva.com does scope properly - mcp:tools and mcp:resources\n  - and is the only Druva surface where scope carries meaning.'\nmcp_scopes:\n- name: mcp:tools\n  source: https://mcp.druva.com/.well-known/oauth-authorization-server\n- name: mcp:resources\n  source: https://mcp.druva.com/.well-known/oauth-authorization-server\nauthorization_model:\n  style: role-based, provisioned out of band\n  roles:\n  - Cloud Administrator\n  - Cloud Admin Read Only\n  docs: https://help.druva.com/en/articles/8580838-create-and-manage-api-credentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/scopes/druva-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Backup
- Cyber Resilience
- Data Protection
- Disaster Recovery
- SaaS Backup
- Ransomware Recovery
- Data Governance
- Enterprise Workloads
- MSP
- Legal Hold
- Endpoints
- GovCloud
- MCP
token_urls:
- https://apis.druva.com/token
- https://govapis.druva.com/token
- https://apis.druva.com/msp/auth/v1/token
---
