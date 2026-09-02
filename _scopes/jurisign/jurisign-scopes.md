---
api_specs:
- filename: jurisign-api-openapi.yml
  format: yaml
  label: JuriSign REST API
  slug: jurisign-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/openapi/jurisign-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.jurisign.fr/developpeurs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Jurisign Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'JuriSign uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JuriSign
provider_slug: jurisign
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: jurisign-scopes
source_filename: jurisign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: searched\nsource: https://www.jurisign.fr/api/openapi.json\ndocs: https://www.jurisign.fr/developpeurs\noauth2: false\nmodel: bearer-token-abilities\nmodel_note: >-\n  These are NOT OAuth 2.0 scopes. JuriSign issues Laravel Sanctum personal access tokens and the `scopes` field on\n  POST /auth/token restricts the token's abilities. There is no authorization server, no /authorize or /token\n  OAuth endpoint, no consent screen, and /.well-known/oauth-authorization-server returns 404. The artifact is\n  recorded under the scope vocabulary because the provider publishes a real, enumerable, per-token permission set\n  that an agent must reason about - but it is a token-ability model, and calling it OAuth would be wrong.\nenforcement:\n  description: Every endpoint checks the token's abilities and returns 403 if the required scope is missing.\n  status_on_missing_scope: 403\ndefault_behaviour:\n  description: >-\n    Omitting `scopes` on POST /auth/token\
  \ grants all five scopes. This is the documented default and preserves\n    behaviour for integrations written before scopes existed.\n  scopes_granted: all\nrequest_example: |\n  POST /api/v1/auth/token\n  { \"email\": \"...\", \"password\": \"...\", \"device_name\": \"my-backoffice\",\n    \"scopes\": [\"documents:read\", \"sign-requests:read\"] }\nscope_count: 5\nscopes:\n- name: documents:read\n  description: Read documents - list, retrieve and download uploaded documents.\n  operations: [listDocuments, getDocument, downloadDocument]\n- name: documents:write\n  description: Create and remove documents - upload PDFs (including multi-file merge) and delete drafts.\n  operations: [uploadDocument, deleteDocument]\n- name: sign-requests:read\n  description: >-\n    Read signature requests, and also covers the templates and bulk-* read endpoints, per the spec: \"sign-requests:read\n    / sign-requests:write also cover the templates and bulk-* endpoints.\"\n  operations: [listSignRequests,\
  \ getSignRequest, downloadSignedPdf, downloadProof, listTemplates, getTemplate, listBulkTemplates, getBulkTemplate, listBulkCampaigns, getBulkCampaign, exportBulkCampaignResults, listPublicForms, getPublicForm]\n- name: sign-requests:write\n  description: >-\n    Create, send, cancel and otherwise mutate signature requests, and also covers the templates and bulk-* write\n    endpoints.\n  operations: [createSignRequest, sendSignRequest, cancelSignRequest, createSignRequestFromTemplate, deleteTemplate, createBulkTemplate, updateBulkTemplate, deleteBulkTemplate, createBulkCampaign, launchBulkCampaign, cancelBulkCampaign, retryBulkCampaign, deleteBulkCampaign, createPublicForm, updatePublicForm, deletePublicForm, rotatePublicFormToken]\n- name: webhooks:manage\n  description: Manage webhook endpoints - list, create, update, delete, read delivery logs and regenerate secrets.\n  operations: [listWebhooks, createWebhook, updateWebhook, deleteWebhook, getWebhookLogs, regenerateWebhookSecret]\n\
  operation_mapping_note: >-\n  The spec names the five scopes and states the templates/bulk coverage rule, but does not annotate each operation\n  with its required scope. The per-scope `operations` lists above apply that stated rule to the operation set; they\n  are a faithful reading of the published rule, not a per-operation assertion by the provider. Least-privilege\n  callers should verify against a 403 in the sandbox.\nuse_case_published:\n  description: >-\n    The developer page frames scopes as a least-privilege pattern - \"Un jeton en lecture seule pour votre tableau\n    de bord, un autre en ecriture pour vos automatisations.\"\n  source: https://www.jurisign.fr/developpeurs\nunscoped_operations:\n  note: >-\n    Five operations sit outside the scope model. The three authentication operations issue or revoke the token\n    itself and so cannot require one; getStatus is unauthenticated; getAccountCredits is documented as scoped\n    strictly to the authenticated token's organization\
  \ but is not attributed to a named scope in the spec.\n  operations: [createToken, createSandboxToken, revokeToken, getStatus, getAccountCredits]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jurisign/refs/heads/main/scopes/jurisign-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Electronic Signature
- E-Signature
- eIDAS
- Document Signing
- PDF
- Webhook
- OTP
- GDPR
- France
- Legal Tech
- Identity Verification
- Audit Trail
- data-residency-eu
token_urls: []
---
