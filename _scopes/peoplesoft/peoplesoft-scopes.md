---
api_specs:
- filename: rest-api.yml
  format: yaml
  label: PeopleSoft REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/rest-api.yml
- filename: application-services-framework.yml
  format: yaml
  label: PeopleSoft Application Services Framework API
  slug: application-services-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/application-services-framework.yml
- filename: integration-broker.yml
  format: yaml
  label: PeopleSoft Integration Broker
  slug: integration-broker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/integration-broker.yml
- filename: query.yml
  format: yaml
  label: PeopleSoft Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/query.yml
- filename: component-interface.yml
  format: yaml
  label: PeopleSoft Component Interface API
  slug: component-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/component-interface.yml
- filename: search-framework.yml
  format: yaml
  label: PeopleSoft Search Framework API
  slug: search-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/search-framework.yml
- filename: notification-framework.yml
  format: yaml
  label: PeopleSoft Notification Framework API
  slug: notification-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/notification-framework.yml
- filename: chatbot-integration.yml
  format: yaml
  label: PeopleSoft Chatbot Integration Framework API
  slug: chatbot-integration-framework-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/chatbot-integration.yml
- filename: approval-workflow-engine.yml
  format: yaml
  label: PeopleSoft Approval Workflow Engine API
  slug: approval-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/approval-workflow-engine.yml
- filename: process-scheduler.yml
  format: yaml
  label: PeopleSoft Process Scheduler API
  slug: process-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/process-scheduler.yml
- filename: cloud-manager.yml
  format: yaml
  label: PeopleSoft Cloud Manager API
  slug: cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/cloud-manager.yml
- filename: update-manager.yml
  format: yaml
  label: PeopleSoft Update Manager API
  slug: update-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/update-manager.yml
- filename: pivot-grid.yml
  format: yaml
  label: PeopleSoft Pivot Grid API
  slug: pivot-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/pivot-grid.yml
- filename: hcm.yml
  format: yaml
  label: PeopleSoft HCM API
  slug: hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/hcm.yml
- filename: recruiting-talent-management.yml
  format: yaml
  label: PeopleSoft Recruiting and Talent Management API
  slug: recruiting-and-talent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/recruiting-talent-management.yml
- filename: financials.yml
  format: yaml
  label: PeopleSoft Financials API
  slug: financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/financials.yml
- filename: supply-chain-management.yml
  format: yaml
  label: PeopleSoft Supply Chain Management API
  slug: supply-chain-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/supply-chain-management.yml
- filename: crm.yml
  format: yaml
  label: PeopleSoft CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/crm.yml
- filename: campus-solutions.yml
  format: yaml
  label: PeopleSoft Campus Solutions API
  slug: campus-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/campus-solutions.yml
- filename: enterprise-performance-management.yml
  format: yaml
  label: PeopleSoft Enterprise Performance Management API
  slug: enterprise-performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/enterprise-performance-management.yml
- filename: interaction-hub.yml
  format: yaml
  label: PeopleSoft Interaction Hub API
  slug: interaction-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/openapi/interaction-hub.yml
authorization_urls:
- https://{hostname}:{port}/psft/oauth/authorize
description: ''
docs: https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Peoplesoft Scopes
name_suffix: OAuth Scopes
note: PeopleSoft OAuth 2.0 (PeopleTools 8.58+) publishes no scope catalog; authorization is enforced by PeopleSoft permission lists and roles tied to the user ID in the token's sub claim, with any scopes defined per deployment in the external identity provider (see https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html).
overview: 'PeopleSoft uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{hostname}:{port}/psft/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PeopleSoft
provider_slug: peoplesoft
schemes:
- flows:
  - authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{hostname}:{port}/psft/oauth/token
  name: oauth2
  source: openapi/application-services-framework.yml
- flows:
  - authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{hostname}:{port}/psft/oauth/token
  name: oauth2
  source: openapi/rest-api.yml
scope_count: 0
scope_names: []
scopes: []
slug: peoplesoft-scopes
source_filename: peoplesoft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/application-services-framework.yml, openapi/rest-api.yml\ndocs: https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html\nnote: PeopleSoft OAuth 2.0 (PeopleTools 8.58+) publishes no scope catalog; authorization\n  is enforced by PeopleSoft permission lists and roles tied to the user ID in the\n  token's sub claim, with any scopes defined per deployment in the external identity\n  provider (see https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html).\nschemes:\n- name: oauth2\n  source: openapi/application-services-framework.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize\n    tokenUrl: https://{hostname}:{port}/psft/oauth/token\n- name: oauth2\n  source: openapi/rest-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize\n\
  \    tokenUrl: https://{hostname}:{port}/psft/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/scopes/peoplesoft-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
token_urls:
- https://{hostname}:{port}/psft/oauth/token
---
