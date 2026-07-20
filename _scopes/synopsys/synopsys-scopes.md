---
api_specs:
- filename: synopsys-polaris-openapi.yml
  format: yaml
  label: Synopsys Polaris API
  slug: polaris
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-polaris-openapi.yml
- filename: cim-openapi.html
  format: yaml
  label: Synopsys Coverity REST API
  slug: coverity
  spec_type: OpenAPI
  url: https://documentation.blackduck.com/bundle/coverity-docs/page/cim-api-docs/openapi/cim-openapi.html
- filename: synopsys-cloud-openlink-openapi.yml
  format: yaml
  label: Synopsys Cloud OpenLink API
  slug: cloud-openlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-cloud-openlink-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Synopsys Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Synopsys publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Synopsys API on a user''s behalf.


  Tokens are issued from https://api.synopsys.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Synopsys
provider_slug: synopsys
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.synopsys.com/oauth/token
  name: oauth2
  source: openapi/synopsys-cloud-openlink-openapi.yml
scope_count: 1
scope_names:
- openlink
scopes:
- description: Access OpenLink API
  flows:
  - clientCredentials
  scope: openlink
slug: synopsys-scopes
source_filename: synopsys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synopsys-cloud-openlink-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/synopsys-cloud-openlink-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.synopsys.com/oauth/token\nscopes:\n- scope: openlink\n  description: Access OpenLink API\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/synopsys-cloud-openlink-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/scopes/synopsys-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Software Security
- Application Security Testing
- Static Analysis
- Software Composition Analysis
- EDA Tools
- Semiconductor Design
- Fortune 1000
token_urls:
- https://api.synopsys.com/oauth/token
---
