---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Allianz Technology Standards Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allianz Technology Standards publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allianz Technology Standards API on a user''s behalf.


  Tokens are issued from https://standards.allianz.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allianz Technology Standards
provider_slug: allianz-technology-standards
schemes:
- description: OAuth2 client credentials for Allianz standards API
  flows:
  - flow: clientCredentials
    tokenUrl: https://standards.allianz.com/oauth2/token
  name: OAuth2
  source: openapi/allianz-technology-standards-compliance.yaml
scope_count: 2
scope_names:
- compliance:check
- standards:read
scopes:
- description: Run compliance checks
  flows:
  - clientCredentials
  scope: compliance:check
- description: Read technology standards
  flows:
  - clientCredentials
  scope: standards:read
slug: allianz-technology-standards-scopes
source_filename: allianz-technology-standards-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/allianz-technology-standards-compliance.yaml\nschemes:\n- name: OAuth2\n  source: openapi/allianz-technology-standards-compliance.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://standards.allianz.com/oauth2/token\n  description: OAuth2 client credentials for Allianz standards API\nscopes:\n- scope: compliance:check\n  description: Run compliance checks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-technology-standards-compliance.yaml\n- scope: standards:read\n  description: Read technology standards\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allianz-technology-standards-compliance.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-technology-standards/refs/heads/main/scopes/allianz-technology-standards-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Best Practices
- Enterprise Architecture
- Guidelines
- Software Development
- Technology Standards
- API Design
- OpenAPI
token_urls:
- https://standards.allianz.com/oauth2/token
---
