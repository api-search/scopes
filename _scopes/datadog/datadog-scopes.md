---
authorization_urls:
- /oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Datadog Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Datadog publishes 68 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Datadog API on a user''s behalf.


  Tokens are issued from /oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Datadog
provider_slug: datadog
schemes:
- description: This API uses OAuth 2 with the implicit grant flow.
  flows:
  - authorizationUrl: /oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: /oauth2/v1/token
  name: AuthZ
  source: openapi/datadog-api-openapi.yml
scope_count: 68
scope_names:
- apm_api_catalog_read
- apm_api_catalog_write
- apm_read
- apm_service_catalog_read
- apm_service_catalog_write
- appsec_vm_read
- cases_read
- cases_write
- ci_visibility_pipelines_write
- ci_visibility_read
- cloud_cost_management_read
- cloud_cost_management_write
- code_analysis_read
- continuous_profiler_pgo_read
- create_webhooks
- dashboards_embed_share
- dashboards_invite_share
- dashboards_public_share
- dashboards_read
- dashboards_write
- data_scanner_read
- data_scanner_write
- embeddable_graphs_share
- events_read
- hosts_read
- incident_notification_settings_write
- incident_read
- incident_settings_write
- incident_write
- metrics_read
- monitor_config_policy_write
- monitors_downtime
- monitors_read
- monitors_write
- org_management
- security_comments_read
- security_monitoring_filters_read
- security_monitoring_filters_write
- security_monitoring_findings_read
- security_monitoring_notification_profiles_read
- security_monitoring_notification_profiles_write
- security_monitoring_rules_read
- security_monitoring_rules_write
- security_monitoring_signals_read
- security_monitoring_suppressions_read
- security_monitoring_suppressions_write
- security_pipelines_read
- security_pipelines_write
- slos_corrections
- slos_read
- slos_write
- synthetics_global_variable_read
- synthetics_global_variable_write
- synthetics_private_location_read
- synthetics_private_location_write
- synthetics_read
- synthetics_write
- teams_manage
- teams_read
- test_optimization_read
- timeseries_query
- usage_read
- user_access_invite
- user_access_manage
- user_access_read
- workflows_read
- workflows_run
- workflows_write
scopes:
- description: View API catalog and API definitions.
  flows:
  - authorizationCode
  scope: apm_api_catalog_read
- description: Add, modify, and delete API catalog definitions.
  flows:
  - authorizationCode
  scope: apm_api_catalog_write
- description: Read and query APM and Trace Analytics.
  flows:
  - authorizationCode
  scope: apm_read
- description: View service catalog and service definitions.
  flows:
  - authorizationCode
  scope: apm_service_catalog_read
- description: Add, modify, and delete service catalog definitions when those definitions are maintained by Datadog.
  flows:
  - authorizationCode
  scope: apm_service_catalog_write
- description: View infrastructure, application code, and library vulnerabilities. This does not restrict API or inventory SQL access to the vulnerability data source.
  flows:
  - authorizationCode
  scope: appsec_vm_read
- description: View Cases.
  flows:
  - authorizationCode
  scope: cases_read
- description: Create and update cases.
  flows:
  - authorizationCode
  scope: cases_write
- description: Create CI Visibility pipeline spans using the API.
  flows:
  - authorizationCode
  scope: ci_visibility_pipelines_write
- description: View CI Visibility.
  flows:
  - authorizationCode
  scope: ci_visibility_read
- description: View Cloud Cost pages and the cloud cost data source in dashboards and notebooks. For more details, see the Cloud Cost Management docs.
  flows:
  - authorizationCode
  scope: cloud_cost_management_read
- description: Configure cloud cost accounts and global customizations. For more details, see the Cloud Cost Management docs.
  flows:
  - authorizationCode
  scope: cloud_cost_management_write
- description: View Code Analysis.
  flows:
  - authorizationCode
  scope: code_analysis_read
- description: Read and query Continuous Profiler data for Profile-Guided Optimization (PGO).
  flows:
  - authorizationCode
  scope: continuous_profiler_pgo_read
- description: Create webhooks integrations.
  flows:
  - authorizationCode
  scope: create_webhooks
- description: Create, modify, and delete shared dashboards with share type 'embed'.
  flows:
  - authorizationCode
  scope: dashboards_embed_share
- description: Create, modify, and delete shared dashboards with share type 'invite'.
  flows:
  - authorizationCode
  scope: dashboards_invite_share
- description: Generate public and authenticated links to share dashboards or embeddable graphs externally.
  flows:
  - authorizationCode
  scope: dashboards_public_share
- description: View dashboards.
  flows:
  - authorizationCode
  scope: dashboards_read
- description: Create and change dashboards.
  flows:
  - authorizationCode
  scope: dashboards_write
- description: View Data Scanner configurations.
  flows:
  - authorizationCode
  scope: data_scanner_read
- description: Edit Data Scanner configurations.
  flows:
  - authorizationCode
  scope: data_scanner_write
- description: Generate public links to share embeddable graphs externally.
  flows:
  - authorizationCode
  scope: embeddable_graphs_share
- description: Read Events data.
  flows:
  - authorizationCode
  scope: events_read
- description: List hosts and their attributes.
  flows:
  - authorizationCode
  scope: hosts_read
- description: Configure Incidents Notification settings.
  flows:
  - authorizationCode
  scope: incident_notification_settings_write
- description: View incidents in Datadog.
  flows:
  - authorizationCode
  scope: incident_read
- description: Configure Incident Settings.
  flows:
  - authorizationCode
  scope: incident_settings_write
- description: Create, view, and manage incidents in Datadog.
  flows:
  - authorizationCode
  scope: incident_write
- description: View custom metrics.
  flows:
  - authorizationCode
  scope: metrics_read
- description: Edit and delete monitor configuration.
  flows:
  - authorizationCode
  scope: monitor_config_policy_write
- description: Set downtimes to suppress alerts from any monitor in an organization. Mute and unmute monitors. The ability to write monitors is not required to set downtimes.
  flows:
  - authorizationCode
  scope: monitors_downtime
- description: View monitors.
  flows:
  - authorizationCode
  scope: monitors_read
- description: Edit, delete, and resolve individual monitors.
  flows:
  - authorizationCode
  scope: monitors_write
- description: Edit org configurations, including authentication and certain security preferences such as configuring SAML, renaming an org, configuring allowed login methods, creating child orgs, subscribing & unsubscribing from apps in the marketplace, and enabling & disabling Remote Configuration for the entire organization.
  flows:
  - authorizationCode
  scope: org_management
- description: Read comments of vulnerabilities.
  flows:
  - authorizationCode
  scope: security_comments_read
- description: Read Security Filters.
  flows:
  - authorizationCode
  scope: security_monitoring_filters_read
- description: Create, edit, and delete Security Filters.
  flows:
  - authorizationCode
  scope: security_monitoring_filters_write
- description: View a list of findings that include both misconfigurations and identity risks.
  flows:
  - authorizationCode
  scope: security_monitoring_findings_read
- description: View Rule Security Notification rules.
  flows:
  - authorizationCode
  scope: security_monitoring_notification_profiles_read
- description: Create, edit, and delete Security Notification rules.
  flows:
  - authorizationCode
  scope: security_monitoring_notification_profiles_write
- description: Read Detection Rules.
  flows:
  - authorizationCode
  scope: security_monitoring_rules_read
- description: Create and edit Detection Rules.
  flows:
  - authorizationCode
  scope: security_monitoring_rules_write
- description: View Security Signals.
  flows:
  - authorizationCode
  scope: security_monitoring_signals_read
- description: Read Rule Suppressions.
  flows:
  - authorizationCode
  scope: security_monitoring_suppressions_read
- description: Write Rule Suppressions.
  flows:
  - authorizationCode
  scope: security_monitoring_suppressions_write
- description: View Security Pipelines.
  flows:
  - authorizationCode
  scope: security_pipelines_read
- description: Create, edit, and delete CSM Security Pipelines.
  flows:
  - authorizationCode
  scope: security_pipelines_write
- description: Apply, edit, and delete SLO status corrections. A user with this permission can make status corrections, even if they do not have permission to edit those SLOs.
  flows:
  - authorizationCode
  scope: slos_corrections
- description: View SLOs and status corrections.
  flows:
  - authorizationCode
  scope: slos_read
- description: Create, edit, and delete SLOs.
  flows:
  - authorizationCode
  scope: slos_write
- description: View, search, and use Synthetics global variables.
  flows:
  - authorizationCode
  scope: synthetics_global_variable_read
- description: Create, edit, and delete global variables for Synthetics.
  flows:
  - authorizationCode
  scope: synthetics_global_variable_write
- description: View, search, and use Synthetics private locations.
  flows:
  - authorizationCode
  scope: synthetics_private_location_read
- description: Create and delete private locations in addition to having access to the associated installation guidelines.
  flows:
  - authorizationCode
  scope: synthetics_private_location_write
- description: List and view configured Synthetic tests and test results.
  flows:
  - authorizationCode
  scope: synthetics_read
- description: Create, edit, and delete Synthetic tests.
  flows:
  - authorizationCode
  scope: synthetics_write
- description: Manage Teams. Create, delete, rename, and edit metadata of all Teams. To control Team membership across all Teams, use the User Access Manage permission.
  flows:
  - authorizationCode
  scope: teams_manage
- description: Read Teams data. A User with this permission can view Team names, metadata, and which Users are on each Team.
  flows:
  - authorizationCode
  scope: teams_read
- description: View Test Optimization.
  flows:
  - authorizationCode
  scope: test_optimization_read
- description: Query Timeseries data.
  flows:
  - authorizationCode
  scope: timeseries_query
- description: View your organization's usage and usage attribution.
  flows:
  - authorizationCode
  scope: usage_read
- description: Invite other users to your organization.
  flows:
  - authorizationCode
  scope: user_access_invite
- description: Disable users, manage user roles, manage SAML-to-role mappings, and configure logs restriction queries.
  flows:
  - authorizationCode
  scope: user_access_manage
- description: View users and their roles and settings.
  flows:
  - authorizationCode
  scope: user_access_read
- description: View workflows.
  flows:
  - authorizationCode
  scope: workflows_read
- description: Run workflows.
  flows:
  - authorizationCode
  scope: workflows_run
- description: Create, edit, and delete workflows.
  flows:
  - authorizationCode
  scope: workflows_write
slug: datadog-scopes
source_filename: datadog-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datadog-api-openapi.yml\nschemes:\n- name: AuthZ\n  source: openapi/datadog-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/v1/authorize\n    tokenUrl: /oauth2/v1/token\n  description: This API uses OAuth 2 with the implicit grant flow.\nscopes:\n- scope: apm_api_catalog_read\n  description: View API catalog and API definitions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: apm_api_catalog_write\n  description: Add, modify, and delete API catalog definitions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: apm_read\n  description: Read and query APM and Trace Analytics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: apm_service_catalog_read\n  description: View service catalog and service definitions.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/datadog-api-openapi.yml\n- scope: apm_service_catalog_write\n  description: Add, modify, and delete service catalog definitions when those definitions are\n    maintained by Datadog.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: appsec_vm_read\n  description: View infrastructure, application code, and library vulnerabilities. This does\n    not restrict API or inventory SQL access to the vulnerability data source.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: cases_read\n  description: View Cases.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: cases_write\n  description: Create and update cases.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: ci_visibility_pipelines_write\n  description: Create CI Visibility pipeline spans using the API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n\
  - scope: ci_visibility_read\n  description: View CI Visibility.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: cloud_cost_management_read\n  description: View Cloud Cost pages and the cloud cost data source in dashboards and notebooks.\n    For more details, see the Cloud Cost Management docs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: cloud_cost_management_write\n  description: Configure cloud cost accounts and global customizations. For more details, see\n    the Cloud Cost Management docs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: code_analysis_read\n  description: View Code Analysis.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: continuous_profiler_pgo_read\n  description: Read and query Continuous Profiler data for Profile-Guided Optimization (PGO).\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/datadog-api-openapi.yml\n- scope: create_webhooks\n  description: Create webhooks integrations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: dashboards_embed_share\n  description: Create, modify, and delete shared dashboards with share type 'embed'.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: dashboards_invite_share\n  description: Create, modify, and delete shared dashboards with share type 'invite'.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: dashboards_public_share\n  description: Generate public and authenticated links to share dashboards or embeddable graphs\n    externally.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: dashboards_read\n  description: View dashboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: dashboards_write\n  description:\
  \ Create and change dashboards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: data_scanner_read\n  description: View Data Scanner configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: data_scanner_write\n  description: Edit Data Scanner configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: embeddable_graphs_share\n  description: Generate public links to share embeddable graphs externally.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: events_read\n  description: Read Events data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: hosts_read\n  description: List hosts and their attributes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: incident_notification_settings_write\n  description: Configure Incidents\
  \ Notification settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: incident_read\n  description: View incidents in Datadog.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: incident_settings_write\n  description: Configure Incident Settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: incident_write\n  description: Create, view, and manage incidents in Datadog.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: metrics_read\n  description: View custom metrics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: monitor_config_policy_write\n  description: Edit and delete monitor configuration.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: monitors_downtime\n  description: Set downtimes to suppress alerts from any monitor in\
  \ an organization. Mute and\n    unmute monitors. The ability to write monitors is not required to set downtimes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: monitors_read\n  description: View monitors.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: monitors_write\n  description: Edit, delete, and resolve individual monitors.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: org_management\n  description: Edit org configurations, including authentication and certain security preferences\n    such as configuring SAML, renaming an org, configuring allowed login methods, creating child\n    orgs, subscribing & unsubscribing from apps in the marketplace, and enabling & disabling\n    Remote Configuration for the entire organization.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_comments_read\n  description:\
  \ Read comments of vulnerabilities.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_filters_read\n  description: Read Security Filters.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_filters_write\n  description: Create, edit, and delete Security Filters.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_findings_read\n  description: View a list of findings that include both misconfigurations and identity risks.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_notification_profiles_read\n  description: View Rule Security Notification rules.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_notification_profiles_write\n  description: Create, edit, and delete Security Notification\
  \ rules.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_rules_read\n  description: Read Detection Rules.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_rules_write\n  description: Create and edit Detection Rules.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_signals_read\n  description: View Security Signals.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_suppressions_read\n  description: Read Rule Suppressions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_monitoring_suppressions_write\n  description: Write Rule Suppressions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_pipelines_read\n  description: View Security Pipelines.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: security_pipelines_write\n  description: Create, edit, and delete CSM Security Pipelines.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: slos_corrections\n  description: Apply, edit, and delete SLO status corrections. A user with this permission can\n    make status corrections, even if they do not have permission to edit those SLOs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: slos_read\n  description: View SLOs and status corrections.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: slos_write\n  description: Create, edit, and delete SLOs.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: synthetics_global_variable_read\n  description: View, search, and use Synthetics global variables.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: synthetics_global_variable_write\n  description: Create, edit, and delete global variables for Synthetics.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: synthetics_private_location_read\n  description: View, search, and use Synthetics private locations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: synthetics_private_location_write\n  description: Create and delete private locations in addition to having access to the associated\n    installation guidelines.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: synthetics_read\n  description: List and view configured Synthetic tests and test results.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: synthetics_write\n  description: Create, edit, and delete Synthetic tests.\n  flows:\n  - authorizationCode\n \
  \ sources:\n  - openapi/datadog-api-openapi.yml\n- scope: teams_manage\n  description: Manage Teams. Create, delete, rename, and edit metadata of all Teams. To control\n    Team membership across all Teams, use the User Access Manage permission.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: teams_read\n  description: Read Teams data. A User with this permission can view Team names, metadata, and\n    which Users are on each Team.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: test_optimization_read\n  description: View Test Optimization.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: timeseries_query\n  description: Query Timeseries data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: usage_read\n  description: View your organization's usage and usage attribution.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/datadog-api-openapi.yml\n- scope: user_access_invite\n  description: Invite other users to your organization.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: user_access_manage\n  description: Disable users, manage user roles, manage SAML-to-role mappings, and configure\n    logs restriction queries.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: user_access_read\n  description: View users and their roles and settings.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: workflows_read\n  description: View workflows.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: workflows_run\n  description: Run workflows.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/datadog-api-openapi.yml\n- scope: workflows_write\n  description: Create, edit, and delete workflows.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/datadog-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/scopes/datadog-scopes.yml
summary_line: 68 scopes · authorizationCode
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
token_urls:
- /oauth2/v1/token
---
