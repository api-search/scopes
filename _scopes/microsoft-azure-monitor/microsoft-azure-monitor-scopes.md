---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Azure Monitor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure Monitor publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure Monitor API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-action-groups-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-activity-log-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-alerts-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-application-insights-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-autoscale-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-data-collection-endpoints-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-data-collection-rules-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-diagnostic-settings-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-logs-ingestion-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-logs-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-metric-definitions-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-metrics-batch-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-metrics-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-private-link-scopes-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/azure-monitor-scheduled-query-rules-openapi.yml
scope_count: 4
scope_names:
- https://api.applicationinsights.io/.default
- https://api.loganalytics.io/.default
- https://management.azure.com/.default
- https://monitor.azure.com/.default
scopes:
- description: Access Application Insights API
  flows:
  - clientCredentials
  scope: https://api.applicationinsights.io/.default
- description: Access Log Analytics API
  flows:
  - clientCredentials
  scope: https://api.loganalytics.io/.default
- description: Access Azure Management API
  flows:
  - clientCredentials
  scope: https://management.azure.com/.default
- description: Access Azure Monitor ingestion
  flows:
  - clientCredentials
  scope: https://monitor.azure.com/.default
slug: microsoft-azure-monitor-scopes
source_filename: microsoft-azure-monitor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-monitor-action-groups-openapi.yml, openapi/azure-monitor-activity-log-openapi.yml,\n  openapi/azure-monitor-alerts-openapi.yml, openapi/azure-monitor-application-insights-openapi.yml,\n  openapi/azure-monitor-autoscale-openapi.yml, openapi/azure-monitor-data-collection-endpoints-openapi.yml,\n  openapi/azure-monitor-data-collection-rules-openapi.yml, openapi/azure-monitor-diagnostic-settings-openapi.yml,\n  openapi/azure-monitor-logs-ingestion-openapi.yml, openapi/azure-monitor-logs-openapi.yml,\n  openapi/azure-monitor-metric-definitions-openapi.yml, openapi/azure-monitor-metrics-batch-openapi.yml,\n  openapi/azure-monitor-metrics-openapi.yml, openapi/azure-monitor-private-link-scopes-openapi.yml,\n  openapi/azure-monitor-scheduled-query-rules-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/azure-monitor-action-groups-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n\
  - name: oauth2\n  source: openapi/azure-monitor-activity-log-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-alerts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-application-insights-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-autoscale-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-data-collection-endpoints-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-data-collection-rules-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-diagnostic-settings-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-logs-ingestion-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-logs-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-metric-definitions-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-metrics-batch-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-metrics-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-private-link-scopes-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n- name: oauth2\n  source: openapi/azure-monitor-scheduled-query-rules-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\nscopes:\n- scope: https://api.applicationinsights.io/.default\n  description: Access Application Insights API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-monitor-application-insights-openapi.yml\n- scope: https://api.loganalytics.io/.default\n  description: Access Log Analytics API\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/azure-monitor-logs-openapi.yml\n- scope: https://management.azure.com/.default\n  description: Access Azure Management API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-monitor-action-groups-openapi.yml\n  - openapi/azure-monitor-activity-log-openapi.yml\n  - openapi/azure-monitor-alerts-openapi.yml\n  - openapi/azure-monitor-autoscale-openapi.yml\n  - openapi/azure-monitor-data-collection-endpoints-openapi.yml\n  - openapi/azure-monitor-data-collection-rules-openapi.yml\n  - openapi/azure-monitor-diagnostic-settings-openapi.yml\n  - openapi/azure-monitor-metric-definitions-openapi.yml\n  - openapi/azure-monitor-metrics-batch-openapi.yml\n  - openapi/azure-monitor-metrics-openapi.yml\n  - openapi/azure-monitor-private-link-scopes-openapi.yml\n  - openapi/azure-monitor-scheduled-query-rules-openapi.yml\n- scope: https://monitor.azure.com/.default\n  description: Access Azure Monitor ingestion\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/azure-monitor-logs-ingestion-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/scopes/microsoft-azure-monitor-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
token_urls:
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
