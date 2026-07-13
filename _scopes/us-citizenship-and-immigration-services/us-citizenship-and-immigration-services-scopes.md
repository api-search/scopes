---
api_specs:
- filename: uscis-case-status-api-openapi.yml
  format: yaml
  label: USCIS Case Status API
  slug: uscis-case-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-case-status-api-openapi.yml
- filename: uscis-foia-api-openapi.yml
  format: yaml
  label: USCIS FOIA Request and Status API
  slug: uscis-foia-request-and-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-foia-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Us Citizenship And Immigration Services Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'US Citizenship and Immigration Services publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the US Citizenship and Immigration Services API on a user''s behalf.


  Tokens are issued from https://api-int.uscis.gov/oauth/accesstoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: US Citizenship and Immigration Services
provider_slug: us-citizenship-and-immigration-services
schemes:
- description: OAuth 2.0 Client Credentials flow. Obtain an access token from the USCIS token endpoint using your client_id and client_secret registered at developer.uscis.gov. Tokens expire after 1,800 seconds (30 minutes).
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-int.uscis.gov/oauth/accesstoken
  name: OAuth2
  source: openapi/uscis-case-status-api-openapi.yml
- description: OAuth 2.0 Client Credentials flow. Obtain an access token from the USCIS token endpoint using your client_id and client_secret registered at developer.uscis.gov. Tokens expire after 1,800 seconds (30 minutes).
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-int.uscis.gov/oauth/accesstoken
  name: OAuth2
  source: openapi/uscis-foia-api-openapi.yml
scope_count: 3
scope_names:
- read:case-status
- read:foia-requests
- write:foia-requests
scopes:
- description: Read immigration case status information
  flows:
  - clientCredentials
  scope: read:case-status
- description: Read FOIA request status
  flows:
  - clientCredentials
  scope: read:foia-requests
- description: Submit FOIA requests
  flows:
  - clientCredentials
  scope: write:foia-requests
slug: us-citizenship-and-immigration-services-scopes
source_filename: us-citizenship-and-immigration-services-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uscis-case-status-api-openapi.yml, openapi/uscis-foia-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/uscis-case-status-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-int.uscis.gov/oauth/accesstoken\n  description: OAuth 2.0 Client Credentials flow. Obtain an access token from the USCIS token\n    endpoint using your client_id and client_secret registered at developer.uscis.gov. Tokens\n    expire after 1,800 seconds (30 minutes).\n- name: OAuth2\n  source: openapi/uscis-foia-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-int.uscis.gov/oauth/accesstoken\n  description: OAuth 2.0 Client Credentials flow. Obtain an access token from the USCIS token\n    endpoint using your client_id and client_secret registered at developer.uscis.gov. Tokens\n    expire after 1,800 seconds (30 minutes).\nscopes:\n- scope: read:case-status\n  description:\
  \ Read immigration case status information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uscis-case-status-api-openapi.yml\n- scope: read:foia-requests\n  description: Read FOIA request status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uscis-foia-api-openapi.yml\n- scope: write:foia-requests\n  description: Submit FOIA requests\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uscis-foia-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/scopes/us-citizenship-and-immigration-services-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Federal Government
- Immigration
- Citizenship
- Case Status
- FOIA
token_urls:
- https://api-int.uscis.gov/oauth/accesstoken
---
