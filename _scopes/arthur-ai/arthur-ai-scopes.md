---
api_specs:
- filename: arthur-ai-platform-openapi.json
  format: json
  label: Arthur Platform API
  slug: arthur-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arthur-ai/refs/heads/main/openapi/arthur-ai-platform-openapi.json
authorization_urls:
- https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Arthur Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Arthur AI publishes 191 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arthur AI API on a user''s behalf.


  Tokens are issued from https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arthur AI
provider_slug: arthur-ai
schemes:
- flows:
  - authorizationUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
  name: OAuth2AuthorizationCode
  source: openapi/arthur-ai-platform-openapi.json
scope_count: 191
scope_names:
- agent_read
- alert_rule_delete
- alert_rule_read
- alert_rule_update
- available_dataset_create_data_retrieval
- available_dataset_delete_data_retrieval
- available_dataset_get_data_retrieval
- available_dataset_put_data_retrieval
- available_dataset_put_schema
- available_dataset_read
- connector_create_available_dataset
- connector_create_dataset
- connector_delete
- connector_get_sensitive_fields
- connector_list_available_datasets
- connector_list_datasets
- connector_put_available_datasets
- connector_put_check_result
- connector_read
- connector_update
- custom_aggregation_delete
- custom_aggregation_put
- custom_aggregation_read
- custom_aggregation_test_create_results
- custom_aggregation_test_delete
- custom_aggregation_test_read
- custom_aggregation_test_read_results
- custom_aggregation_update
- data_plane_association_delete
- data_plane_delete
- data_plane_jobs_dequeue_next
- data_plane_list_associations
- data_plane_read
- data_plane_regenerate_creds
- data_plane_update
- dataset_create_data_retrieval
- dataset_delete
- dataset_delete_data_retrieval
- dataset_get_data_retrieval
- dataset_put_data_retrieval
- dataset_put_schema
- dataset_read
- dataset_update
- delete_user
- group_create_group_membership
- group_delete
- group_delete_group_membership
- group_list_role_bindings
- group_list_users
- group_read
- group_update
- model_add_metrics_for_version
- model_alert_read
- model_check_compliance
- model_create_alert
- model_create_alert_rule
- model_create_metric_version
- model_delete
- model_list_alert_rules
- model_list_alerts
- model_list_attestations
- model_list_metric_versions
- model_list_policy_assignments
- model_metrics_schedule_delete
- model_metrics_schedule_update
- model_put_metric_config
- model_query_metrics
- model_read
- model_task_delete
- model_task_delete_connection_info
- model_task_get_connection_info
- model_task_put_connection_info
- model_task_put_state_cache
- model_task_read
- model_task_regenerate_validation_key
- model_task_sync
- model_task_update
- model_update
- organization_create_group
- organization_create_policy
- organization_create_role_binding
- organization_create_service_account
- organization_create_user
- organization_create_workspace
- organization_delete
- organization_invite_user
- organization_list_agent_llm_models
- organization_list_agent_tools
- organization_list_group_memberships
- organization_list_groups
- organization_list_models
- organization_list_policies
- organization_list_policy_assignments
- organization_list_policy_compliance
- organization_list_role_bindings
- organization_list_roles
- organization_list_unregistered_agents
- organization_list_users
- organization_list_workspaces
- organization_read
- organization_update
- policy_alert_rule_delete
- policy_alert_rule_read
- policy_alert_rule_update
- policy_assignment_check_compliance
- policy_assignment_create
- policy_assignment_create_attestation
- policy_assignment_delete
- policy_assignment_list_attestations
- policy_assignment_read
- policy_assignment_set_compliance_status
- policy_attestation_rule_delete
- policy_attestation_rule_read
- policy_attestation_rule_update
- policy_check_compliance
- policy_create_alert_rule
- policy_create_attestation_rule
- policy_delete
- policy_list_alert_rules
- policy_list_assignments
- policy_list_attestation_rules
- policy_list_compliance_history
- policy_read
- policy_update
- project_create_available_dataset
- project_create_connector
- project_create_dataset
- project_create_job
- project_create_model
- project_create_model_link_task
- project_create_model_task
- project_create_role_binding
- project_delete
- project_generate_metrics_spec
- project_job_append_errors
- project_job_append_logs
- project_job_put_state
- project_job_read
- project_job_read_errors
- project_job_read_logs
- project_job_read_runs
- project_job_update
- project_list_connectors
- project_list_data_plane_associations
- project_list_datasets
- project_list_jobs
- project_list_models
- project_list_role_bindings
- project_read
- project_update
- unregistered_agent_patch
- user_list_role_bindings
- user_regenerate_creds
- user_update
- webhook_delete
- webhook_read
- webhook_update
- workspace_check_all_policies_compliance
- workspace_create_custom_aggregation
- workspace_create_custom_aggregation_test
- workspace_create_data_plane
- workspace_create_data_plane_association
- workspace_create_project
- workspace_create_role_binding
- workspace_create_webhook
- workspace_delete
- workspace_get_statistics
- workspace_list_agent_data_sources
- workspace_list_agent_llm_models
- workspace_list_agent_sub_agents
- workspace_list_agent_tools
- workspace_list_agents
- workspace_list_alert_rules
- workspace_list_alerts
- workspace_list_custom_aggregation_tests
- workspace_list_custom_aggregations
- workspace_list_data_plane_associations
- workspace_list_data_planes
- workspace_list_datasets
- workspace_list_models
- workspace_list_policy_assignments
- workspace_list_policy_compliance
- workspace_list_projects
- workspace_list_role_bindings
- workspace_list_unregistered_agents
- workspace_list_webhooks
- workspace_read
- workspace_test_webhook
- workspace_update
- workspace_upsert_agents
- workspace_validate_custom_aggregation
scopes:
- description: ''
  flows: []
  scope: agent_read
- description: ''
  flows: []
  scope: alert_rule_delete
- description: ''
  flows: []
  scope: alert_rule_read
- description: ''
  flows: []
  scope: alert_rule_update
- description: ''
  flows: []
  scope: available_dataset_create_data_retrieval
- description: ''
  flows: []
  scope: available_dataset_delete_data_retrieval
- description: ''
  flows: []
  scope: available_dataset_get_data_retrieval
- description: ''
  flows: []
  scope: available_dataset_put_data_retrieval
- description: ''
  flows: []
  scope: available_dataset_put_schema
- description: ''
  flows: []
  scope: available_dataset_read
- description: ''
  flows: []
  scope: connector_create_available_dataset
- description: ''
  flows: []
  scope: connector_create_dataset
- description: ''
  flows: []
  scope: connector_delete
- description: ''
  flows: []
  scope: connector_get_sensitive_fields
- description: ''
  flows: []
  scope: connector_list_available_datasets
- description: ''
  flows: []
  scope: connector_list_datasets
- description: ''
  flows: []
  scope: connector_put_available_datasets
- description: ''
  flows: []
  scope: connector_put_check_result
- description: ''
  flows: []
  scope: connector_read
- description: ''
  flows: []
  scope: connector_update
- description: ''
  flows: []
  scope: custom_aggregation_delete
- description: ''
  flows: []
  scope: custom_aggregation_put
- description: ''
  flows: []
  scope: custom_aggregation_read
- description: ''
  flows: []
  scope: custom_aggregation_test_create_results
- description: ''
  flows: []
  scope: custom_aggregation_test_delete
- description: ''
  flows: []
  scope: custom_aggregation_test_read
- description: ''
  flows: []
  scope: custom_aggregation_test_read_results
- description: ''
  flows: []
  scope: custom_aggregation_update
- description: ''
  flows: []
  scope: data_plane_association_delete
- description: ''
  flows: []
  scope: data_plane_delete
- description: ''
  flows: []
  scope: data_plane_jobs_dequeue_next
- description: ''
  flows: []
  scope: data_plane_list_associations
- description: ''
  flows: []
  scope: data_plane_read
- description: ''
  flows: []
  scope: data_plane_regenerate_creds
- description: ''
  flows: []
  scope: data_plane_update
- description: ''
  flows: []
  scope: dataset_create_data_retrieval
- description: ''
  flows: []
  scope: dataset_delete
- description: ''
  flows: []
  scope: dataset_delete_data_retrieval
- description: ''
  flows: []
  scope: dataset_get_data_retrieval
- description: ''
  flows: []
  scope: dataset_put_data_retrieval
- description: ''
  flows: []
  scope: dataset_put_schema
- description: ''
  flows: []
  scope: dataset_read
- description: ''
  flows: []
  scope: dataset_update
- description: ''
  flows: []
  scope: delete_user
- description: ''
  flows: []
  scope: group_create_group_membership
- description: ''
  flows: []
  scope: group_delete
- description: ''
  flows: []
  scope: group_delete_group_membership
- description: ''
  flows: []
  scope: group_list_role_bindings
- description: ''
  flows: []
  scope: group_list_users
- description: ''
  flows: []
  scope: group_read
- description: ''
  flows: []
  scope: group_update
- description: ''
  flows: []
  scope: model_add_metrics_for_version
- description: ''
  flows: []
  scope: model_alert_read
- description: ''
  flows: []
  scope: model_check_compliance
- description: ''
  flows: []
  scope: model_create_alert
- description: ''
  flows: []
  scope: model_create_alert_rule
- description: ''
  flows: []
  scope: model_create_metric_version
- description: ''
  flows: []
  scope: model_delete
- description: ''
  flows: []
  scope: model_list_alert_rules
- description: ''
  flows: []
  scope: model_list_alerts
- description: ''
  flows: []
  scope: model_list_attestations
- description: ''
  flows: []
  scope: model_list_metric_versions
- description: ''
  flows: []
  scope: model_list_policy_assignments
- description: ''
  flows: []
  scope: model_metrics_schedule_delete
- description: ''
  flows: []
  scope: model_metrics_schedule_update
- description: ''
  flows: []
  scope: model_put_metric_config
- description: ''
  flows: []
  scope: model_query_metrics
- description: ''
  flows: []
  scope: model_read
- description: ''
  flows: []
  scope: model_task_delete
- description: ''
  flows: []
  scope: model_task_delete_connection_info
- description: ''
  flows: []
  scope: model_task_get_connection_info
- description: ''
  flows: []
  scope: model_task_put_connection_info
- description: ''
  flows: []
  scope: model_task_put_state_cache
- description: ''
  flows: []
  scope: model_task_read
- description: ''
  flows: []
  scope: model_task_regenerate_validation_key
- description: ''
  flows: []
  scope: model_task_sync
- description: ''
  flows: []
  scope: model_task_update
- description: ''
  flows: []
  scope: model_update
- description: ''
  flows: []
  scope: organization_create_group
- description: ''
  flows: []
  scope: organization_create_policy
- description: ''
  flows: []
  scope: organization_create_role_binding
- description: ''
  flows: []
  scope: organization_create_service_account
- description: ''
  flows: []
  scope: organization_create_user
- description: ''
  flows: []
  scope: organization_create_workspace
- description: ''
  flows: []
  scope: organization_delete
- description: ''
  flows: []
  scope: organization_invite_user
- description: ''
  flows: []
  scope: organization_list_agent_llm_models
- description: ''
  flows: []
  scope: organization_list_agent_tools
- description: ''
  flows: []
  scope: organization_list_group_memberships
- description: ''
  flows: []
  scope: organization_list_groups
- description: ''
  flows: []
  scope: organization_list_models
- description: ''
  flows: []
  scope: organization_list_policies
- description: ''
  flows: []
  scope: organization_list_policy_assignments
- description: ''
  flows: []
  scope: organization_list_policy_compliance
- description: ''
  flows: []
  scope: organization_list_role_bindings
- description: ''
  flows: []
  scope: organization_list_roles
- description: ''
  flows: []
  scope: organization_list_unregistered_agents
- description: ''
  flows: []
  scope: organization_list_users
- description: ''
  flows: []
  scope: organization_list_workspaces
- description: ''
  flows: []
  scope: organization_read
- description: ''
  flows: []
  scope: organization_update
- description: ''
  flows: []
  scope: policy_alert_rule_delete
- description: ''
  flows: []
  scope: policy_alert_rule_read
- description: ''
  flows: []
  scope: policy_alert_rule_update
- description: ''
  flows: []
  scope: policy_assignment_check_compliance
- description: ''
  flows: []
  scope: policy_assignment_create
- description: ''
  flows: []
  scope: policy_assignment_create_attestation
- description: ''
  flows: []
  scope: policy_assignment_delete
- description: ''
  flows: []
  scope: policy_assignment_list_attestations
- description: ''
  flows: []
  scope: policy_assignment_read
- description: ''
  flows: []
  scope: policy_assignment_set_compliance_status
- description: ''
  flows: []
  scope: policy_attestation_rule_delete
- description: ''
  flows: []
  scope: policy_attestation_rule_read
- description: ''
  flows: []
  scope: policy_attestation_rule_update
- description: ''
  flows: []
  scope: policy_check_compliance
- description: ''
  flows: []
  scope: policy_create_alert_rule
- description: ''
  flows: []
  scope: policy_create_attestation_rule
- description: ''
  flows: []
  scope: policy_delete
- description: ''
  flows: []
  scope: policy_list_alert_rules
- description: ''
  flows: []
  scope: policy_list_assignments
- description: ''
  flows: []
  scope: policy_list_attestation_rules
- description: ''
  flows: []
  scope: policy_list_compliance_history
- description: ''
  flows: []
  scope: policy_read
- description: ''
  flows: []
  scope: policy_update
- description: ''
  flows: []
  scope: project_create_available_dataset
- description: ''
  flows: []
  scope: project_create_connector
- description: ''
  flows: []
  scope: project_create_dataset
- description: ''
  flows: []
  scope: project_create_job
- description: ''
  flows: []
  scope: project_create_model
- description: ''
  flows: []
  scope: project_create_model_link_task
- description: ''
  flows: []
  scope: project_create_model_task
- description: ''
  flows: []
  scope: project_create_role_binding
- description: ''
  flows: []
  scope: project_delete
- description: ''
  flows: []
  scope: project_generate_metrics_spec
- description: ''
  flows: []
  scope: project_job_append_errors
- description: ''
  flows: []
  scope: project_job_append_logs
- description: ''
  flows: []
  scope: project_job_put_state
- description: ''
  flows: []
  scope: project_job_read
- description: ''
  flows: []
  scope: project_job_read_errors
- description: ''
  flows: []
  scope: project_job_read_logs
- description: ''
  flows: []
  scope: project_job_read_runs
- description: ''
  flows: []
  scope: project_job_update
- description: ''
  flows: []
  scope: project_list_connectors
- description: ''
  flows: []
  scope: project_list_data_plane_associations
- description: ''
  flows: []
  scope: project_list_datasets
- description: ''
  flows: []
  scope: project_list_jobs
- description: ''
  flows: []
  scope: project_list_models
- description: ''
  flows: []
  scope: project_list_role_bindings
- description: ''
  flows: []
  scope: project_read
- description: ''
  flows: []
  scope: project_update
- description: ''
  flows: []
  scope: unregistered_agent_patch
- description: ''
  flows: []
  scope: user_list_role_bindings
- description: ''
  flows: []
  scope: user_regenerate_creds
- description: ''
  flows: []
  scope: user_update
- description: ''
  flows: []
  scope: webhook_delete
- description: ''
  flows: []
  scope: webhook_read
- description: ''
  flows: []
  scope: webhook_update
- description: ''
  flows: []
  scope: workspace_check_all_policies_compliance
- description: ''
  flows: []
  scope: workspace_create_custom_aggregation
- description: ''
  flows: []
  scope: workspace_create_custom_aggregation_test
- description: ''
  flows: []
  scope: workspace_create_data_plane
- description: ''
  flows: []
  scope: workspace_create_data_plane_association
- description: ''
  flows: []
  scope: workspace_create_project
- description: ''
  flows: []
  scope: workspace_create_role_binding
- description: ''
  flows: []
  scope: workspace_create_webhook
- description: ''
  flows: []
  scope: workspace_delete
- description: ''
  flows: []
  scope: workspace_get_statistics
- description: ''
  flows: []
  scope: workspace_list_agent_data_sources
- description: ''
  flows: []
  scope: workspace_list_agent_llm_models
- description: ''
  flows: []
  scope: workspace_list_agent_sub_agents
- description: ''
  flows: []
  scope: workspace_list_agent_tools
- description: ''
  flows: []
  scope: workspace_list_agents
- description: ''
  flows: []
  scope: workspace_list_alert_rules
- description: ''
  flows: []
  scope: workspace_list_alerts
- description: ''
  flows: []
  scope: workspace_list_custom_aggregation_tests
- description: ''
  flows: []
  scope: workspace_list_custom_aggregations
- description: ''
  flows: []
  scope: workspace_list_data_plane_associations
- description: ''
  flows: []
  scope: workspace_list_data_planes
- description: ''
  flows: []
  scope: workspace_list_datasets
- description: ''
  flows: []
  scope: workspace_list_models
- description: ''
  flows: []
  scope: workspace_list_policy_assignments
- description: ''
  flows: []
  scope: workspace_list_policy_compliance
- description: ''
  flows: []
  scope: workspace_list_projects
- description: ''
  flows: []
  scope: workspace_list_role_bindings
- description: ''
  flows: []
  scope: workspace_list_unregistered_agents
- description: ''
  flows: []
  scope: workspace_list_webhooks
- description: ''
  flows: []
  scope: workspace_read
- description: ''
  flows: []
  scope: workspace_test_webhook
- description: ''
  flows: []
  scope: workspace_update
- description: ''
  flows: []
  scope: workspace_upsert_agents
- description: ''
  flows: []
  scope: workspace_validate_custom_aggregation
slug: arthur-ai-scopes
source_filename: arthur-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/arthur-ai-platform-openapi.json\nschemes:\n- name: OAuth2AuthorizationCode\n  source: openapi/arthur-ai-platform-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/auth\n    tokenUrl: https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token\nscopes:\n- scope: agent_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: alert_rule_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: alert_rule_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: alert_rule_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: available_dataset_create_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: available_dataset_delete_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: available_dataset_get_data_retrieval\n\
  \  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: available_dataset_put_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: available_dataset_put_schema\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: available_dataset_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_create_available_dataset\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_create_dataset\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_get_sensitive_fields\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_list_available_datasets\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_list_datasets\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_put_available_datasets\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: connector_put_check_result\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: connector_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_put\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_test_create_results\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_test_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_test_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_test_read_results\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: custom_aggregation_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: data_plane_association_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: data_plane_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: data_plane_jobs_dequeue_next\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: data_plane_list_associations\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: data_plane_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: data_plane_regenerate_creds\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: data_plane_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_create_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_delete_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_get_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: dataset_put_data_retrieval\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_put_schema\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: dataset_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: delete_user\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_create_group_membership\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_delete_group_membership\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_list_role_bindings\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_list_users\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: group_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: model_add_metrics_for_version\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_alert_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_check_compliance\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_create_alert\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_create_alert_rule\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_create_metric_version\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_list_alert_rules\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_list_alerts\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_list_attestations\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_list_metric_versions\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_list_policy_assignments\n\
  \  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_metrics_schedule_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_metrics_schedule_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_put_metric_config\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_query_metrics\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_delete_connection_info\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_get_connection_info\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_put_connection_info\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_put_state_cache\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_read\n\
  \  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_regenerate_validation_key\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_sync\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_task_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: model_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_create_group\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_create_policy\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_create_role_binding\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_create_service_account\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_create_user\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_create_workspace\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_delete\n\
  \  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_invite_user\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_agent_llm_models\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_agent_tools\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_group_memberships\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_groups\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_models\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_policies\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_policy_assignments\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_policy_compliance\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_role_bindings\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: organization_list_roles\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_unregistered_agents\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_users\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_list_workspaces\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: organization_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_alert_rule_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_alert_rule_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_alert_rule_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_assignment_check_compliance\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_assignment_create\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: policy_assignment_create_attestation\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_assignment_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_assignment_list_attestations\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_assignment_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_assignment_set_compliance_status\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_attestation_rule_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_attestation_rule_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_attestation_rule_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_check_compliance\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_create_alert_rule\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_create_attestation_rule\n\
  \  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_list_alert_rules\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_list_assignments\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_list_attestation_rules\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_list_compliance_history\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: policy_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_available_dataset\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_connector\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_dataset\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_job\n  sources:\n\
  \  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_model\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_model_link_task\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_model_task\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_create_role_binding\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_generate_metrics_spec\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_append_errors\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_append_logs\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_put_state\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_read_errors\n  sources:\n\
  \  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_read_logs\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_read_runs\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_job_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_list_connectors\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_list_data_plane_associations\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_list_datasets\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_list_jobs\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_list_models\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_list_role_bindings\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: project_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: unregistered_agent_patch\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: user_list_role_bindings\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: user_regenerate_creds\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: user_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: webhook_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: webhook_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: webhook_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_check_all_policies_compliance\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_create_custom_aggregation\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_create_custom_aggregation_test\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_create_data_plane\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: workspace_create_data_plane_association\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_create_project\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_create_role_binding\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_create_webhook\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_delete\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_get_statistics\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_agent_data_sources\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_agent_llm_models\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_agent_sub_agents\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_agent_tools\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_agents\n  sources:\n\
  \  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_alert_rules\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_alerts\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_custom_aggregation_tests\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_custom_aggregations\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_data_plane_associations\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_data_planes\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_datasets\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_models\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_policy_assignments\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_policy_compliance\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n\
  - scope: workspace_list_projects\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_role_bindings\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_unregistered_agents\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_list_webhooks\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_read\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_test_webhook\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_update\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_upsert_agents\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n- scope: workspace_validate_custom_aggregation\n  sources:\n  - openapi/arthur-ai-platform-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthur-ai/refs/heads/main/scopes/arthur-ai-scopes.yml
summary_line: 191 scopes · authorizationCode
tags:
- Company
- AI
- AI Governance
- AI Observability
- Machine Learning
- LLM Evaluation
- Model Monitoring
- MLOps
- Guardrails
- Agents
token_urls:
- https://platform-auth.arthur.ai/realms/arthur/protocol/openid-connect/token
---
