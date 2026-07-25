---
api_specs:
- filename: pandadoc-api-logs-api-openapi.yml
  format: yaml
  label: PandaDoc API Logs API
  slug: pandadoc-api-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-api-logs-api-openapi.yml
- filename: pandadoc-contacts-api-openapi.yml
  format: yaml
  label: PandaDoc Contacts API
  slug: pandadoc-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-contacts-api-openapi.yml
- filename: pandadoc-document-attachments-api-openapi.yml
  format: yaml
  label: PandaDoc Document Attachments API
  slug: pandadoc-document-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-attachments-api-openapi.yml
- filename: pandadoc-document-fields-api-openapi.yml
  format: yaml
  label: PandaDoc Document Fields API
  slug: pandadoc-document-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-fields-api-openapi.yml
- filename: pandadoc-document-link-to-crm-api-openapi.yml
  format: yaml
  label: PandaDoc Document Link to CRM API
  slug: pandadoc-document-link-to-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-link-to-crm-api-openapi.yml
- filename: pandadoc-document-recipients-api-openapi.yml
  format: yaml
  label: PandaDoc Document Recipients API
  slug: pandadoc-document-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-recipients-api-openapi.yml
- filename: pandadoc-document-reminders-api-openapi.yml
  format: yaml
  label: PandaDoc Document Reminders API
  slug: pandadoc-document-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-reminders-api-openapi.yml
- filename: pandadoc-documents-api-openapi.yml
  format: yaml
  label: PandaDoc Documents API
  slug: pandadoc-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-documents-api-openapi.yml
- filename: pandadoc-folders-api-openapi.yml
  format: yaml
  label: PandaDoc Folders API
  slug: pandadoc-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-folders-api-openapi.yml
- filename: pandadoc-forms-api-openapi.yml
  format: yaml
  label: PandaDoc Forms API
  slug: pandadoc-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-forms-api-openapi.yml
- filename: pandadoc-members-api-openapi.yml
  format: yaml
  label: PandaDoc Members API
  slug: pandadoc-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-members-api-openapi.yml
- filename: pandadoc-templates-api-openapi.yml
  format: yaml
  label: PandaDoc Templates API
  slug: pandadoc-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-templates-api-openapi.yml
- filename: pandadoc-webhook-events-api-openapi.yml
  format: yaml
  label: PandaDoc Webhook Events API
  slug: pandadoc-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-webhook-events-api-openapi.yml
- filename: pandadoc-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: PandaDoc Webhook Subscriptions API
  slug: pandadoc-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-webhook-subscriptions-api-openapi.yml
- filename: pandadoc-workspaces-api-openapi.yml
  format: yaml
  label: PandaDoc Workspaces API
  slug: pandadoc-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-workspaces-api-openapi.yml
authorization_urls:
- https://app.pandadoc.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pandadoc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PandaDoc publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PandaDoc API on a user''s behalf.


  Tokens are issued from https://api.pandadoc.com/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PandaDoc
provider_slug: pandadoc
schemes:
- description: OAuth 2.0 authentication. Use the authorization code flow to obtain user-scoped access tokens. Tokens expire after approximately one year.
  flows:
  - authorizationUrl: https://app.pandadoc.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.pandadoc.com/oauth2/access_token
  name: oauth2
  source: openapi/pandadoc-rest-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to documents, templates, contacts, and workspace data.
  flows:
  - authorizationCode
  scope: read
- description: Write access to create and modify documents, templates, and contacts.
  flows:
  - authorizationCode
  scope: write
slug: pandadoc-scopes
source_filename: pandadoc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pandadoc-rest-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/pandadoc-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.pandadoc.com/oauth2/authorize\n    tokenUrl: https://api.pandadoc.com/oauth2/access_token\n  description: OAuth 2.0 authentication. Use the authorization code flow to obtain user-scoped\n    access tokens. Tokens expire after approximately one year.\nscopes:\n- scope: read\n  description: Read access to documents, templates, contacts, and workspace data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pandadoc-rest-api-openapi.yml\n- scope: write\n  description: Write access to create and modify documents, templates, and contacts.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pandadoc-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/scopes/pandadoc-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Document Automation
- E-Signature
- Document Management
- Document Generation
- Webhooks
token_urls:
- https://api.pandadoc.com/oauth2/access_token
---
