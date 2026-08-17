---
api_specs:
- filename: apollo-api-documentation-accounts-api-openapi.yml
  format: yaml
  label: Apollo API Accounts
  slug: apollo-api-documentation-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-accounts-api-openapi.yml
- filename: apollo-api-documentation-analytics-api-openapi.yml
  format: yaml
  label: Apollo API Analytics
  slug: apollo-api-documentation-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-analytics-api-openapi.yml
- filename: apollo-api-documentation-calls-api-openapi.yml
  format: yaml
  label: Apollo API Calls
  slug: apollo-api-documentation-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-calls-api-openapi.yml
- filename: apollo-api-documentation-contacts-api-openapi.yml
  format: yaml
  label: Apollo API Contacts
  slug: apollo-api-documentation-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-contacts-api-openapi.yml
- filename: apollo-api-documentation-conversations-api-openapi.yml
  format: yaml
  label: Apollo API Conversations
  slug: apollo-api-documentation-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-conversations-api-openapi.yml
- filename: apollo-api-documentation-deals-api-openapi.yml
  format: yaml
  label: Apollo API Deals
  slug: apollo-api-documentation-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-deals-api-openapi.yml
- filename: apollo-api-documentation-emailer-messages-api-openapi.yml
  format: yaml
  label: Apollo API Emailer Messages
  slug: apollo-api-documentation-emailer-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-emailer-messages-api-openapi.yml
- filename: apollo-api-documentation-enrichment-api-openapi.yml
  format: yaml
  label: Apollo API Enrichment
  slug: apollo-api-documentation-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-enrichment-api-openapi.yml
- filename: apollo-api-documentation-fields-api-openapi.yml
  format: yaml
  label: Apollo API Fields
  slug: apollo-api-documentation-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-fields-api-openapi.yml
- filename: apollo-api-documentation-miscellaneous-api-openapi.yml
  format: yaml
  label: Apollo API Miscellaneous
  slug: apollo-api-documentation-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-miscellaneous-api-openapi.yml
- filename: apollo-api-documentation-search-api-openapi.yml
  format: yaml
  label: Apollo API Search
  slug: apollo-api-documentation-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-search-api-openapi.yml
- filename: apollo-api-documentation-sequences-api-openapi.yml
  format: yaml
  label: Apollo API Sequences
  slug: apollo-api-documentation-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-sequences-api-openapi.yml
- filename: apollo-api-documentation-tasks-api-openapi.yml
  format: yaml
  label: Apollo API Tasks
  slug: apollo-api-documentation-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/openapi/apollo-api-documentation-tasks-api-openapi.yml
authorization_urls: []
description: Apollo's OAuth 2.0 scope vocabulary, read verbatim from the RFC 8414 authorization-server metadata Apollo serves anonymously at https://mcp.apollo.io/.well-known/oauth-authorization-server (HTTP 200, 2026-08-14). The identical list is served at /.well-known/oauth-protected-resource and /.well-known/openid-configuration. Scopes are per-endpoint capability grants, not read/write tiers — a partner app requests exactly the endpoints it calls. Apollo adds read_user_profile and app_scopes by default to every registered app. Note the REST OpenAPI declares OAuth as a plain `http bearer` securityScheme with no flows block, so these scopes are NOT derivable from the spec; this artifact is the only machine-readable record of them.
docs: https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Apollo Api Documentation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Apollo API Documentation uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apollo API Documentation
provider_slug: apollo-api-documentation
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: apollo-api-documentation-scopes
source_filename: apollo-api-documentation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.apollo.io/.well-known/oauth-authorization-server\ndocs: https://docs.apollo.io/docs/use-oauth-20-authorization-flow-to-access-apollo-user-information-partners\nprovider: Apollo API Documentation\nproviderId: apollo-api-documentation\ndescription: >-\n  Apollo's OAuth 2.0 scope vocabulary, read verbatim from the RFC 8414 authorization-server metadata Apollo\n  serves anonymously at https://mcp.apollo.io/.well-known/oauth-authorization-server (HTTP 200, 2026-08-14).\n  The identical list is served at /.well-known/oauth-protected-resource and /.well-known/openid-configuration.\n  Scopes are per-endpoint capability grants, not read/write tiers — a partner app requests exactly the\n  endpoints it calls. Apollo adds read_user_profile and app_scopes by default to every registered app.\n  Note the REST OpenAPI declares OAuth as a plain `http bearer` securityScheme with no flows block, so these\n  scopes are NOT derivable\
  \ from the spec; this artifact is the only machine-readable record of them.\nauthorization_server:\n  issuer: https://mcp.apollo.io\n  authorization_endpoint: https://mcp.apollo.io/mcp/oauth_metadata/redirect_to_authorize\n  user_facing_authorize_url: https://app.apollo.io/#/oauth/authorize\n  token_endpoint: https://mcp.apollo.io/api/v1/oauth/token\n  revocation_endpoint: https://mcp.apollo.io/api/v1/oauth/revoke\n  registration_endpoint: https://mcp.apollo.io/api/v1/oauth/applications/register_oauth_client\n  jwks_uri: https://mcp.apollo.io/mcp/oauth_metadata/jwks\n  grant_types: [authorization_code, refresh_token, client_credentials]\n  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  scope_delimiter: space\nscope_count: 67\nscopes:\n  - {name: read_user_profile, description: Basic user info. Added by Apollo to every app by default., default: true}\n  - {name: app_scopes, description: Umbrella\
  \ grant covering all scopes selected during app registration., default: true}\n  - {name: people_match, description: People enrichment., operation: people-enrichment}\n  - {name: people_bulk_match, description: Bulk people enrichment., operation: bulk-people-enrichment}\n  - {name: organizations_enrich, description: Organization enrichment., operation: organization-enrichment}\n  - {name: organizations_bulk_enrich, description: Bulk organization enrichment., operation: bulk-organization-enrichment}\n  - {name: organizations_job_posting, description: Organization job postings., operation: organization-jobs-postings}\n  - {name: mixed_people_api_search, description: People API search., operation: people-api-search}\n  - {name: mixed_companies_search, description: Organization search., operation: organization-search}\n  - {name: organizations_search, description: Organization search (alternate grant).}\n  - {name: webhook_result_read, description: Poll asynchronous webhook results., operation:\
  \ poll-webhook-result}\n  - {name: contact_read, description: Read a saved contact., operation: view-a-contact}\n  - {name: contact_write, description: Create contacts., operation: create-a-contact}\n  - {name: contact_update, description: Update contacts., operation: update-a-contact}\n  - {name: contacts_search, description: Search saved contacts., operation: search-for-contacts}\n  - {name: contacts_bulk_create, description: Bulk create contacts., operation: bulk-create-contacts}\n  - {name: account_write, description: Create accounts., operation: create-an-account}\n  - {name: account_update, description: Update accounts., operation: update-an-account}\n  - {name: account_bulk_create, description: Bulk create accounts., operation: bulk-create-accounts}\n  - {name: opportunity_read, description: Read a deal., operation: view-deal}\n  - {name: opportunity_write, description: Create or update a deal., operation: create-deal}\n  - {name: opportunities_list, description: List deals., operation:\
  \ list-all-deals}\n  - {name: emailer_campaign_read, description: Read a sequence.}\n  - {name: emailer_campaigns_search, description: Search sequences., operation: search-for-sequences}\n  - {name: emailer_campaigns_create, description: Create a sequence., operation: create-sequence}\n  - {name: emailer_campaigns_update, description: Update a sequence., operation: update-sequence}\n  - {name: emailer_campaigns_approve, description: Activate a sequence., operation: approve-sequence}\n  - {name: emailer_campaigns_add_contact_ids, description: Add contacts to a sequence., operation: add-contacts-to-sequence}\n  - {name: emailer_campaigns_remove_or_stop_contact_ids, description: Remove or stop contacts in a sequence., operation: update-contact-status-sequence}\n  - {name: emailer_campaigns_activity_feed, description: Contact sequence activity., operation: get-contact-sequence-activity}\n  - {name: emailer_schedules_list, description: List email schedules., operation: list-email-schedules}\n\
  \  - {name: emailer_messages_search, description: Search outreach emails.}\n  - {name: emailer_messages_create, description: Create an email draft., operation: create-an-email-draft}\n  - {name: emailer_messages_send_now, description: Send an email now., operation: send-email-now}\n  - {name: emailer_messages_email_send_status, description: Check email send status., operation: check-email-send-status}\n  - {name: emailer_messages_get_content, description: Get email content., operation: get-email-content}\n  - {name: email_accounts_list, description: List connected mailboxes., operation: get-a-list-of-email-accounts}\n  - {name: email_account_purchase_list, description: Browse purchasable mailboxes for cold email.}\n  - {name: email_account_purchase_create, description: Purchase a mailbox for cold email.}\n  - {name: domain_purchase_list, description: Browse purchasable sending domains.}\n  - {name: domain_purchase_create, description: Purchase a sending domain.}\n  - {name: domain_authentication_status,\
  \ description: Check SPF/DKIM/DMARC status for a sending domain.}\n  - {name: tasks_create, description: Create tasks., operation: create-a-task}\n  - {name: tasks_list, description: Search or list tasks., operation: search-tasks}\n  - {name: report_sync, description: Query the analytics report., operation: sync-report}\n  - {name: agent_task, description: Agent task execution.}\n  - {name: context_center_read, description: Read Context Center data.}\n  - {name: context_center_write, description: Write Context Center data.}\n  - {name: custom_objects_read, description: Read custom object records.}\n  - {name: custom_objects_write, description: Create or update custom objects.}\n  - {name: custom_field_write, description: Create or update a custom field., operation: create-a-custom-field}\n  - {name: custom_fields_list, description: List custom fields., operation: get-a-list-of-all-custom-fields}\n  - {name: api_usage_stats_read, description: View API usage stats and rate limits., operation:\
  \ post_apiusage}\n  - {name: credit_usage_stats_read, description: View credit usage stats., operation: view-credit-usage-stats}\n  - {name: users_list, description: List workspace users., operation: get-a-list-of-users}\n  - {name: conversation_intelligence_search, description: Search conversations., operation: search-conversations}\n  - {name: conversation_intelligence_show, description: Get conversation info., operation: get-conversations-info}\n  - {name: tags_list, description: List tags.}\n  - {name: lists_create, description: Create a list., operation: create-a-list}\n  - {name: lists_update, description: Update a list., operation: update-a-list}\n  - {name: lists_add_entities, description: Add records to a list., operation: add-records-to-a-list}\n  - {name: lists_remove_entities, description: Remove records from a list., operation: remove-records-from-a-list}\n  - {name: website_visitors_read, description: Read website-visitor intent data.}\n  - {name: website_visitor_domain_tracker_read,\
  \ description: Read website visitor domain tracker config.}\n  - {name: website_visitor_domain_tracker_update, description: Update website visitor domain tracker config.}\n  - {name: website_visitor_domain_tracker_send_install_email, description: Email the visitor-tracker install script.}\n  - {name: website_visitor_domain_tracker_install_script, description: Retrieve the visitor-tracker install script.}\nnotes:\n  - >-\n    `operation:` is a derived cross-reference to the operationId in\n    openapi/_original/apollo-api-documentation-apollo-rest-api-openapi.json where the scope name and the\n    endpoint path are the same resource. Scopes with no `operation:` have no matching public REST operation —\n    they grant MCP-only or app-only capability (custom objects, Context Center, website visitors, domain and\n    mailbox purchasing, agent_task).\n  - >-\n    Example authorization URL published by Apollo:\n    https://app.apollo.io/#/oauth/authorize?client_id=<id>&redirect_uri=<uri>&response_type=code&scope=contacts_search%20person_read&state=xxxx\n\
  \  - >-\n    Apollo warns that editing an app's scopes after registration requires repeating the whole authorization\n    flow.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-api-documentation/refs/heads/main/scopes/apollo-api-documentation-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Documentation
- Sales Intelligence
- Data Enrichment
- People Search
- Company Search
- Sales Engagement
- CRM
- MCP
- Agents
- Go-To-Market
token_urls: []
---
