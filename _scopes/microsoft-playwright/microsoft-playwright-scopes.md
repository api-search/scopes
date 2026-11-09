---
api_specs:
- filename: microsoft-playwright-accountquotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Account Quotas API
  slug: microsoft-playwright-accountquotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accountquotas-api-openapi.yml
- filename: microsoft-playwright-accounts-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Accounts API
  slug: microsoft-playwright-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-accounts-api-openapi.yml
- filename: microsoft-playwright-operations-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Operations API
  slug: microsoft-playwright-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-operations-api-openapi.yml
- filename: microsoft-playwright-quotas-api-openapi.yml
  format: yaml
  label: Microsoft Playwright Quotas API
  slug: microsoft-playwright-quotas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-playwright/openapi/microsoft-playwright-quotas-api-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/authorize
description: ''
docs: ''
flows:
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Microsoft Playwright Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Playwright publishes 2 OAuth 2.0 scopes via the implicit and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Playwright API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/v2.0/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Playwright
provider_slug: microsoft-playwright
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: OAuth2Auth
  source: openapi/microsoft-playwright-authmanager-openapi.yml
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/v2.0/oauth2/token
  name: OAuth2Auth_
  source: openapi/microsoft-playwright-authmanager-openapi.yml
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
  name: azure_auth
  source: openapi/microsoft-playwright-management-openapi.yml
scope_count: 2
scope_names:
- https://playwright.microsoft.com/.default
- user_impersonation
scopes:
- description: ''
  flows:
  - authorizationCode
  - implicit
  scope: https://playwright.microsoft.com/.default
- description: impersonate your user account
  flows:
  - implicit
  scope: user_impersonation
slug: microsoft-playwright-scopes
source_filename: microsoft-playwright-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/microsoft-playwright-authmanager-openapi.yml, openapi/microsoft-playwright-management-openapi.yml\nschemes:\n- name: OAuth2Auth\n  source: openapi/microsoft-playwright-authmanager-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n- name: OAuth2Auth_\n  source: openapi/microsoft-playwright-authmanager-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/v2.0/oauth2/token\n- name: azure_auth\n  source: openapi/microsoft-playwright-management-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n  description: Azure Active Directory OAuth2 Flow.\nscopes:\n- scope: https://playwright.microsoft.com/.default\n  flows:\n  - authorizationCode\n  - implicit\n\
  \  sources:\n  - openapi/microsoft-playwright-authmanager-openapi.yml\n- scope: user_impersonation\n  description: impersonate your user account\n  flows:\n  - implicit\n  sources:\n  - openapi/microsoft-playwright-management-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-playwright/scopes/microsoft-playwright-scopes.yml
summary_line: 2 scopes · implicit/authorizationCode
tags:
- Browser Automation
- End-to-End Testing
- Microsoft
- Testing
- Open Source
- MCP
- Microsoft Azure
token_bound: false
token_urls:
- https://login.microsoftonline.com/common/v2.0/oauth2/token
---
