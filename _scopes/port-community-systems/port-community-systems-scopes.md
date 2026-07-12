---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Port Community Systems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Port Community Systems publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Port Community Systems API on a user''s behalf.


  Tokens are issued from https://auth.portbase.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Port Community Systems
provider_slug: port-community-systems
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.portbase.com/oauth2/token
  name: oauth2
  source: openapi/portbase-port-community-openapi.yml
scope_count: 4
scope_names:
- customs.write
- manifests.write
- vessel-calls.read
- vessel-calls.write
scopes:
- description: Submit customs declarations
  flows:
  - clientCredentials
  scope: customs.write
- description: Submit cargo manifests
  flows:
  - clientCredentials
  scope: manifests.write
- description: Read vessel call data
  flows:
  - clientCredentials
  scope: vessel-calls.read
- description: Submit and update vessel calls
  flows:
  - clientCredentials
  scope: vessel-calls.write
slug: port-community-systems-scopes
source_filename: port-community-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/portbase-port-community-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/portbase-port-community-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.portbase.com/oauth2/token\nscopes:\n- scope: customs.write\n  description: Submit customs declarations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/portbase-port-community-openapi.yml\n- scope: manifests.write\n  description: Submit cargo manifests\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/portbase-port-community-openapi.yml\n- scope: vessel-calls.read\n  description: Read vessel call data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/portbase-port-community-openapi.yml\n- scope: vessel-calls.write\n  description: Submit and update vessel calls\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/portbase-port-community-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/scopes/port-community-systems-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Maritime
- Port
- Logistics
- Customs
- Cargo
- Shipping
token_urls:
- https://auth.portbase.com/oauth2/token
---
