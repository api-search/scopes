---
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Azure Test Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Azure DevTest Labs publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Azure DevTest Labs API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
schemes:
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/azure-test-labs-openapi.yaml
scope_count: 1
scope_names:
- user_impersonation
scopes:
- description: Access Microsoft Azure
  flows:
  - implicit
  scope: user_impersonation
slug: azure-test-labs-scopes
source_filename: azure-test-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-test-labs-openapi.yaml\nschemes:\n- name: azure_auth\n  source: openapi/azure-test-labs-openapi.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: OAuth2 Implicit Grant\nscopes:\n- scope: user_impersonation\n  description: Access Microsoft Azure\n  flows:\n  - implicit\n  sources:\n  - openapi/azure-test-labs-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/scopes/azure-test-labs-scopes.yml
summary_line: 1 scope · implicit
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
token_urls: []
---
