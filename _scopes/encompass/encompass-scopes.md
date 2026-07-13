---
api_specs:
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Management API
  slug: encompass-loan-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Loan Pipeline API
  slug: encompass-loan-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Borrower Pair & Applications API
  slug: encompass-borrower-pair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Contacts API
  slug: encompass-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass eFolder Documents & Attachments API
  slug: encompass-efolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Milestones & Associates API
  slug: encompass-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Conditions API
  slug: encompass-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Users API
  slug: encompass-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
- filename: encompass-openapi.yml
  format: yaml
  label: Encompass Webhooks API
  slug: encompass-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/openapi/encompass-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.icemortgagetechnology.com/developer-connect/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Encompass Scopes
name_suffix: OAuth Scopes
note: Encompass Developer Connect uses a single OAuth 2.0 scope, lp (Lending Platform), across all grant types; fine-grained permissions are governed by token claims, the Encompass instance, and user personas/roles rather than granular scopes (https://developer.icemortgagetechnology.com/developer-connect/docs/authentication-and-authorization-in-the-encompass-lending-platform).
overview: 'Encompass publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Encompass API on a user''s behalf.


  Tokens are issued from https://api.elliemae.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Encompass
provider_slug: encompass
schemes:
- description: OAuth 2.0 client credentials / authorization code issued per Encompass instance.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.elliemae.com/oauth2/v1/token
  name: oAuth2
  source: openapi/encompass-openapi.yml
scope_count: 1
scope_names:
- lp
scopes:
- description: Lending Platform - the single scope required for access to the Encompass Developer Connect (Lending Platform) APIs; used with the authorization_code, password, client_credentials, and token-exchange (user impersonation) grant types.
  flows: []
  scope: lp
slug: encompass-scopes
source_filename: encompass-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/encompass-openapi.yml\ndocs: https://developer.icemortgagetechnology.com/developer-connect/docs/authentication\nnote: Encompass Developer Connect uses a single OAuth 2.0 scope, lp (Lending Platform),\n  across all grant types; fine-grained permissions are governed by token claims, the\n  Encompass instance, and user personas/roles rather than granular scopes\n  (https://developer.icemortgagetechnology.com/developer-connect/docs/authentication-and-authorization-in-the-encompass-lending-platform).\nschemes:\n- name: oAuth2\n  source: openapi/encompass-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.elliemae.com/oauth2/v1/token\n  description: OAuth 2.0 client credentials / authorization code issued per Encompass instance.\nscopes:\n- scope: lp\n  description: Lending Platform - the single scope required for access to the Encompass\n    Developer Connect (Lending Platform) APIs; used with\
  \ the authorization_code, password,\n    client_credentials, and token-exchange (user impersonation) grant types.\n  sources:\n  - https://developer.icemortgagetechnology.com/developer-connect/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encompass/refs/heads/main/scopes/encompass-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Mortgage
- Loan Origination
- LOS
- Fintech
- ICE Mortgage Technology
- Ellie Mae
- Lending
token_urls:
- https://api.elliemae.com/oauth2/v1/token
---
