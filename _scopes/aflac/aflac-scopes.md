---
api_specs:
- filename: aflac-enterprise-connect-openapi.yml
  format: yaml
  label: Aflac Enterprise Connect API
  slug: enterprise-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-enterprise-connect-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Aflac Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'aflac publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the aflac API on a user''s behalf.


  Tokens are issued from https://auth.enterprise-connect.aflac.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: aflac
provider_slug: aflac
schemes:
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  source: openapi/aflac-enterprise-connect-openapi.yml
scope_count: 6
scope_names:
- claims:read
- claims:write
- eligibility:read
- enrollment:read
- enrollment:write
- groups:read
scopes:
- description: Read claim records
  flows:
  - clientCredentials
  scope: claims:read
- description: Submit claims
  flows:
  - clientCredentials
  scope: claims:write
- description: Verify eligibility
  flows:
  - clientCredentials
  scope: eligibility:read
- description: Read enrollment records
  flows:
  - clientCredentials
  scope: enrollment:read
- description: Create and update enrollments
  flows:
  - clientCredentials
  scope: enrollment:write
- description: Read group records
  flows:
  - clientCredentials
  scope: groups:read
slug: aflac-scopes
source_filename: aflac-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aflac-enterprise-connect-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/aflac-enterprise-connect-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\nscopes:\n- scope: claims:read\n  description: Read claim records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n- scope: claims:write\n  description: Submit claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n- scope: eligibility:read\n  description: Verify eligibility\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n- scope: enrollment:read\n  description: Read enrollment records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n\
  - scope: enrollment:write\n  description: Create and update enrollments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n- scope: groups:read\n  description: Read group records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-enterprise-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/scopes/aflac-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Fortune 500
token_urls:
- https://auth.enterprise-connect.aflac.com/oauth/token
---
