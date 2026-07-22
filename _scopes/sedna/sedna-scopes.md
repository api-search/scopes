---
api_specs:
- filename: sedna-openapi.json
  format: json
  label: Sedna API
  slug: sedna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Sedna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SEDNA publishes 53 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SEDNA API on a user''s behalf.


  Tokens are issued from https://{tenant}.sednanetwork.com/platform/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SEDNA
provider_slug: sedna
schemes:
- description: This API prefers OAuth 2 with client credentials flow. You can create your credentials in the <a href='https://{tenant}.sednanetwork.com/platform/settings/api-credential-management'>Api Credential Management page</a>.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{tenant}.sednanetwork.com/platform/oauth/token
  name: OAuth
  source: openapi/sedna-openapi.json
scope_count: 53
scope_names:
- CATEGORYTAG_DELETE
- CATEGORYTAG_READ
- CATEGORYTAG_WRITE
- CHARTERING_DELETE
- CHARTERING_READ
- CHARTERING_WRITE
- COMMENT_READ
- COMPANY_READ
- COMPANY_WRITE
- CONTACTGROUP_DELETE
- CONTACTGROUP_READ
- CONTACTGROUP_WRITE
- CONTACT_DELETE
- CONTACT_READ
- CONTACT_WRITE
- CRMENTITY_DELETE
- CRMENTITY_READ
- CRMENTITY_WRITE
- DOCUMENT_READ
- EVENT_READ
- JOBREFERENCE_DELETE
- JOBREFERENCE_READ
- JOBREFERENCE_WRITE
- KEYWORD_DELETE
- KEYWORD_READ
- KEYWORD_WRITE
- LEGAL_HOLD_DELETE
- LEGAL_HOLD_READ
- LEGAL_HOLD_WRITE
- MESSAGE_DELETE
- MESSAGE_READ
- MESSAGE_RETENTION_SETTINGS_READ
- MESSAGE_RETENTION_SETTINGS_WRITE
- MESSAGE_WRITE
- PERSONAL_DATA_UNREDACTED_READ
- QUARANTINED_MESSAGE_READ
- QUARANTINED_MESSAGE_WRITE
- RETENTION_POLICY_DELETE
- RETENTION_POLICY_READ
- RETENTION_POLICY_WRITE
- SAVEDSEARCH_DELETE
- SAVEDSEARCH_READ
- SAVEDSEARCH_WRITE
- TEAM_DELETE
- TEAM_READ
- TEAM_WRITE
- TEMPLATE_READ
- USER_DELETE
- USER_READ
- USER_WRITE
- WORKFLOW_DELETE
- WORKFLOW_READ
- WORKFLOW_WRITE
scopes:
- description: Delete category tags
  flows:
  - clientCredentials
  scope: CATEGORYTAG_DELETE
- description: Read category tags
  flows:
  - clientCredentials
  scope: CATEGORYTAG_READ
- description: Create and update category tags
  flows:
  - clientCredentials
  scope: CATEGORYTAG_WRITE
- description: Delete chartering (Pulse) information
  flows:
  - clientCredentials
  scope: CHARTERING_DELETE
- description: Read chartering (Pulse) information
  flows:
  - clientCredentials
  scope: CHARTERING_READ
- description: Create chartering (Pulse) information
  flows:
  - clientCredentials
  scope: CHARTERING_WRITE
- description: Read message comments
  flows:
  - clientCredentials
  scope: COMMENT_READ
- description: Read company info
  flows:
  - clientCredentials
  scope: COMPANY_READ
- description: Update company info (eg. signature)
  flows:
  - clientCredentials
  scope: COMPANY_WRITE
- description: Delete contact groups
  flows:
  - clientCredentials
  scope: CONTACTGROUP_DELETE
- description: Read contact groups
  flows:
  - clientCredentials
  scope: CONTACTGROUP_READ
- description: Create and update contact groups
  flows:
  - clientCredentials
  scope: CONTACTGROUP_WRITE
- description: Delete contacts
  flows:
  - clientCredentials
  scope: CONTACT_DELETE
- description: Read contacts
  flows:
  - clientCredentials
  scope: CONTACT_READ
- description: Create and update contacts
  flows:
  - clientCredentials
  scope: CONTACT_WRITE
- description: Delete CRM contacts
  flows:
  - clientCredentials
  scope: CRMENTITY_DELETE
- description: Read CRM contacts
  flows:
  - clientCredentials
  scope: CRMENTITY_READ
- description: Create and update CRM Contacts
  flows:
  - clientCredentials
  scope: CRMENTITY_WRITE
- description: Read and download attachments
  flows:
  - clientCredentials
  scope: DOCUMENT_READ
- description: Read events from the events endpoint
  flows:
  - clientCredentials
  scope: EVENT_READ
- description: Delete job references
  flows:
  - clientCredentials
  scope: JOBREFERENCE_DELETE
- description: Read job references
  flows:
  - clientCredentials
  scope: JOBREFERENCE_READ
- description: Create and update job references
  flows:
  - clientCredentials
  scope: JOBREFERENCE_WRITE
- description: Delete custom keywords
  flows:
  - clientCredentials
  scope: KEYWORD_DELETE
- description: Read custom keywords
  flows:
  - clientCredentials
  scope: KEYWORD_READ
- description: Create and update custom keywords
  flows:
  - clientCredentials
  scope: KEYWORD_WRITE
- description: Delete legal holds
  flows:
  - clientCredentials
  scope: LEGAL_HOLD_DELETE
- description: Read legal holds
  flows:
  - clientCredentials
  scope: LEGAL_HOLD_READ
- description: Create and update legal holds
  flows:
  - clientCredentials
  scope: LEGAL_HOLD_WRITE
- description: Archive email messages
  flows:
  - clientCredentials
  scope: MESSAGE_DELETE
- description: Read (draft) email messages
  flows:
  - clientCredentials
  scope: MESSAGE_READ
- description: Read message retention settings
  flows:
  - clientCredentials
  scope: MESSAGE_RETENTION_SETTINGS_READ
- description: Update message retention settings
  flows:
  - clientCredentials
  scope: MESSAGE_RETENTION_SETTINGS_WRITE
- description: Create and send (draft) email messages
  flows:
  - clientCredentials
  scope: MESSAGE_WRITE
- description: Read unredacted emails with personal data
  flows:
  - clientCredentials
  scope: PERSONAL_DATA_UNREDACTED_READ
- description: Read quarantined email messages
  flows:
  - clientCredentials
  scope: QUARANTINED_MESSAGE_READ
- description: Release quarantined email messages
  flows:
  - clientCredentials
  scope: QUARANTINED_MESSAGE_WRITE
- description: Delete retention policies
  flows:
  - clientCredentials
  scope: RETENTION_POLICY_DELETE
- description: Read retention policies
  flows:
  - clientCredentials
  scope: RETENTION_POLICY_READ
- description: Create and update retention policies
  flows:
  - clientCredentials
  scope: RETENTION_POLICY_WRITE
- description: Remove saved searches
  flows:
  - clientCredentials
  scope: SAVEDSEARCH_DELETE
- description: Read saved search details
  flows:
  - clientCredentials
  scope: SAVEDSEARCH_READ
- description: Create and update saved searches
  flows:
  - clientCredentials
  scope: SAVEDSEARCH_WRITE
- description: Delete teams
  flows:
  - clientCredentials
  scope: TEAM_DELETE
- description: Read team details
  flows:
  - clientCredentials
  scope: TEAM_READ
- description: Create and update teams
  flows:
  - clientCredentials
  scope: TEAM_WRITE
- description: Read templates
  flows:
  - clientCredentials
  scope: TEMPLATE_READ
- description: Archive users
  flows:
  - clientCredentials
  scope: USER_DELETE
- description: Read user details
  flows:
  - clientCredentials
  scope: USER_READ
- description: Create and update users
  flows:
  - clientCredentials
  scope: USER_WRITE
- description: Delete workflows
  flows:
  - clientCredentials
  scope: WORKFLOW_DELETE
- description: Read workflow details
  flows:
  - clientCredentials
  scope: WORKFLOW_READ
- description: Create and update workflows
  flows:
  - clientCredentials
  scope: WORKFLOW_WRITE
slug: sedna-scopes
source_filename: sedna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sedna-openapi.json\nschemes:\n- name: OAuth\n  source: openapi/sedna-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.sednanetwork.com/platform/oauth/token\n  description: This API prefers OAuth 2 with client credentials flow. You can create your credentials\n    in the <a href='https://{tenant}.sednanetwork.com/platform/settings/api-credential-management'>Api\n    Credential Management page</a>.\nscopes:\n- scope: CATEGORYTAG_DELETE\n  description: Delete category tags\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CATEGORYTAG_READ\n  description: Read category tags\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CATEGORYTAG_WRITE\n  description: Create and update category tags\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CHARTERING_DELETE\n  description: Delete\
  \ chartering (Pulse) information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CHARTERING_READ\n  description: Read chartering (Pulse) information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CHARTERING_WRITE\n  description: Create chartering (Pulse) information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: COMMENT_READ\n  description: Read message comments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: COMPANY_READ\n  description: Read company info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: COMPANY_WRITE\n  description: Update company info (eg. signature)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CONTACTGROUP_DELETE\n  description: Delete contact groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope:\
  \ CONTACTGROUP_READ\n  description: Read contact groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CONTACTGROUP_WRITE\n  description: Create and update contact groups\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CONTACT_DELETE\n  description: Delete contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CONTACT_READ\n  description: Read contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CONTACT_WRITE\n  description: Create and update contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CRMENTITY_DELETE\n  description: Delete CRM contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CRMENTITY_READ\n  description: Read CRM contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: CRMENTITY_WRITE\n\
  \  description: Create and update CRM Contacts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: DOCUMENT_READ\n  description: Read and download attachments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: EVENT_READ\n  description: Read events from the events endpoint\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: JOBREFERENCE_DELETE\n  description: Delete job references\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: JOBREFERENCE_READ\n  description: Read job references\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: JOBREFERENCE_WRITE\n  description: Create and update job references\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: KEYWORD_DELETE\n  description: Delete custom keywords\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n\
  - scope: KEYWORD_READ\n  description: Read custom keywords\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: KEYWORD_WRITE\n  description: Create and update custom keywords\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: LEGAL_HOLD_DELETE\n  description: Delete legal holds\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: LEGAL_HOLD_READ\n  description: Read legal holds\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: LEGAL_HOLD_WRITE\n  description: Create and update legal holds\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: MESSAGE_DELETE\n  description: Archive email messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: MESSAGE_READ\n  description: Read (draft) email messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n\
  - scope: MESSAGE_RETENTION_SETTINGS_READ\n  description: Read message retention settings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: MESSAGE_RETENTION_SETTINGS_WRITE\n  description: Update message retention settings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: MESSAGE_WRITE\n  description: Create and send (draft) email messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: PERSONAL_DATA_UNREDACTED_READ\n  description: Read unredacted emails with personal data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: QUARANTINED_MESSAGE_READ\n  description: Read quarantined email messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: QUARANTINED_MESSAGE_WRITE\n  description: Release quarantined email messages\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope:\
  \ RETENTION_POLICY_DELETE\n  description: Delete retention policies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: RETENTION_POLICY_READ\n  description: Read retention policies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: RETENTION_POLICY_WRITE\n  description: Create and update retention policies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: SAVEDSEARCH_DELETE\n  description: Remove saved searches\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: SAVEDSEARCH_READ\n  description: Read saved search details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: SAVEDSEARCH_WRITE\n  description: Create and update saved searches\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: TEAM_DELETE\n  description: Delete teams\n  flows:\n  - clientCredentials\n  sources:\n \
  \ - openapi/sedna-openapi.json\n- scope: TEAM_READ\n  description: Read team details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: TEAM_WRITE\n  description: Create and update teams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: TEMPLATE_READ\n  description: Read templates\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: USER_DELETE\n  description: Archive users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: USER_READ\n  description: Read user details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: USER_WRITE\n  description: Create and update users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: WORKFLOW_DELETE\n  description: Delete workflows\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: WORKFLOW_READ\n  description:\
  \ Read workflow details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n- scope: WORKFLOW_WRITE\n  description: Create and update workflows\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sedna-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/scopes/sedna-scopes.yml
summary_line: 53 scopes · clientCredentials
tags:
- Company
- Shipping
- Maritime
- Email
- Communications
- Workflow
- Commodity Trading
- Logistics
- Messaging
token_urls:
- https://{tenant}.sednanetwork.com/platform/oauth/token
---
