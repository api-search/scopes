---
authorization_urls:
- https://{hostname}/ewws/oauth
description: ''
docs: https://help.agiloft.com/space/HELP/43714795/Control%20Access%20to%20REST%20API%20Operations
flows:
- authorizationCode
- authorizationCodePKCE
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Agiloft Scopes
name_suffix: OAuth Scopes
note: Agiloft's scope model has two distinct halves and neither is a conventional OAuth scope string namespace. (1) The OAuth 2.0 authorization request carries exactly one scope value of the form permissions_for:{CONTACT_ID}, naming the Agiloft contact record whose permissions the token will carry — the permission set itself lives on that user, not in the scope string. (2) A separate Scope parameter, configured at Setup > Integration > Access Token API > Configure, restricts which REST operations a given access token may invoke. A blank Scope parameter grants every operation, which the docs flag as a hazard. Both are documented publicly; no scope catalogue was derived from a spec because Agiloft's OpenAPI is generated per knowledgebase behind KB login.
overview: 'Agiloft publishes 1 OAuth 2.0 scope via the authorizationCode, authorizationCodePKCE, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agiloft API on a user''s behalf.


  Tokens are issued from https://{hostname}/ewws/otoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agiloft
provider_slug: agiloft
schemes:
- flows:
  - authorizationUrl: https://{hostname}/ewws/oauth
    flow: authorizationCode
    tokenUrl: https://{hostname}/ewws/otoken
  - authorizationUrl: https://{hostname}/ewws/oauth
    flow: authorizationCodePKCE
    tokenUrl: https://{hostname}/ewws/otoken
  - flow: clientCredentials
    tokenUrl: https://{hostname}/ewws/otoken
  name: OAuth2
  source: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API
scope_count: 1
scope_names:
- permissions_for:{CONTACT_ID}
scopes:
- description: The only OAuth scope value Agiloft accepts. CONTACT_ID is the numeric id of the Agiloft contact record configured in the API application's "Associate this Application with Contact ID" field — for example permissions_for:222. The token then carries that user's group permissions.
  flows:
  - authorizationCode
  - authorizationCodePKCE
  scope: permissions_for:{CONTACT_ID}
slug: agiloft-scopes
source_filename: agiloft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://help.agiloft.com/space/HELP/43714795/Control%20Access%20to%20REST%20API%20Operations\ndocs: https://help.agiloft.com/space/HELP/43714795/Control%20Access%20to%20REST%20API%20Operations\nnote: >-\n  Agiloft's scope model has two distinct halves and neither is a conventional OAuth scope string\n  namespace. (1) The OAuth 2.0 authorization request carries exactly one scope value of the form\n  permissions_for:{CONTACT_ID}, naming the Agiloft contact record whose permissions the token will\n  carry — the permission set itself lives on that user, not in the scope string. (2) A separate\n  Scope parameter, configured at Setup > Integration > Access Token API > Configure, restricts\n  which REST operations a given access token may invoke. A blank Scope parameter grants every\n  operation, which the docs flag as a hazard. Both are documented publicly; no scope catalogue was\n  derived from a spec because Agiloft's OpenAPI is\
  \ generated per knowledgebase behind KB login.\nschemes:\n- name: OAuth2\n  source: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{hostname}/ewws/oauth\n    tokenUrl: https://{hostname}/ewws/otoken\n  - flow: authorizationCodePKCE\n    authorizationUrl: https://{hostname}/ewws/oauth\n    tokenUrl: https://{hostname}/ewws/otoken\n  - flow: clientCredentials\n    tokenUrl: https://{hostname}/ewws/otoken\nscopes:\n- scope: 'permissions_for:{CONTACT_ID}'\n  description: >-\n    The only OAuth scope value Agiloft accepts. CONTACT_ID is the numeric id of the Agiloft contact\n    record configured in the API application's \"Associate this Application with Contact ID\" field —\n    for example permissions_for:222. The token then carries that user's group permissions.\n  flows: [authorizationCode, authorizationCodePKCE]\n  required: true\n  sources: [https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API]\n\
  operation_scopes:\n  parameter: Scope\n  configured_at: Setup > Integration > Access Token API > Configure > Advanced configuration\n  default_when_blank: all operations granted\n  applies_to: REST access tokens\n  supports_per_user_lists: true\n  supports_default_list: true\n  operations:\n  - {operation: EWCreate, description: Create a record in a table}\n  - {operation: EWRead, description: Read a record by id}\n  - {operation: EWUpdate, description: Update fields on an existing record}\n  - {operation: EWDelete, description: Delete one or more records}\n  - {operation: REST, description: 'The /ewws/REST/{kbName}/{table}[/{id}] resource-style interface'}\n  - {operation: EWBroadcast, description: Broadcast operation}\n  - {operation: EWSelect, description: Limited SQL-style select returning record identifiers}\n  - {operation: EWSearch, description: Saved-search and ad hoc query search}\n  - {operation: EWGetChoiceLineID, description: Resolve the internal id of a choice value}\n  -\
  \ {operation: EWHotlinks, description: Create a secure hotlink for third-party portal integration}\n  - {operation: EWAttach, description: Attach a file to a record}\n  - {operation: EWRetrieve, description: Retrieve an attachment}\n  - {operation: EWRemoveAttachment, description: Remove an attachment from a record}\n  - {operation: EWOData, description: OData operation named in the scope list; no public OData reference is published}\n  - {operation: EWTable, description: List every table and field in the system}\n  - {operation: EWSavedSearch, description: Return details about a saved search defined in a table}\n  - {operation: EWAttachInfo, description: Return attachment metadata for a record}\n  - {operation: webhooks, description: Register, read, update and delete webhook subscriptions}\n  - {operation: EWActionButton, description: Run an action button from a specified record}\n  - {operation: EWAsyncStatus, description: Check the execution status of an asynchronous call}\n  note:\
  \ >-\n    EWUpsert is documented as a REST operation but does not appear in the published Available\n    Operations list for the Scope parameter; do not assume it can be scoped independently.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agiloft/refs/heads/main/scopes/agiloft-scopes.yml
summary_line: 1 scope · authorizationCode/authorizationCodePKCE/clientCredentials
tags:
- Contract Lifecycle Management
- Contract Management
- Legal
- Procurement
- Enterprise Software
- No-Code
- Workflow Automation
- Document Automation
- Webhook
- SCIM
- Company
token_urls:
- https://{hostname}/ewws/otoken
---
