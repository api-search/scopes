---
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Swift Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SWIFT publishes 2 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SWIFT API on a user''s behalf.


  Tokens are issued from https://api.swift.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SWIFT
provider_slug: swift
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  source: openapi/swift-swiftref-api-openapi.yml
scope_count: 2
scope_names:
- urn:swiftref:external
- urn:swiftref:internal
scopes:
- description: External customer access to SwiftRef data
  flows:
  - password
  scope: urn:swiftref:external
- description: Internal payment validation access
  flows:
  - password
  scope: urn:swiftref:internal
slug: swift-scopes
source_filename: swift-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swift-swiftref-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/swift-swiftref-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\nscopes:\n- scope: urn:swiftref:external\n  description: External customer access to SwiftRef data\n  flows:\n  - password\n  sources:\n  - openapi/swift-swiftref-api-openapi.yml\n- scope: urn:swiftref:internal\n  description: Internal payment validation access\n  flows:\n  - password\n  sources:\n  - openapi/swift-swiftref-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift/refs/heads/main/scopes/swift-scopes.yml
summary_line: 2 scopes · password
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
token_urls:
- https://api.swift.com/oauth2/v1/token
---
