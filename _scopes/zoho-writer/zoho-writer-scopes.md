---
authorization_urls:
- https://accounts.zoho.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zoho Writer Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zoho Writer publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zoho Writer API on a user''s behalf.


  Tokens are issued from https://accounts.zoho.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zoho Writer
provider_slug: zoho-writer
schemes:
- description: OAuth 2.0 authentication. Refer to https://www.zoho.com/writer/help/api/v1/oauth-2.html for setup.
  flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: OAuth2
  source: openapi/zoho-writer-openapi.json
scope_count: 6
scope_names:
- WorkDrive.files.ALL
- WorkDrive.organization.ALL
- WorkDrive.workspace.ALL
- ZohoPC.files.ALL
- ZohoWriter.documentEditor.ALL
- ZohoWriter.merge.ALL
scopes:
- description: Access to WorkDrive files
  flows:
  - authorizationCode
  scope: WorkDrive.files.ALL
- description: Organization-level WorkDrive access
  flows:
  - authorizationCode
  scope: WorkDrive.organization.ALL
- description: Workspace-level WorkDrive access
  flows:
  - authorizationCode
  scope: WorkDrive.workspace.ALL
- description: Access to Zoho personal cloud files
  flows:
  - authorizationCode
  scope: ZohoPC.files.ALL
- description: Full access to document editor operations
  flows:
  - authorizationCode
  scope: ZohoWriter.documentEditor.ALL
- description: Full access to merge operations
  flows:
  - authorizationCode
  scope: ZohoWriter.merge.ALL
slug: zoho-writer-scopes
source_filename: zoho-writer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zoho-writer-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/zoho-writer-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n  description: OAuth 2.0 authentication. Refer to https://www.zoho.com/writer/help/api/v1/oauth-2.html\n    for setup.\nscopes:\n- scope: WorkDrive.files.ALL\n  description: Access to WorkDrive files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-writer-openapi.json\n- scope: WorkDrive.organization.ALL\n  description: Organization-level WorkDrive access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-writer-openapi.json\n- scope: WorkDrive.workspace.ALL\n  description: Workspace-level WorkDrive access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-writer-openapi.json\n- scope: ZohoPC.files.ALL\n  description: Access to Zoho\
  \ personal cloud files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-writer-openapi.json\n- scope: ZohoWriter.documentEditor.ALL\n  description: Full access to document editor operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-writer-openapi.json\n- scope: ZohoWriter.merge.ALL\n  description: Full access to merge operations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zoho-writer-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-writer/refs/heads/main/scopes/zoho-writer-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Documents
- Word Processor
- Mail Merge
- Document Generation
- Electronic Signatures
- Zoho
- Office Suite
- Automation
token_urls:
- https://accounts.zoho.com/oauth/v2/token
---
