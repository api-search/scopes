---
api_specs:
- filename: medidata-rave-openapi.yml
  format: yaml
  label: Medidata Rave EDC API
  slug: medidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/openapi/medidata-rave-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Medidata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'medidata publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the medidata API on a user''s behalf.


  Tokens are issued from https://identity.medidata.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: medidata
provider_slug: medidata
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://identity.medidata.com/connect/token
  name: OAuth2
  source: openapi/medidata-rave-openapi.yml
scope_count: 2
scope_names:
- rave.read
- rave.write
scopes:
- description: Read access to Rave study data
  flows:
  - clientCredentials
  scope: rave.read
- description: Write access to Rave study data
  flows:
  - clientCredentials
  scope: rave.write
slug: medidata-scopes
source_filename: medidata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/medidata-rave-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/medidata-rave-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.medidata.com/connect/token\nscopes:\n- scope: rave.read\n  description: Read access to Rave study data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/medidata-rave-openapi.yml\n- scope: rave.write\n  description: Write access to Rave study data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/medidata-rave-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medidata/refs/heads/main/scopes/medidata-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- https://identity.medidata.com/connect/token
---
