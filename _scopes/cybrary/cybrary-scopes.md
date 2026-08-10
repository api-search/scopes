---
api_specs:
- filename: cybrary-completions-api-openapi.yml
  format: yaml
  label: Cybrary Completions API
  slug: cybrary-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybrary/refs/heads/main/openapi/cybrary-completions-api-openapi.yml
authorization_urls: []
description: ''
docs: https://help.cybrary.it/completions-export-integration
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cybrary Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cybrary publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cybrary API on a user''s behalf.


  Tokens are issued from https://app.cybrary.it/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cybrary
provider_slug: cybrary
schemes:
- description: OAuth 2.0 client credentials. Credentials are issued by Cybrary to the customer organization; client authentication is sent as a HTTP Basic Authorization header.
  flows:
  - flow: clientCredentials
    tokenUrl: https://app.cybrary.it/auth/oauth/token
  name: oauth2
  source: openapi/cybrary-completions-export-openapi.yml
scope_count: 1
scope_names:
- use-integrations
scopes:
- description: Access the Cybrary integrations APIs, including the completions export.
  flows:
  - clientCredentials
  scope: use-integrations
slug: cybrary-scopes
source_filename: cybrary-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://help.cybrary.it/completions-export-integration\ndocs: https://help.cybrary.it/completions-export-integration\nderived_from: openapi/cybrary-completions-export-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/cybrary-completions-export-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.cybrary.it/auth/oauth/token\n  description: OAuth 2.0 client credentials. Credentials are issued by Cybrary to the customer\n    organization; client authentication is sent as a HTTP Basic Authorization header.\nscopes:\n- scope: use-integrations\n  description: Access the Cybrary integrations APIs, including the completions export.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cybrary-completions-export-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybrary/refs/heads/main/scopes/cybrary-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Company
- Cybersecurity
- Training
- Education
- Learning Management
- Certification
- Workforce Development
- xAPI
- SCIM
- Security Awareness
token_urls:
- https://app.cybrary.it/auth/oauth/token
---
