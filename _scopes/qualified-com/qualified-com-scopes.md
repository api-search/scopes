---
api_specs:
- filename: qualified-com-enterprise-api-openapi.json
  format: json
  label: Qualified Enterprise API
  slug: qualified-com-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-enterprise-api-openapi.json
authorization_urls: []
description: ''
docs: https://app.qualified.com/docs/api
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Qualified Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Qualified uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qualified
provider_slug: qualified-com
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: qualified-com-scopes
source_filename: qualified-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://app.qualified.com/docs/api\ndocs: https://app.qualified.com/docs/api\napi: qualified-com-enterprise-api\nmodel: >-\n  Qualified does not run an OAuth 2.0 authorization-code flow for the Enterprise API.\n  API keys are minted inside the Qualified app with an explicit, named set of\n  OAuth-style scopes, and the key is then presented as a bearer token. The OpenAPI\n  declares only `bearerToken` (http/bearer), so the scope vocabulary below is read\n  from the published reference rather than from `securitySchemes` — recorded here so\n  the permission surface is machine-readable even though the spec does not model it.\nenforcement:\n  insufficient_scope_status: 403\n  insufficient_scope_body: '{\"code\": \"insufficient_scope\"}'\n  convention: >-\n    Read endpoints require a :view scope; write endpoints require a :manage scope.\n    Granting :manage also grants the matching :view.\nscope_count: 9\nscopes:\n- name: lead:view\n\
  \  description: Read leads.\n  operations: [listLeads, getLead]\n- name: lead:manage\n  description: Create and update leads. Implies lead:view.\n  operations: [upsertLead]\n- name: company:manage\n  description: Create and update companies. Companies cannot be read back.\n  operations: [upsertCompany]\n- name: session:view\n  description: Read website sessions.\n  operations: [listSessions, getSession]\n- name: conversation:view\n  description: Read conversations and messages. Covers both message endpoints.\n  operations: [listConversations, getConversation, listConversationMessages, listMessages, getMessage]\n- name: meeting:view\n  description: Read meetings.\n  operations: [listMeetings, getMeeting]\n- name: meeting:manage\n  description: Cancel meetings. Implies meeting:view.\n  operations: [cancelMeeting]\n- name: email:view\n  description: Read outbound email activity.\n  operations: [listEmails, getEmail]\n- name: bulk_job:manage\n  description: Submit bulk jobs and read their\
  \ status. Covers both /v2/bulk endpoints.\n  operations: [createBulkJob, getBulkJob]\n- name: gdpr:manage\n  description: Submit GDPR deletion requests.\n  operations: [createGdprDeletionRequest]\n- name: legacy:view\n  description: Read the legacy /v1 bot and rep reporting endpoints.\n  operations: [listBotConversations, listRepConversations]\nunscoped_operations:\n- operationId: listLeadFields\n  note: GET /v2/leads/fields requires only a valid token, no scope.\n- operationId: listCompanyFields\n  note: GET /v2/companies/fields requires only a valid token, no scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/scopes/qualified-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Conversational Marketing
- Sales
- Marketing
- Artificial Intelligence
- AI Agents
- Lead Generation
- Customer Engagement
- Salesforce
- Analytics
token_urls: []
---
