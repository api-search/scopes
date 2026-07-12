---
authorization_urls:
- https://api.bamboohr.com/oauth/authorize.php
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bamboohr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BambooHR publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BambooHR API on a user''s behalf.


  Tokens are issued from https://api.bamboohr.com/token.php.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BambooHR
provider_slug: bamboohr
schemes:
- description: OAuth 2.0 authorization code flow (for multi-customer apps).
  flows:
  - authorizationUrl: https://api.bamboohr.com/oauth/authorize.php
    flow: authorizationCode
    tokenUrl: https://api.bamboohr.com/token.php
  name: oauth2
  source: openapi/bamboohr-openapi.yml
scope_count: 1
scope_names:
- offline_access
scopes:
- description: Issue a refresh token along with the access token
  flows:
  - authorizationCode
  scope: offline_access
slug: bamboohr-scopes
source_filename: bamboohr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bamboohr-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bamboohr-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bamboohr.com/oauth/authorize.php\n    tokenUrl: https://api.bamboohr.com/token.php\n  description: OAuth 2.0 authorization code flow (for multi-customer apps).\nscopes:\n- scope: offline_access\n  description: Issue a refresh token along with the access token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bamboohr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/scopes/bamboohr-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- HR
- HRIS
- Human Resources
- Payroll
- Time Tracking
- Applicant Tracking
- Performance Management
token_urls:
- https://api.bamboohr.com/token.php
---
