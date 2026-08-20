---
api_specs:
- filename: apollo-io-enrichment-api-openapi.yml
  format: yaml
  label: Apollo.io Enrichment API
  slug: apollo-io-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-enrichment-api-openapi.yml
- filename: apollo-io-search-api-openapi.yml
  format: yaml
  label: Apollo.io Search API
  slug: apollo-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-search-api-openapi.yml
- filename: apollo-io-accounts-api-openapi.yml
  format: yaml
  label: Apollo.io Accounts API
  slug: apollo-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-accounts-api-openapi.yml
- filename: apollo-io-contacts-api-openapi.yml
  format: yaml
  label: Apollo.io Contacts API
  slug: apollo-io-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-contacts-api-openapi.yml
- filename: apollo-io-deals-api-openapi.yml
  format: yaml
  label: Apollo.io Deals API
  slug: apollo-io-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-deals-api-openapi.yml
- filename: apollo-io-sequences-api-openapi.yml
  format: yaml
  label: Apollo.io Sequences API
  slug: apollo-io-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-sequences-api-openapi.yml
- filename: apollo-io-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo.io Emailer Messages API
  slug: apollo-io-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-emailer-messages-api-openapi.yml
- filename: apollo-io-tasks-api-openapi.yml
  format: yaml
  label: Apollo.io Tasks API
  slug: apollo-io-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-tasks-api-openapi.yml
- filename: apollo-io-calls-api-openapi.yml
  format: yaml
  label: Apollo.io Calls API
  slug: apollo-io-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-calls-api-openapi.yml
- filename: apollo-io-conversations-api-openapi.yml
  format: yaml
  label: Apollo.io Conversations API
  slug: apollo-io-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-conversations-api-openapi.yml
- filename: apollo-io-analytics-api-openapi.yml
  format: yaml
  label: Apollo.io Analytics API
  slug: apollo-io-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-analytics-api-openapi.yml
- filename: apollo-io-fields-api-openapi.yml
  format: yaml
  label: Apollo.io Fields API
  slug: apollo-io-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-fields-api-openapi.yml
- filename: apollo-io-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo.io Miscellaneous API
  slug: apollo-io-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/openapi/apollo-io-miscellaneous-api-openapi.yml
authorization_urls:
- https://app.apollo.io/#/oauth/authorize
- https://mcp.apollo.io/mcp/oauth_metadata/redirect_to_authorize
description: ''
docs: https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Apollo Io Scopes
name_suffix: OAuth Scopes
note: Apollo's OpenAPI declares OAuth as an http/bearer scheme, so the scope set is not in the spec's securitySchemes. The authoritative anonymous source is the RFC 8414 authorization-server metadata Apollo serves at mcp.apollo.io, cross-referenced against the per-operation `OAuth scopes:` line published in every endpoint reference page. Partners select scopes at OAuth app registration; read_user_profile and app_scopes are added by Apollo automatically.
overview: 'Apollo.io publishes 91 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Apollo.io API on a user''s behalf.


  Tokens are issued from https://app.apollo.io/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apollo.io
provider_slug: apollo-io
schemes:
- flows:
  - authorizationUrl: https://app.apollo.io/#/oauth/authorize
    docs: https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners
    flow: authorizationCode
    tokenUrl: https://app.apollo.io/api/v1/oauth/token
  - audience: Apollo MCP (mcp.apollo.io)
    authorizationUrl: https://mcp.apollo.io/mcp/oauth_metadata/redirect_to_authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://mcp.apollo.io/api/v1/oauth/applications/register_oauth_client
    revocationUrl: https://mcp.apollo.io/api/v1/oauth/revoke
    tokenUrl: https://mcp.apollo.io/api/v1/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: bearerAuth
  type: oauth2
scope_count: 91
scope_names:
- read_user_profile
- app_scopes
- people_bulk_match
- organizations_bulk_enrich
- organizations_enrich
- people_match
- webhook_result_read
- mixed_people_api_search
- organizations_job_posting
- mixed_companies_search
- organizations_search
- contact_write
- contact_update
- contacts_search
- contact_read
- account_write
- account_update
- context_center_read
- context_center_write
- emailer_campaigns_search
- emailer_campaigns_create
- emailer_campaigns_update
- emailer_campaigns_approve
- emailer_campaigns_add_contact_ids
- emailer_campaigns_remove_or_stop_contact_ids
- emailer_schedules_list
- emailer_messages_search
- emailer_messages_create
- emailer_messages_send_now
- emailer_messages_email_send_status
- emailer_messages_get_content
- emailer_campaigns_activity_feed
- report_sync
- agent_task
- email_accounts_list
- custom_objects_write
- custom_objects_read
- custom_field_write
- opportunity_write
- opportunities_list
- opportunity_read
- tasks_create
- tasks_list
- email_account_purchase_list
- email_account_purchase_create
- domain_purchase_list
- domain_purchase_create
- domain_authentication_status
- account_bulk_create
- contacts_bulk_create
- api_usage_stats_read
- credit_usage_stats_read
- users_list
- custom_fields_list
- conversation_intelligence_search
- conversation_intelligence_show
- tags_list
- lists_create
- lists_update
- lists_add_entities
- lists_remove_entities
- website_visitor_domain_tracker_read
- website_visitor_domain_tracker_update
- website_visitor_domain_tracker_send_install_email
- website_visitor_domain_tracker_install_script
- website_visitors_read
- emailer_campaign_read
- account_owners_update
- account_read
- account_stages_list
- account_stages_update
- accounts_search
- contact_owners_update
- contact_stages_list
- contact_stages_update
- contacts_bulk_update
- conversations_export
- conversations_find_export
- conversations_search
- conversations_show
- emailer_campaigns_abort
- emailer_campaigns_archive
- notes_list
- opportunity_stages_list
- opportunity_update
- organization_read
- organizations_news_articles
- person_read
- phone_call_search
- phone_call_update
- phone_call_write
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: read_user_profile
- description: ''
  flows:
  - authorizationCode
  scope: app_scopes
- description: ''
  flows:
  - authorizationCode
  scope: people_bulk_match
- description: ''
  flows:
  - authorizationCode
  scope: organizations_bulk_enrich
- description: ''
  flows:
  - authorizationCode
  scope: organizations_enrich
- description: ''
  flows:
  - authorizationCode
  scope: people_match
- description: ''
  flows:
  - authorizationCode
  scope: webhook_result_read
- description: ''
  flows:
  - authorizationCode
  scope: mixed_people_api_search
- description: ''
  flows:
  - authorizationCode
  scope: organizations_job_posting
- description: ''
  flows:
  - authorizationCode
  scope: mixed_companies_search
- description: ''
  flows:
  - authorizationCode
  scope: organizations_search
- description: ''
  flows:
  - authorizationCode
  scope: contact_write
- description: ''
  flows:
  - authorizationCode
  scope: contact_update
- description: ''
  flows:
  - authorizationCode
  scope: contacts_search
- description: ''
  flows:
  - authorizationCode
  scope: contact_read
- description: ''
  flows:
  - authorizationCode
  scope: account_write
- description: ''
  flows:
  - authorizationCode
  scope: account_update
- description: ''
  flows:
  - authorizationCode
  scope: context_center_read
- description: ''
  flows:
  - authorizationCode
  scope: context_center_write
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_search
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_create
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_update
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_approve
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_add_contact_ids
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_remove_or_stop_contact_ids
- description: ''
  flows:
  - authorizationCode
  scope: emailer_schedules_list
- description: ''
  flows:
  - authorizationCode
  scope: emailer_messages_search
- description: ''
  flows:
  - authorizationCode
  scope: emailer_messages_create
- description: ''
  flows:
  - authorizationCode
  scope: emailer_messages_send_now
- description: ''
  flows:
  - authorizationCode
  scope: emailer_messages_email_send_status
- description: ''
  flows:
  - authorizationCode
  scope: emailer_messages_get_content
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_activity_feed
- description: ''
  flows:
  - authorizationCode
  scope: report_sync
- description: ''
  flows:
  - authorizationCode
  scope: agent_task
- description: ''
  flows:
  - authorizationCode
  scope: email_accounts_list
- description: ''
  flows:
  - authorizationCode
  scope: custom_objects_write
- description: ''
  flows:
  - authorizationCode
  scope: custom_objects_read
- description: ''
  flows:
  - authorizationCode
  scope: custom_field_write
- description: ''
  flows:
  - authorizationCode
  scope: opportunity_write
- description: ''
  flows:
  - authorizationCode
  scope: opportunities_list
- description: ''
  flows:
  - authorizationCode
  scope: opportunity_read
- description: ''
  flows:
  - authorizationCode
  scope: tasks_create
- description: ''
  flows:
  - authorizationCode
  scope: tasks_list
- description: ''
  flows:
  - authorizationCode
  scope: email_account_purchase_list
- description: ''
  flows:
  - authorizationCode
  scope: email_account_purchase_create
- description: ''
  flows:
  - authorizationCode
  scope: domain_purchase_list
- description: ''
  flows:
  - authorizationCode
  scope: domain_purchase_create
- description: ''
  flows:
  - authorizationCode
  scope: domain_authentication_status
- description: ''
  flows:
  - authorizationCode
  scope: account_bulk_create
- description: ''
  flows:
  - authorizationCode
  scope: contacts_bulk_create
- description: ''
  flows:
  - authorizationCode
  scope: api_usage_stats_read
- description: ''
  flows:
  - authorizationCode
  scope: credit_usage_stats_read
- description: ''
  flows:
  - authorizationCode
  scope: users_list
- description: ''
  flows:
  - authorizationCode
  scope: custom_fields_list
- description: ''
  flows:
  - authorizationCode
  scope: conversation_intelligence_search
- description: ''
  flows:
  - authorizationCode
  scope: conversation_intelligence_show
- description: ''
  flows:
  - authorizationCode
  scope: tags_list
- description: ''
  flows:
  - authorizationCode
  scope: lists_create
- description: ''
  flows:
  - authorizationCode
  scope: lists_update
- description: ''
  flows:
  - authorizationCode
  scope: lists_add_entities
- description: ''
  flows:
  - authorizationCode
  scope: lists_remove_entities
- description: ''
  flows:
  - authorizationCode
  scope: website_visitor_domain_tracker_read
- description: ''
  flows:
  - authorizationCode
  scope: website_visitor_domain_tracker_update
- description: ''
  flows:
  - authorizationCode
  scope: website_visitor_domain_tracker_send_install_email
- description: ''
  flows:
  - authorizationCode
  scope: website_visitor_domain_tracker_install_script
- description: ''
  flows:
  - authorizationCode
  scope: website_visitors_read
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaign_read
- description: ''
  flows:
  - authorizationCode
  scope: account_owners_update
- description: ''
  flows:
  - authorizationCode
  scope: account_read
- description: ''
  flows:
  - authorizationCode
  scope: account_stages_list
- description: ''
  flows:
  - authorizationCode
  scope: account_stages_update
- description: ''
  flows:
  - authorizationCode
  scope: accounts_search
- description: ''
  flows:
  - authorizationCode
  scope: contact_owners_update
- description: ''
  flows:
  - authorizationCode
  scope: contact_stages_list
- description: ''
  flows:
  - authorizationCode
  scope: contact_stages_update
- description: ''
  flows:
  - authorizationCode
  scope: contacts_bulk_update
- description: ''
  flows:
  - authorizationCode
  scope: conversations_export
- description: ''
  flows:
  - authorizationCode
  scope: conversations_find_export
- description: ''
  flows:
  - authorizationCode
  scope: conversations_search
- description: ''
  flows:
  - authorizationCode
  scope: conversations_show
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_abort
- description: ''
  flows:
  - authorizationCode
  scope: emailer_campaigns_archive
- description: ''
  flows:
  - authorizationCode
  scope: notes_list
- description: ''
  flows:
  - authorizationCode
  scope: opportunity_stages_list
- description: ''
  flows:
  - authorizationCode
  scope: opportunity_update
- description: ''
  flows:
  - authorizationCode
  scope: organization_read
- description: ''
  flows:
  - authorizationCode
  scope: organizations_news_articles
- description: ''
  flows:
  - authorizationCode
  scope: person_read
- description: ''
  flows:
  - authorizationCode
  scope: phone_call_search
- description: ''
  flows:
  - authorizationCode
  scope: phone_call_update
- description: ''
  flows:
  - authorizationCode
  scope: phone_call_write
slug: apollo-io-scopes
source_filename: apollo-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.apollo.io/.well-known/oauth-authorization-server\ndocs: https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners\nnote: Apollo's OpenAPI declares OAuth as an http/bearer scheme, so the scope set is not in the spec's\n  securitySchemes. The authoritative anonymous source is the RFC 8414 authorization-server metadata Apollo\n  serves at mcp.apollo.io, cross-referenced against the per-operation `OAuth scopes:` line published in\n  every endpoint reference page. Partners select scopes at OAuth app registration; read_user_profile and\n  app_scopes are added by Apollo automatically.\nschemes:\n- name: bearerAuth\n  type: oauth2\n  grant_types:\n  - authorization_code\n  - refresh_token\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.apollo.io/#/oauth/authorize\n    tokenUrl: https://app.apollo.io/api/v1/oauth/token\n    docs: https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners\n\
  \  - flow: authorizationCode\n    audience: Apollo MCP (mcp.apollo.io)\n    authorizationUrl: https://mcp.apollo.io/mcp/oauth_metadata/redirect_to_authorize\n    tokenUrl: https://mcp.apollo.io/api/v1/oauth/token\n    registrationUrl: https://mcp.apollo.io/api/v1/oauth/applications/register_oauth_client\n    revocationUrl: https://mcp.apollo.io/api/v1/oauth/revoke\n    pkce:\n    - S256\nscope_count: 91\nscopes:\n- scope: read_user_profile\n  flows:\n  - authorizationCode\n  operations:\n  - get-current-user-profile\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: app_scopes\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: people_bulk_match\n  flows:\n  - authorizationCode\n  operations:\n  - bulk-people-enrichment\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: organizations_bulk_enrich\n  flows:\n  - authorizationCode\n  operations:\n  - bulk-organization-enrichment\n\
  \  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: organizations_enrich\n  flows:\n  - authorizationCode\n  operations:\n  - organization-enrichment\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: people_match\n  flows:\n  - authorizationCode\n  operations:\n  - people-enrichment\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: webhook_result_read\n  flows:\n  - authorizationCode\n  operations:\n  - poll-webhook-result\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: mixed_people_api_search\n  flows:\n  - authorizationCode\n  operations:\n  - people-api-search\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: organizations_job_posting\n  flows:\n  - authorizationCode\n  operations:\n  - organization-jobs-postings\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: mixed_companies_search\n  flows:\n  - authorizationCode\n  operations:\n  - organization-search\n\
  \  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: organizations_search\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: contact_write\n  flows:\n  - authorizationCode\n  operations:\n  - create-a-contact\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: contact_update\n  flows:\n  - authorizationCode\n  operations:\n  - update-a-contact\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: contacts_search\n  flows:\n  - authorizationCode\n  operations:\n  - search-for-contacts\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: contact_read\n  flows:\n  - authorizationCode\n  operations:\n  - view-a-contact\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: account_write\n  flows:\n  - authorizationCode\n  operations:\n  - create-an-account\n  source: well-known/apollo-io-oauth-authorization-server.json\n\
  - scope: account_update\n  flows:\n  - authorizationCode\n  operations:\n  - update-an-account\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: context_center_read\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: context_center_write\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_search\n  flows:\n  - authorizationCode\n  operations:\n  - search-for-sequences\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_create\n  flows:\n  - authorizationCode\n  operations:\n  - create-sequence\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_update\n  flows:\n  - authorizationCode\n  operations:\n  - update-sequence\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_approve\n  flows:\n\
  \  - authorizationCode\n  operations:\n  - approve-sequence\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_add_contact_ids\n  flows:\n  - authorizationCode\n  operations:\n  - add-contacts-to-sequence\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_remove_or_stop_contact_ids\n  flows:\n  - authorizationCode\n  operations:\n  - update-contact-status-sequence\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_schedules_list\n  flows:\n  - authorizationCode\n  operations:\n  - list-email-schedules\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_messages_search\n  flows:\n  - authorizationCode\n  operations:\n  - emailer_messages/search\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_messages_create\n  flows:\n  - authorizationCode\n  operations:\n  - create-an-email-draft\n  source: well-known/apollo-io-oauth-authorization-server.json\n\
  - scope: emailer_messages_send_now\n  flows:\n  - authorizationCode\n  operations:\n  - send-email-now\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_messages_email_send_status\n  flows:\n  - authorizationCode\n  operations:\n  - check-email-send-status\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_messages_get_content\n  flows:\n  - authorizationCode\n  operations:\n  - get-email-content\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaigns_activity_feed\n  flows:\n  - authorizationCode\n  operations:\n  - get-contact-sequence-activity\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: report_sync\n  flows:\n  - authorizationCode\n  operations:\n  - sync-report\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: agent_task\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n\
  - scope: email_accounts_list\n  flows:\n  - authorizationCode\n  operations:\n  - get-a-list-of-email-accounts\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: custom_objects_write\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: custom_objects_read\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: custom_field_write\n  flows:\n  - authorizationCode\n  operations:\n  - create-a-custom-field\n  - update-a-custom-field\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: opportunity_write\n  flows:\n  - authorizationCode\n  operations:\n  - create-deal\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: opportunities_list\n  flows:\n  - authorizationCode\n  operations:\n  - view-associated-deals\n  - list-all-deals\n  source: well-known/apollo-io-oauth-authorization-server.json\n\
  - scope: opportunity_read\n  flows:\n  - authorizationCode\n  operations:\n  - view-deal\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: tasks_create\n  flows:\n  - authorizationCode\n  operations:\n  - create-a-task\n  - bulk-create-tasks\n  - update-a-task\n  - complete-a-task\n  - skip-a-task\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: tasks_list\n  flows:\n  - authorizationCode\n  operations:\n  - get-a-task\n  - search-tasks\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: email_account_purchase_list\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: email_account_purchase_create\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: domain_purchase_list\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n\
  - scope: domain_purchase_create\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: domain_authentication_status\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: account_bulk_create\n  flows:\n  - authorizationCode\n  operations:\n  - bulk-create-accounts\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: contacts_bulk_create\n  flows:\n  - authorizationCode\n  operations:\n  - bulk-create-contacts\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: api_usage_stats_read\n  flows:\n  - authorizationCode\n  operations:\n  - post_apiusage\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: credit_usage_stats_read\n  flows:\n  - authorizationCode\n  operations:\n  - view-credit-usage-stats\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: users_list\n  flows:\n\
  \  - authorizationCode\n  operations:\n  - get-a-list-of-users\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: custom_fields_list\n  flows:\n  - authorizationCode\n  operations:\n  - get-a-list-of-fields\n  - get-a-list-of-all-custom-fields\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: conversation_intelligence_search\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: conversation_intelligence_show\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: tags_list\n  flows:\n  - authorizationCode\n  operations:\n  - get-a-list-of-all-lists\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: lists_create\n  flows:\n  - authorizationCode\n  operations:\n  - create-a-list\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: lists_update\n  flows:\n  - authorizationCode\n\
  \  operations:\n  - update-a-list\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: lists_add_entities\n  flows:\n  - authorizationCode\n  operations:\n  - add-records-to-a-list\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: lists_remove_entities\n  flows:\n  - authorizationCode\n  operations:\n  - remove-records-from-a-list\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: website_visitor_domain_tracker_read\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: website_visitor_domain_tracker_update\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: website_visitor_domain_tracker_send_install_email\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: website_visitor_domain_tracker_install_script\n \
  \ flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: website_visitors_read\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: emailer_campaign_read\n  flows:\n  - authorizationCode\n  operations: []\n  source: well-known/apollo-io-oauth-authorization-server.json\n- scope: account_owners_update\n  flows:\n  - authorizationCode\n  operations:\n  - update-account-ownership\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: account_read\n  flows:\n  - authorizationCode\n  operations:\n  - get_accounts{id}\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server\
  \ scopes_supported\n    set.\n- scope: account_stages_list\n  flows:\n  - authorizationCode\n  operations:\n  - list-account-stages\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: account_stages_update\n  flows:\n  - authorizationCode\n  operations:\n  - bulk-update-accounts\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: accounts_search\n  flows:\n  - authorizationCode\n  operations:\n  - search-for-accounts\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: contact_owners_update\n\
  \  flows:\n  - authorizationCode\n  operations:\n  - update-contact-ownership\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: contact_stages_list\n  flows:\n  - authorizationCode\n  operations:\n  - list-contact-stages\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: contact_stages_update\n  flows:\n  - authorizationCode\n  operations:\n  - update-contact-stage\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: contacts_bulk_update\n  flows:\n  - authorizationCode\n  operations:\n\
  \  - bulk-update-contacts\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: conversations_export\n  flows:\n  - authorizationCode\n  operations:\n  - export-conversations\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: conversations_find_export\n  flows:\n  - authorizationCode\n  operations:\n  - get-conversations-export\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: conversations_search\n  flows:\n  - authorizationCode\n  operations:\n  - search-conversations\n  source:\
  \ openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: conversations_show\n  flows:\n  - authorizationCode\n  operations:\n  - get-conversations-info\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: emailer_campaigns_abort\n  flows:\n  - authorizationCode\n  operations:\n  - abort-sequence\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: emailer_campaigns_archive\n  flows:\n  - authorizationCode\n  operations:\n  - archive-sequence\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json\
  \ (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: notes_list\n  flows:\n  - authorizationCode\n  operations:\n  - get-a-list-of-notes\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: opportunity_stages_list\n  flows:\n  - authorizationCode\n  operations:\n  - list-deal-stages\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: opportunity_update\n  flows:\n  - authorizationCode\n  operations:\n  - update-deal\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the\
  \ API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: organization_read\n  flows:\n  - authorizationCode\n  operations:\n  - get_organizations{id}\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: organizations_news_articles\n  flows:\n  - authorizationCode\n  operations:\n  - news_articles_search\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: person_read\n  flows:\n  - authorizationCode\n  operations:\n  - get_people{id}\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server\
  \ scopes_supported\n    set.\n- scope: phone_call_search\n  flows:\n  - authorizationCode\n  operations:\n  - get_phone_callssearch\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: phone_call_update\n  flows:\n  - authorizationCode\n  operations:\n  - put_phone_callsupdate\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n- scope: phone_call_write\n  flows:\n  - authorizationCode\n  operations:\n  - phonecalls_create\n  source: openapi/_original/apollo-io-apollo-rest-api-openapi.json (endpoint reference)\n  note: Documented per-operation in the API reference; not listed in the MCP authorization-server scopes_supported\n    set.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/scopes/apollo-io-scopes.yml
summary_line: 91 scopes · authorizationCode
tags:
- Sales Intelligence
- Prospecting
- Engagement
- B2B Data
- Enrichment
- CRM
- Sales Engagement
- Conversation Intelligence
- MCP
- Software-as-a-Service
token_urls:
- https://app.apollo.io/api/v1/oauth/token
- https://mcp.apollo.io/api/v1/oauth/token
---
