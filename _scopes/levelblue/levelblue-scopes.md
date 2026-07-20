---
api_specs:
- filename: levelblue-usm-anywhere-openapi.yml
  format: yaml
  label: USM Anywhere API
  slug: usm-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levelblue/refs/heads/main/openapi/levelblue-usm-anywhere-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/user-management/api-clients
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Levelblue Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LevelBlue publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the LevelBlue API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LevelBlue
provider_slug: levelblue
schemes:
- bearerFormat: JWT
  name: bearerAuth
  note: The spec models the access token as an http/bearer scheme rather than an OAuth2 securityScheme, so no flows{} scopes map is declared. The scopes below are read from the documented /oauth/token success response.
  scheme: bearer
  source: openapi/levelblue-usm-anywhere-openapi.yml
  type: http
scope_count: 3
scope_names:
- trust
- read
- write
scopes:
- description: Present in the documented token response. LevelBlue does not publish a scope reference defining its effect.
  flows: []
  scope: trust
- description: Read access to USM Anywhere resources (alarms, events). Not separately documented.
  flows: []
  scope: read
- description: Write access to USM Anywhere resources (e.g. adding and removing alarm labels). Not separately documented.
  flows: []
  scope: write
slug: levelblue-scopes
source_filename: levelblue-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/levelblue-usm-anywhere-openapi.yml\ndocs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/user-management/api-clients\n\ngrant:\n  type: client_credentials\n  token_endpoint: https://your-subdomain.alienvault.cloud/api/2.0/oauth/token\n  client_authentication: http-basic (client ID as username, client secret as password)\n  token_format: JWT\n  expires_in: 899\n\nschemes:\n- name: bearerAuth\n  source: openapi/levelblue-usm-anywhere-openapi.yml\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: >-\n    The spec models the access token as an http/bearer scheme rather than an OAuth2\n    securityScheme, so no flows{} scopes map is declared. The scopes below are read from\n    the documented /oauth/token success response.\n\nscopes:\n- scope: trust\n  description: >-\n    Present in the documented token response. LevelBlue does not publish a scope\n    reference defining its effect.\n  sources:\
  \ ['openapi/levelblue-usm-anywhere-openapi.yml#POST /oauth/token (200 example)']\n- scope: read\n  description: >-\n    Read access to USM Anywhere resources (alarms, events). Not separately documented.\n  sources: ['openapi/levelblue-usm-anywhere-openapi.yml#POST /oauth/token (200 example)']\n- scope: write\n  description: >-\n    Write access to USM Anywhere resources (e.g. adding and removing alarm labels). Not\n    separately documented.\n  sources: ['openapi/levelblue-usm-anywhere-openapi.yml#POST /oauth/token (200 example)']\n\nauthorization_model:\n  note: >-\n    Effective API authorization is governed by the USM Anywhere role assigned to the API\n    client, not by requesting narrower scopes. Documented roles are Read-Only,\n    Investigator, Analyst and Manager; the API Clients page itself requires the Manager\n    role.\n  roles: [Read-Only, Investigator, Analyst, Manager]\n  source: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/user-management/api-clients\n\
  \ngaps:\n- >-\n    No scopes/permissions reference page is published. The three scope values above are\n    the literal contents of the `scope` field in the spec's own token-response example\n    (\"trust read write\") — they are not documented individually, and there is no\n    documented way to request a subset.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levelblue/refs/heads/main/scopes/levelblue-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Enterprise
- Cybersecurity
- Security
- Threat Intelligence
- Managed Security
- SIEM
- Threat Detection
- Incident Response
- Compliance
token_urls: []
---
