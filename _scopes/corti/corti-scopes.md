---
api_specs:
- filename: corti-transcribe-asyncapi.json
  format: json
  label: Corti Speech to Text API
  slug: corti-speech-to-text-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/asyncapi/corti-transcribe-asyncapi.json
- filename: corti-stream-asyncapi.json
  format: json
  label: Corti Ambient Documentation API
  slug: corti-ambient-documentation-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/asyncapi/corti-stream-asyncapi.json
authorization_urls:
- https://auth.eu.corti.app/realms/base/protocol/openid-connect/auth
description: OAuth 2.0 scopes harvested from Corti's live Keycloak OpenID Connect discovery document (base realm). Corti issues short-lived (5 minute) access tokens via the client_credentials grant; streaming clients may request limited-scope tokens (e.g. "openid transcribe" or "openid streams"). Standard OIDC scopes (openid, profile, email, phone, address, offline_access, roles, groups) are omitted from the per-scope list below and noted under oidc_standard_scopes.
docs: https://docs.corti.ai/authentication/overview
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Corti Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Corti publishes 44 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Corti API on a user''s behalf.


  Tokens are issued from https://auth.eu.corti.app/realms/base/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Corti
provider_slug: corti
schemes:
- environments:
  - eu: https://auth.eu.corti.app
  - us: https://auth.us.corti.app
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.eu.corti.app/realms/base/protocol/openid-connect/token
  - authorizationUrl: https://auth.eu.corti.app/realms/base/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.eu.corti.app/realms/base/protocol/openid-connect/token
  name: CortiAuth
  type: oauth2
scope_count: 44
scope_names:
- interactions:read
- interactions:readall
- interactions:write
- interactions:update
- interactions:delete
- recordings:read
- recordings:write
- recordings:delete
- transcripts:read
- transcripts:write
- transcripts:delete
- documents:read
- documents:write
- documents:update
- documents:delete
- guided_documents:read
- guided_documents:write
- guided_documents:update
- guided_documents:delete
- guided_templates_sections:read
- guided_templates_sections:write
- guided_templates_sections:update
- guided_templates_sections:delete
- templates:read
- codes:read
- codes:write
- codes:update
- facts:read
- facts:write
- facts:update
- transcribe
- streams
- tools:write
- anonymize:write
- languages:read
- admin:read
- admin:write
- admin-templates:read
- admin-logging:write
- admin-retention:write
- admin-retention-policy:write
- admin-caching:write
- admin-db:write
- admin-triggers:write
scopes:
- description: Read interactions
  flows: []
  scope: interactions:read
- description: Read all interactions in the tenant
  flows: []
  scope: interactions:readall
- description: Create interactions
  flows: []
  scope: interactions:write
- description: Update interactions
  flows: []
  scope: interactions:update
- description: Delete interactions
  flows: []
  scope: interactions:delete
- description: Read recordings
  flows: []
  scope: recordings:read
- description: Upload/create recordings
  flows: []
  scope: recordings:write
- description: Delete recordings
  flows: []
  scope: recordings:delete
- description: Read transcripts
  flows: []
  scope: transcripts:read
- description: Create/update transcripts
  flows: []
  scope: transcripts:write
- description: Delete transcripts
  flows: []
  scope: transcripts:delete
- description: Read generated documents
  flows: []
  scope: documents:read
- description: Generate documents
  flows: []
  scope: documents:write
- description: Update documents
  flows: []
  scope: documents:update
- description: Delete documents
  flows: []
  scope: documents:delete
- description: Read guided (structured) documents
  flows: []
  scope: guided_documents:read
- description: Generate guided documents
  flows: []
  scope: guided_documents:write
- description: Update guided documents
  flows: []
  scope: guided_documents:update
- description: Delete guided documents
  flows: []
  scope: guided_documents:delete
- description: Read guided template sections
  flows: []
  scope: guided_templates_sections:read
- description: Create guided template sections
  flows: []
  scope: guided_templates_sections:write
- description: Update guided template sections
  flows: []
  scope: guided_templates_sections:update
- description: Delete guided template sections
  flows: []
  scope: guided_templates_sections:delete
- description: Read document templates
  flows: []
  scope: templates:read
- description: Read predicted medical codes
  flows: []
  scope: codes:read
- description: Predict/generate medical codes
  flows: []
  scope: codes:write
- description: Update/select medical codes
  flows: []
  scope: codes:update
- description: Read facts extracted from interactions
  flows: []
  scope: facts:read
- description: Add/extract facts
  flows: []
  scope: facts:write
- description: Update facts
  flows: []
  scope: facts:update
- description: Access the real-time stateless speech-to-text (transcribe) WebSocket
  flows: []
  scope: transcribe
- description: Access the real-time ambient documentation (stream) WebSocket
  flows: []
  scope: streams
- description: Invoke stateless tools (e.g. coding
  flows: []
  scope: tools:write
- description: Anonymize/de-identify content
  flows: []
  scope: anonymize:write
- description: List supported languages
  flows: []
  scope: languages:read
- description: Administration API read access
  flows: []
  scope: admin:read
- description: Administration API write access
  flows: []
  scope: admin:write
- description: Read admin-managed templates
  flows: []
  scope: admin-templates:read
- description: Manage admin logging configuration
  flows: []
  scope: admin-logging:write
- description: Manage data retention
  flows: []
  scope: admin-retention:write
- description: Manage retention policy
  flows: []
  scope: admin-retention-policy:write
- description: Manage caching configuration
  flows: []
  scope: admin-caching:write
- description: Manage database configuration
  flows: []
  scope: admin-db:write
- description: Manage admin triggers
  flows: []
  scope: admin-triggers:write
slug: corti-scopes
source_filename: corti-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.eu.corti.app/realms/base/.well-known/openid-configuration\ndocs: https://docs.corti.ai/authentication/overview\ndescription: >-\n  OAuth 2.0 scopes harvested from Corti's live Keycloak OpenID Connect discovery\n  document (base realm). Corti issues short-lived (5 minute) access tokens via the\n  client_credentials grant; streaming clients may request limited-scope tokens\n  (e.g. \"openid transcribe\" or \"openid streams\"). Standard OIDC scopes (openid,\n  profile, email, phone, address, offline_access, roles, groups) are omitted from\n  the per-scope list below and noted under oidc_standard_scopes.\nschemes:\n- name: CortiAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.eu.corti.app/realms/base/protocol/openid-connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.eu.corti.app/realms/base/protocol/openid-connect/auth\n    tokenUrl: https://auth.eu.corti.app/realms/base/protocol/openid-connect/token\n\
  \  environments:\n  - eu: https://auth.eu.corti.app\n  - us: https://auth.us.corti.app\noidc_standard_scopes:\n- openid\n- profile\n- email\n- phone\n- address\n- offline_access\n- roles\n- groups\n- web-origins\n- microprofile-jwt\n- acr\n- basic\n- service_account\nscopes:\n- {scope: 'interactions:read', description: Read interactions}\n- {scope: 'interactions:readall', description: Read all interactions in the tenant}\n- {scope: 'interactions:write', description: Create interactions}\n- {scope: 'interactions:update', description: Update interactions}\n- {scope: 'interactions:delete', description: Delete interactions}\n- {scope: 'recordings:read', description: Read recordings}\n- {scope: 'recordings:write', description: Upload/create recordings}\n- {scope: 'recordings:delete', description: Delete recordings}\n- {scope: 'transcripts:read', description: Read transcripts}\n- {scope: 'transcripts:write', description: Create/update transcripts}\n- {scope: 'transcripts:delete', description:\
  \ Delete transcripts}\n- {scope: 'documents:read', description: Read generated documents}\n- {scope: 'documents:write', description: Generate documents}\n- {scope: 'documents:update', description: Update documents}\n- {scope: 'documents:delete', description: Delete documents}\n- {scope: 'guided_documents:read', description: Read guided (structured) documents}\n- {scope: 'guided_documents:write', description: Generate guided documents}\n- {scope: 'guided_documents:update', description: Update guided documents}\n- {scope: 'guided_documents:delete', description: Delete guided documents}\n- {scope: 'guided_templates_sections:read', description: Read guided template sections}\n- {scope: 'guided_templates_sections:write', description: Create guided template sections}\n- {scope: 'guided_templates_sections:update', description: Update guided template sections}\n- {scope: 'guided_templates_sections:delete', description: Delete guided template sections}\n- {scope: 'templates:read', description:\
  \ Read document templates}\n- {scope: 'codes:read', description: Read predicted medical codes}\n- {scope: 'codes:write', description: Predict/generate medical codes}\n- {scope: 'codes:update', description: Update/select medical codes}\n- {scope: 'facts:read', description: Read facts extracted from interactions}\n- {scope: 'facts:write', description: Add/extract facts}\n- {scope: 'facts:update', description: Update facts}\n- {scope: 'transcribe', description: Access the real-time stateless speech-to-text (transcribe) WebSocket}\n- {scope: 'streams', description: Access the real-time ambient documentation (stream) WebSocket}\n- {scope: 'tools:write', description: Invoke stateless tools (e.g. coding, fact extraction)}\n- {scope: 'anonymize:write', description: Anonymize/de-identify content}\n- {scope: 'languages:read', description: List supported languages}\n- {scope: 'admin:read', description: Administration API read access}\n- {scope: 'admin:write', description: Administration API write\
  \ access}\n- {scope: 'admin-templates:read', description: Read admin-managed templates}\n- {scope: 'admin-logging:write', description: Manage admin logging configuration}\n- {scope: 'admin-retention:write', description: Manage data retention}\n- {scope: 'admin-retention-policy:write', description: Manage retention policy}\n- {scope: 'admin-caching:write', description: Manage caching configuration}\n- {scope: 'admin-db:write', description: Manage database configuration}\n- {scope: 'admin-triggers:write', description: Manage admin triggers}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corti/refs/heads/main/scopes/corti-scopes.yml
summary_line: 44 scopes · clientCredentials/authorizationCode
tags:
- Company
- Health
- Healthcare
- Artificial Intelligence
- Speech to Text
- Medical Coding
- Clinical Documentation
- Agents
- Machine Learning
token_urls:
- https://auth.eu.corti.app/realms/base/protocol/openid-connect/token
---
