---
api_specs:
- filename: resistant-ai-documents-openapi.json
  format: json
  label: Resistant Documents API
  slug: resistant-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-documents-openapi.json
- filename: resistant-ai-tenant-management-openapi.json
  format: json
  label: Resistant Documents Tenant Management API
  slug: resistant-documents-tenant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-tenant-management-openapi.json
authorization_urls: []
description: ''
docs: https://developers.resistant.ai/getting-started/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Resistant Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Resistant AI publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Resistant AI API on a user''s behalf.


  Tokens are issued from https://eu.id.resistant.ai/oauth2/aus2un1hkrKhPjir4417/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Resistant AI
provider_slug: resistant-ai
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://eu.id.resistant.ai/oauth2/aus2un1hkrKhPjir4417/v1/token
  name: OAuth2
  source: openapi/resistant-ai-documents-openapi.json
scope_count: 2
scope_names:
- submissions.read
- submissions.write
scopes:
- description: Read analysis results for a submission
  flows:
  - clientCredentials
  scope: submissions.read
- description: Create a new submission
  flows:
  - clientCredentials
  scope: submissions.write
slug: resistant-ai-scopes
source_filename: resistant-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/resistant-ai-documents-openapi.json\ndocs: https://developers.resistant.ai/getting-started/authentication\nschemes:\n- name: OAuth2\n  source: openapi/resistant-ai-documents-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://eu.id.resistant.ai/oauth2/aus2un1hkrKhPjir4417/v1/token\nscopes:\n- scope: submissions.read\n  description: Read analysis results for a submission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/resistant-ai-documents-openapi.json\n- scope: submissions.write\n  description: Create a new submission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/resistant-ai-documents-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/scopes/resistant-ai-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- Ai
- Fraud Detection
- Financial Crime
- Document Verification
- Document Forensics
- AML
- Identity Verification
- Fintech
- Machine Learning
token_urls:
- https://eu.id.resistant.ai/oauth2/aus2un1hkrKhPjir4417/v1/token
---
