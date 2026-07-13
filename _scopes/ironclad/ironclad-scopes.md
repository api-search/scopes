---
api_specs:
- filename: ironclad-public-api-openapi.yml
  format: yaml
  label: Ironclad Public API
  slug: ironclad-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-public-api-openapi.yml
- filename: ironclad-oauth-20-api-openapi.yml
  format: yaml
  label: Ironclad OAuth 2.0 API
  slug: ironclad-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-oauth-20-api-openapi.yml
- filename: ironclad-scim-api-openapi.yml
  format: yaml
  label: Ironclad SCIM 2.0 API
  slug: ironclad-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-scim-api-openapi.yml
authorization_urls:
- https://na1.ironcladapp.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ironclad Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ironclad publishes 60 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ironclad API on a user''s behalf.


  Tokens are issued from https://na1.ironcladapp.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ironclad
provider_slug: ironclad
schemes:
- flows:
  - authorizationUrl: https://na1.ironcladapp.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://na1.ironcladapp.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://na1.ironcladapp.com/oauth/token
  name: OAuth2
  source: openapi/ironclad-public-api-openapi.yml
scope_count: 60
scope_names:
- public.entities.createEntities
- public.entities.deleteEntities
- public.entities.readEntities
- public.entities.readRelationshipTypes
- public.entities.updateEntities
- public.export.createReports
- public.export.readReports
- public.obligations.createObligations
- public.obligations.deleteObligations
- public.obligations.readObligations
- public.obligations.updateObligations
- public.records.applyContractAction
- public.records.createAttachments
- public.records.createComments
- public.records.createRecords
- public.records.createSmartImportRecords
- public.records.deleteAttachments
- public.records.deleteRecords
- public.records.readAttachments
- public.records.readRecords
- public.records.readSchemas
- public.records.readSmartImportRecords
- public.records.updateRecords
- public.search.conversational
- public.webhooks.createWebhooks
- public.webhooks.deleteWebhooks
- public.webhooks.readWebhooks
- public.webhooks.updateWebhooks
- public.workflows.cancel
- public.workflows.cancelSignatureRequests
- public.workflows.createComments
- public.workflows.createDocuments
- public.workflows.createEmbeddableSignerUrls
- public.workflows.createSignatureRecipientUrls
- public.workflows.createWorkflows
- public.workflows.deleteScheduledSignatureRequest
- public.workflows.deleteSigners
- public.workflows.pauseAndResume
- public.workflows.readApprovals
- public.workflows.readComments
- public.workflows.readDocuments
- public.workflows.readEmailCommunications
- public.workflows.readParticipants
- public.workflows.readRoleAssignees
- public.workflows.readSchemas
- public.workflows.readSignStatus
- public.workflows.readSignatures
- public.workflows.readTurnHistory
- public.workflows.readWorkflows
- public.workflows.remindSigners
- public.workflows.revertToReview
- public.workflows.scheduleSendSignatureRequest
- public.workflows.sendSignatureRequests
- public.workflows.updateApprovals
- public.workflows.updateRoleAssignment
- public.workflows.updateScheduledSignatureRequest
- public.workflows.updateSignaturePacket
- public.workflows.updateSigners
- public.workflows.updateWorkflows
- public.workflows.uploadSignedDocuments
scopes:
- description: Create Entities
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.entities.createEntities
- description: Delete Entities
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.entities.deleteEntities
- description: Read Entities
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.entities.readEntities
- description: Read Relationship Types
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.entities.readRelationshipTypes
- description: Update Entities
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.entities.updateEntities
- description: Create Reports
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.export.createReports
- description: Read Reports
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.export.readReports
- description: Create Obligations
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.obligations.createObligations
- description: Delete Obligations
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.obligations.deleteObligations
- description: Read Obligations
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.obligations.readObligations
- description: Update Obligations
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.obligations.updateObligations
- description: Apply Contract Actions
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.applyContractAction
- description: Create Record Attachments
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.createAttachments
- description: Create Workflow Comments
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.createComments
- description: Create Records
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.createRecords
- description: Create Records via Smart Import
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.createSmartImportRecords
- description: Delete Record Attachments
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.deleteAttachments
- description: Delete Records
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.deleteRecords
- description: Read Record Attachments
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.readAttachments
- description: Read Records
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.readRecords
- description: Read Record Schemas
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.readSchemas
- description: Read Record Import Details from Smart Import
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.readSmartImportRecords
- description: Update Records
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.records.updateRecords
- description: Run Conversational agent Search
  flows:
  - authorizationCode
  scope: public.search.conversational
- description: Create Webhooks
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.webhooks.createWebhooks
- description: Delete Webhooks
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.webhooks.deleteWebhooks
- description: Read Webhooks
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.webhooks.readWebhooks
- description: Update Webhooks
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.webhooks.updateWebhooks
- description: Cancel Workflows
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.cancel
- description: Cancel Signature Requests
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.cancelSignatureRequests
- description: Create Workflow Comments
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.createComments
- description: Create Workflow Documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.createDocuments
- description: Create Embeddable Signature Request Recipient URLs
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.createEmbeddableSignerUrls
- description: Create Signature Request Recipient URLs
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.createSignatureRecipientUrls
- description: Create Workflows
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.createWorkflows
- description: Delete Scheduled Signature Request
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.deleteScheduledSignatureRequest
- description: Delete Signers
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.deleteSigners
- description: Resume and Pause Workflows
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.pauseAndResume
- description: Read Workflow Approvals
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readApprovals
- description: Read Workflow Comments
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readComments
- description: Read Workflow Documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readDocuments
- description: Read Workflow Email Communications
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readEmailCommunications
- description: Read Workflow Participants
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readParticipants
- description: Read Workflow Role Eligible Assignees
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readRoleAssignees
- description: Read Workflow Schemas
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readSchemas
- description: Read Sign Status
  flows:
  - authorizationCode
  scope: public.workflows.readSignStatus
- description: Read Workflow Signatures
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readSignatures
- description: Read Workflow Turn History
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readTurnHistory
- description: Read Workflows
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.readWorkflows
- description: Remind Signers
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.remindSigners
- description: Revert Workflows to Review
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.revertToReview
- description: Schedule Send Signature Request
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.scheduleSendSignatureRequest
- description: Send Signature Requests
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.sendSignatureRequests
- description: Update Workflow Approvals
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.updateApprovals
- description: Update Workflow Role Assignment
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.updateRoleAssignment
- description: Update Scheduled Signature Request
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.updateScheduledSignatureRequest
- description: Update Signature Packet
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.updateSignaturePacket
- description: Update Signers
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.updateSigners
- description: Update Workflows
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.updateWorkflows
- description: Upload Signed Workflow Documents
  flows:
  - authorizationCode
  - clientCredentials
  scope: public.workflows.uploadSignedDocuments
slug: ironclad-scopes
source_filename: ironclad-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ironclad-public-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/ironclad-public-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://na1.ironcladapp.com/oauth/authorize\n    tokenUrl: https://na1.ironcladapp.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://na1.ironcladapp.com/oauth/token\nscopes:\n- scope: public.entities.createEntities\n  description: Create Entities\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.entities.deleteEntities\n  description: Delete Entities\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.entities.readEntities\n  description: Read Entities\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.entities.readRelationshipTypes\n\
  \  description: Read Relationship Types\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.entities.updateEntities\n  description: Update Entities\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.export.createReports\n  description: Create Reports\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.export.readReports\n  description: Read Reports\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.obligations.createObligations\n  description: Create Obligations\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.obligations.deleteObligations\n  description: Delete Obligations\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.obligations.readObligations\n  description: Read Obligations\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.obligations.updateObligations\n  description: Update Obligations\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.applyContractAction\n  description: Apply Contract Actions\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.createAttachments\n  description: Create Record Attachments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.createComments\n  description: Create Workflow Comments\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.createRecords\n  description: Create Records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.createSmartImportRecords\n  description: Create Records via Smart Import\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.deleteAttachments\n  description: Delete Record Attachments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.deleteRecords\n  description: Delete Records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.readAttachments\n  description: Read Record Attachments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n\
  - scope: public.records.readRecords\n  description: Read Records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.readSchemas\n  description: Read Record Schemas\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.readSmartImportRecords\n  description: Read Record Import Details from Smart Import\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.records.updateRecords\n  description: Update Records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.search.conversational\n  description: Run Conversational agent Search\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.webhooks.createWebhooks\n  description:\
  \ Create Webhooks\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.webhooks.deleteWebhooks\n  description: Delete Webhooks\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.webhooks.readWebhooks\n  description: Read Webhooks\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.webhooks.updateWebhooks\n  description: Update Webhooks\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.cancel\n  description: Cancel Workflows\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.cancelSignatureRequests\n  description: Cancel Signature Requests\n  flows:\n  - authorizationCode\n  - clientCredentials\n\
  \  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.createComments\n  description: Create Workflow Comments\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.createDocuments\n  description: Create Workflow Documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.createEmbeddableSignerUrls\n  description: Create Embeddable Signature Request Recipient URLs\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.createSignatureRecipientUrls\n  description: Create Signature Request Recipient URLs\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.createWorkflows\n  description: Create Workflows\n  flows:\n  -\
  \ authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.deleteScheduledSignatureRequest\n  description: Delete Scheduled Signature Request\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.deleteSigners\n  description: Delete Signers\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.pauseAndResume\n  description: Resume and Pause Workflows\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readApprovals\n  description: Read Workflow Approvals\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readComments\n  description: Read Workflow Comments\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readDocuments\n  description: Read Workflow Documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readEmailCommunications\n  description: Read Workflow Email Communications\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readParticipants\n  description: Read Workflow Participants\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readRoleAssignees\n  description: Read Workflow Role Eligible Assignees\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readSchemas\n  description: Read Workflow Schemas\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readSignStatus\n  description: Read Sign Status\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readSignatures\n  description: Read Workflow Signatures\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readTurnHistory\n  description: Read Workflow Turn History\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.readWorkflows\n  description: Read Workflows\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.remindSigners\n  description: Remind Signers\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n\
  - scope: public.workflows.revertToReview\n  description: Revert Workflows to Review\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.scheduleSendSignatureRequest\n  description: Schedule Send Signature Request\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.sendSignatureRequests\n  description: Send Signature Requests\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.updateApprovals\n  description: Update Workflow Approvals\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.updateRoleAssignment\n  description: Update Workflow Role Assignment\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n\
  - scope: public.workflows.updateScheduledSignatureRequest\n  description: Update Scheduled Signature Request\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.updateSignaturePacket\n  description: Update Signature Packet\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.updateSigners\n  description: Update Signers\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.updateWorkflows\n  description: Update Workflows\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n- scope: public.workflows.uploadSignedDocuments\n  description: Upload Signed Workflow Documents\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/scopes/ironclad-scopes.yml
summary_line: 60 scopes · authorizationCode/clientCredentials
tags:
- Contract Lifecycle Management
- CLM
- Contracts
- Legal Tech
- LegalOps
- Enterprise
- Workflows
- eSignature
- Clickwrap
- AI
- OAuth
- SCIM
- Webhooks
token_urls:
- https://na1.ironcladapp.com/oauth/token
---
