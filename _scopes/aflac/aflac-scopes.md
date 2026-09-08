---
api_specs:
- filename: aflac-claims-api-openapi.yml
  format: yaml
  label: aflac Claims API
  slug: aflac-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-claims-api-openapi.yml
- filename: aflac-eligibility-api-openapi.yml
  format: yaml
  label: aflac Eligibility API
  slug: aflac-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-eligibility-api-openapi.yml
- filename: aflac-enrollment-api-openapi.yml
  format: yaml
  label: aflac Enrollment API
  slug: aflac-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-enrollment-api-openapi.yml
- filename: aflac-groups-api-openapi.yml
  format: yaml
  label: aflac Groups API
  slug: aflac-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-groups-api-openapi.yml
- filename: aflac-policies-api-openapi.yml
  format: yaml
  label: aflac Policies API
  slug: aflac-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/openapi/aflac-policies-api-openapi.yml
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
overview: 'Aflac publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aflac API on a user''s behalf.


  Tokens are issued from https://auth.enterprise-connect.aflac.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aflac
provider_slug: aflac
schemes:
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  source: openapi/aflac-claims-api-openapi.yml
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  source: openapi/aflac-eligibility-api-openapi.yml
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  source: openapi/aflac-enrollment-api-openapi.yml
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  source: openapi/aflac-groups-api-openapi.yml
- description: OAuth 2.0 client credentials flow for server-to-server API access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token
  name: oauth2
  source: openapi/aflac-policies-api-openapi.yml
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
source_yaml: "# NOTE added 2026-09-04 by the enrichment pass. These scopes and the tokenUrl below are DERIVED\n# from openapi/_ae-authored/ scaffolds written by API Evangelist, not from anything Aflac\n# published. Aflac publishes NO OAuth scope reference anonymously, and the host\n# auth.enterprise-connect.aflac.com in the tokenUrl resolves NXDOMAIN (checked 2026-09-04).\n# Aflac's own documentation states OAuth 2.0 client-credentials is the only supported method but\n# does not enumerate scopes. Treat every scope string below as an API Evangelist derivation.\n# See authentication/aflac-authentication.yml for the searched, first-party auth profile.\ngenerated: '2026-09-04'\nmethod: derived\nsource: openapi/aflac-claims-api-openapi.yml, openapi/aflac-eligibility-api-openapi.yml, openapi/aflac-enrollment-api-openapi.yml,\n  openapi/aflac-groups-api-openapi.yml, openapi/aflac-policies-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/aflac-claims-api-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\n- name: oauth2\n  source: openapi/aflac-eligibility-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\n- name: oauth2\n  source: openapi/aflac-enrollment-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\n- name: oauth2\n  source: openapi/aflac-groups-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\n- name: oauth2\n  source: openapi/aflac-policies-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.enterprise-connect.aflac.com/oauth/token\n  description: OAuth 2.0 client credentials flow for server-to-server API access.\nscopes:\n- scope: claims:read\n  description: Read claim records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-claims-api-openapi.yml\n  - openapi/aflac-eligibility-api-openapi.yml\n  - openapi/aflac-enrollment-api-openapi.yml\n  - openapi/aflac-groups-api-openapi.yml\n  - openapi/aflac-policies-api-openapi.yml\n- scope: claims:write\n  description: Submit claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-claims-api-openapi.yml\n  - openapi/aflac-eligibility-api-openapi.yml\n  - openapi/aflac-enrollment-api-openapi.yml\n  - openapi/aflac-groups-api-openapi.yml\n  - openapi/aflac-policies-api-openapi.yml\n- scope: eligibility:read\n  description: Verify eligibility\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-claims-api-openapi.yml\n  - openapi/aflac-eligibility-api-openapi.yml\n\
  \  - openapi/aflac-enrollment-api-openapi.yml\n  - openapi/aflac-groups-api-openapi.yml\n  - openapi/aflac-policies-api-openapi.yml\n- scope: enrollment:read\n  description: Read enrollment records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-claims-api-openapi.yml\n  - openapi/aflac-eligibility-api-openapi.yml\n  - openapi/aflac-enrollment-api-openapi.yml\n  - openapi/aflac-groups-api-openapi.yml\n  - openapi/aflac-policies-api-openapi.yml\n- scope: enrollment:write\n  description: Create and update enrollments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-claims-api-openapi.yml\n  - openapi/aflac-eligibility-api-openapi.yml\n  - openapi/aflac-enrollment-api-openapi.yml\n  - openapi/aflac-groups-api-openapi.yml\n  - openapi/aflac-policies-api-openapi.yml\n- scope: groups:read\n  description: Read group records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aflac-claims-api-openapi.yml\n  - openapi/aflac-eligibility-api-openapi.yml\n  - openapi/aflac-enrollment-api-openapi.yml\n\
  \  - openapi/aflac-groups-api-openapi.yml\n  - openapi/aflac-policies-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aflac/refs/heads/main/scopes/aflac-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Fortune 500
- Insurance
- Supplemental Insurance
- Employee Benefits
- Claims
- Enrollment
- Policy Administration
- Enterprise Integration
token_urls:
- https://auth.enterprise-connect.aflac.com/oauth/token
---
