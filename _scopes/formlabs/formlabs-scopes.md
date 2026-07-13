---
api_specs:
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Printers
  slug: formlabs-web-api-printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Prints
  slug: formlabs-web-api-prints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Consumables
  slug: formlabs-web-api-consumables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Events
  slug: formlabs-web-api-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Groups
  slug: formlabs-web-api-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Formlabs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Formlabs publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Formlabs API on a user''s behalf.


  Tokens are issued from https://api.formlabs.com/developer/v1/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Formlabs
provider_slug: formlabs
schemes:
- description: OAuth 2.0 Client Credentials flow. Exchange a client_id and client_secret at the token endpoint for a Bearer access token valid for 24 hours, scoped to developer-api. The Formlabs identity provider also supports OpenID Connect for interactive sign-in via PreForm / Local API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.formlabs.com/developer/v1/o/token/
  name: OAuth2ClientCredentials
  source: openapi/formlabs-openapi.yml
scope_count: 1
scope_names:
- developer-api
scopes:
- description: Access the Formlabs Dashboard Developer API
  flows:
  - clientCredentials
  scope: developer-api
slug: formlabs-scopes
source_filename: formlabs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formlabs-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/formlabs-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.formlabs.com/developer/v1/o/token/\n  description: OAuth 2.0 Client Credentials flow. Exchange a client_id and client_secret at\n    the token endpoint for a Bearer access token valid for 24 hours, scoped to developer-api.\n    The Formlabs identity provider also supports OpenID Connect for interactive sign-in via\n    PreForm / Local API.\nscopes:\n- scope: developer-api\n  description: Access the Formlabs Dashboard Developer API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/formlabs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/scopes/formlabs-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- 3D Printing
- Additive Manufacturing
- SLA
- SLS
- Hardware
- Dashboard
token_urls:
- https://api.formlabs.com/developer/v1/o/token/
---
