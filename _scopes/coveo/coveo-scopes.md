---
authorization_urls:
- https://platform.cloud.coveo.com/oauth/authorize
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Coveo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Coveo publishes 1 OAuth 2.0 scope via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coveo API on a user''s behalf.


  Tokens are issued from https://platform.cloud.coveo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coveo
provider_slug: coveo
schemes:
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-activity-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-analytics-admin-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-authorization-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-catalog-management-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-commerce-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-connectivity-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-context-openapi-original.yml
- description: OAuth2
  flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-customer-service-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-event-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-extension-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-field-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-knowledge-genai-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-machine-learning-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-migration-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-ml-config-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-notification-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-organization-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-platform-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-push-openapi-original.yml
- description: OAuth2
  flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-schema-service-openapi-original.yml
- description: This API uses OAuth 2 with the implicit grant flow
  flows:
  - authorizationUrl: /oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-search-interface-openapi-original.yml
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-search-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: OAuth2
  source: openapi/coveo-search-pages-openapi-original.yml
- description: OAuth2
  flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-search-usage-metrics-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-security-cache-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/coveo-source-logs-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-source-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-tailgate-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: v8
  source: openapi/coveo-usage-analytics-read-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: implicit
  name: v8
  source: openapi/coveo-usage-analytics-write-openapi-original.yml
- flows:
  - authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.cloud.coveo.com/oauth/token
  name: oauth2
  source: openapi/coveo-workspace-openapi-original.yml
scope_count: 1
scope_names:
- full
scopes:
- description: required
  flows:
  - authorizationCode
  - implicit
  scope: full
slug: coveo-scopes
source_filename: coveo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coveo-activity-openapi-original.yml, openapi/coveo-analytics-admin-openapi-original.yml,\n  openapi/coveo-authorization-openapi-original.yml, openapi/coveo-catalog-management-openapi-original.yml,\n  openapi/coveo-commerce-openapi-original.yml, openapi/coveo-connectivity-openapi-original.yml,\n  openapi/coveo-context-openapi-original.yml, openapi/coveo-customer-service-openapi-original.yml,\n  openapi/coveo-event-openapi-original.yml, openapi/coveo-extension-openapi-original.yml, openapi/coveo-field-openapi-original.yml,\n  openapi/coveo-knowledge-genai-openapi-original.yml, openapi/coveo-machine-learning-openapi-original.yml,\n  openapi/coveo-migration-openapi-original.yml, openapi/coveo-ml-config-openapi-original.yml,\n  openapi/coveo-notification-openapi-original.yml, openapi/coveo-organization-openapi-original.yml,\n  openapi/coveo-platform-openapi-original.yml, openapi/coveo-push-openapi-original.yml, openapi/coveo-schema-service-openapi-original.yml,\n\
  \  openapi/coveo-search-interface-openapi-original.yml, openapi/coveo-search-openapi-original.yml,\n  openapi/coveo-search-pages-openapi-original.yml, openapi/coveo-search-usage-metrics-openapi-original.yml,\n  openapi/coveo-security-cache-openapi-original.yml, openapi/coveo-source-logs-openapi-original.yml,\n  openapi/coveo-source-openapi-original.yml, openapi/coveo-tailgate-openapi-original.yml, openapi/coveo-usage-analytics-read-openapi-original.yml,\n  openapi/coveo-usage-analytics-write-openapi-original.yml, openapi/coveo-workspace-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/coveo-activity-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-analytics-admin-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n\
  \    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-authorization-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-catalog-management-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-commerce-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-connectivity-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl:\
  \ https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-context-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n- name: oauth2\n  source: openapi/coveo-customer-service-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n  description: OAuth2\n- name: oauth2\n  source: openapi/coveo-event-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-extension-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-field-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-knowledge-genai-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-machine-learning-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-migration-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-ml-config-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-notification-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-organization-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-platform-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-push-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n\
  - name: oauth2\n  source: openapi/coveo-schema-service-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n  description: OAuth2\n- name: oauth2\n  source: openapi/coveo-search-interface-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: /oauth/authorize\n  description: This API uses OAuth 2 with the implicit grant flow\n- name: oauth2\n  source: openapi/coveo-search-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n  description: This API uses OAuth 2 with the implicit grant flow.\n- name: OAuth2\n  source: openapi/coveo-search-pages-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n- name: oauth2\n  source: openapi/coveo-search-usage-metrics-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n\
  \  description: OAuth2\n- name: oauth2\n  source: openapi/coveo-security-cache-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-source-logs-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n- name: oauth2\n  source: openapi/coveo-source-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: oauth2\n  source: openapi/coveo-tailgate-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\n- name: v8\n  source: openapi/coveo-usage-analytics-read-openapi-original.yml\n\
  \  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n- name: v8\n  source: openapi/coveo-usage-analytics-write-openapi-original.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n- name: oauth2\n  source: openapi/coveo-workspace-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.cloud.coveo.com/oauth/authorize\n    tokenUrl: https://platform.cloud.coveo.com/oauth/token\nscopes:\n- scope: full\n  description: required\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/coveo-activity-openapi-original.yml\n  - openapi/coveo-analytics-admin-openapi-original.yml\n  - openapi/coveo-authorization-openapi-original.yml\n  - openapi/coveo-catalog-management-openapi-original.yml\n  - openapi/coveo-commerce-openapi-original.yml\n  - openapi/coveo-connectivity-openapi-original.yml\n  - openapi/coveo-context-openapi-original.yml\n\
  \  - openapi/coveo-customer-service-openapi-original.yml\n  - openapi/coveo-event-openapi-original.yml\n  - openapi/coveo-extension-openapi-original.yml\n  - openapi/coveo-field-openapi-original.yml\n  - openapi/coveo-knowledge-genai-openapi-original.yml\n  - openapi/coveo-machine-learning-openapi-original.yml\n  - openapi/coveo-migration-openapi-original.yml\n  - openapi/coveo-ml-config-openapi-original.yml\n  - openapi/coveo-notification-openapi-original.yml\n  - openapi/coveo-organization-openapi-original.yml\n  - openapi/coveo-platform-openapi-original.yml\n  - openapi/coveo-push-openapi-original.yml\n  - openapi/coveo-schema-service-openapi-original.yml\n  - openapi/coveo-search-interface-openapi-original.yml\n  - openapi/coveo-search-openapi-original.yml\n  - openapi/coveo-search-pages-openapi-original.yml\n  - openapi/coveo-search-usage-metrics-openapi-original.yml\n  - openapi/coveo-security-cache-openapi-original.yml\n  - openapi/coveo-source-logs-openapi-original.yml\n  - openapi/coveo-source-openapi-original.yml\n\
  \  - openapi/coveo-tailgate-openapi-original.yml\n  - openapi/coveo-usage-analytics-read-openapi-original.yml\n  - openapi/coveo-usage-analytics-write-openapi-original.yml\n  - openapi/coveo-workspace-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coveo/refs/heads/main/scopes/coveo-scopes.yml
summary_line: 1 scope · authorizationCode/implicit
tags:
- AI
- Analytics
- Catalog
- Commerce
- Customers
- Experiences
- Machine Learning
- Personalization
- Recommendations
- Search
token_urls:
- https://platform.cloud.coveo.com/oauth/token
---
