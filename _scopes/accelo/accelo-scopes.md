---
api_specs:
- filename: accelo-openapi.yml
  format: yaml
  label: Accelo REST API
  slug: accelo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-openapi.yml
authorization_urls:
- https://{deployment}.api.accelo.com/oauth2/v0/authorize
description: ''
docs: https://api.accelo.com/docs/#scope
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Accelo Scopes
name_suffix: OAuth Scopes
note: Accelo documents a scope template rather than a fixed scope list — read()/write() wrapping "all" or any API resource name (e.g. companies, contacts, staff); scope is optional and defaults to read(all) (https://api.accelo.com/docs/#scope).
overview: 'Accelo publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Accelo API on a user''s behalf.


  Tokens are issued from https://{deployment}.api.accelo.com/oauth2/v0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accelo
provider_slug: accelo
schemes:
- flows:
  - authorizationUrl: https://{deployment}.api.accelo.com/oauth2/v0/authorize
    flow: authorizationCode
    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token
  - flow: clientCredentials
    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token
  name: OAuth2
  source: openapi/accelo-openapi.yml
scope_count: 4
scope_names:
- read(all)
- write(all)
- read({resource})
- write({resource})
scopes:
- description: Read only access to all data the user owns or has access to.
  flows: []
  scope: read(all)
- description: Read and write access to all data the user owns or has access to.
  flows: []
  scope: write(all)
- description: Read only access to data related to the {resource} object, which may be any resource. Multiple resources may be concatenated, e.g. read(companies,contacts).
  flows: []
  scope: read({resource})
- description: Read and write access related to the resource specified. Multiple resources may be concatenated, e.g. write(companies,contacts).
  flows: []
  scope: write({resource})
slug: accelo-scopes
source_filename: accelo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/accelo-openapi.yml\ndocs: https://api.accelo.com/docs/#scope\nschemes:\n- name: OAuth2\n  source: openapi/accelo-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{deployment}.api.accelo.com/oauth2/v0/authorize\n    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token\n  - flow: clientCredentials\n    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token\nscopes:\n- scope: read(all)\n  description: Read only access to all data the user owns or has access to.\n  sources:\n  - https://api.accelo.com/docs/#scope\n- scope: write(all)\n  description: Read and write access to all data the user owns or has access to.\n  sources:\n  - https://api.accelo.com/docs/#scope\n- scope: read({resource})\n  description: Read only access to data related to the {resource} object, which\n    may be any resource. Multiple resources may be concatenated, e.g.\n    read(companies,contacts).\n\
  \  sources:\n  - https://api.accelo.com/docs/#scope\n- scope: write({resource})\n  description: Read and write access related to the resource specified. Multiple\n    resources may be concatenated, e.g. write(companies,contacts).\n  sources:\n  - https://api.accelo.com/docs/#scope\nnote: Accelo documents a scope template rather than a fixed scope list — read()/write()\n  wrapping \"all\" or any API resource name (e.g. companies, contacts, staff); scope\n  is optional and defaults to read(all) (https://api.accelo.com/docs/#scope).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/scopes/accelo-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Professional Services Automation
- Project Management
- CRM
- Time Tracking
- Invoicing
- Service Operations
token_urls:
- https://{deployment}.api.accelo.com/oauth2/v0/token
---
