---
api_specs:
- filename: v1
  format: yaml
  label: Power Apps API
  slug: power-apps-api
  spec_type: OpenAPI
  url: https://api.powerapps.com/openapi/v1
- filename: v1
  format: yaml
  label: Power Automate API
  slug: power-automate-api
  spec_type: OpenAPI
  url: https://api.flow.microsoft.com/openapi/v1
- filename: swagger.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://api.powerbi.com/v1.0/myorg/swagger.json
- filename: power-platform-api-openapi.json
  format: json
  label: Power Platform Unified API
  slug: power-platform-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/openapi/power-platform-api-openapi.json
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Power Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Power Platform APIs publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Power Platform APIs API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schemes:
- description: Microsoft Entra ID OAuth 2.0 authentication. Register your application and obtain tokens via the Microsoft identity platform.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  source: openapi/power-platform-api-openapi.json
scope_count: 1
scope_names:
- https://api.powerplatform.com/.default
scopes:
- description: Access Power Platform API resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://api.powerplatform.com/.default
slug: power-platform-scopes
source_filename: power-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/power-platform-api-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/power-platform-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n  description: Microsoft Entra ID OAuth 2.0 authentication. Register your application and obtain\n    tokens via the Microsoft identity platform.\nscopes:\n- scope: https://api.powerplatform.com/.default\n  description: Access Power Platform API resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/power-platform-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/scopes/power-platform-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
- https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
---
