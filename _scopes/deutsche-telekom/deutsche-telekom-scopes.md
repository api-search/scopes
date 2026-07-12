---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Deutsche Telekom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deutsche Telekom publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deutsche Telekom API on a user''s behalf.


  Tokens are issued from https://example.com/auth/realms/realm//protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deutsche Telekom
provider_slug: deutsche-telekom
schemes:
- description: OAuth2 client_credentials flow
  flows:
  - flow: clientCredentials
    tokenUrl: https://example.com/auth/realms/realm//protocol/openid-connect/token
  name: OAuth2
  source: openapi/controlplane-rover-server-openapi.yml
scope_count: 13
scope_names:
- tardis:admin:all
- tardis:admin:obfuscated
- tardis:admin:read
- tardis:hub:all
- tardis:hub:obfuscated
- tardis:hub:read
- tardis:supervisor:read
- tardis:team:all
- tardis:team:obfuscated
- tardis:team:read
- tardis:user:all
- tardis:user:obfuscated
- tardis:user:read
scopes:
- description: Admin access to all resources
  flows:
  - clientCredentials
  scope: tardis:admin:all
- description: Admin obfuscated access to all resources
  flows:
  - clientCredentials
  scope: tardis:admin:obfuscated
- description: Admin read access to all resources
  flows:
  - clientCredentials
  scope: tardis:admin:read
- description: Access to all resources of a hub
  flows:
  - clientCredentials
  scope: tardis:hub:all
- description: Obfuscated access to all resources of a hub
  flows:
  - clientCredentials
  scope: tardis:hub:obfuscated
- description: Read access to all resources of a hub
  flows:
  - clientCredentials
  scope: tardis:hub:read
- description: (deprecated) Admin obfuscated access to all resources
  flows:
  - clientCredentials
  scope: tardis:supervisor:read
- description: Access to all resources of a team
  flows:
  - clientCredentials
  scope: tardis:team:all
- description: Obfuscated access to all resources of a team
  flows:
  - clientCredentials
  scope: tardis:team:obfuscated
- description: Read access to all resources of a team
  flows:
  - clientCredentials
  scope: tardis:team:read
- description: (deprecated) Access to all resources of a team
  flows:
  - clientCredentials
  scope: tardis:user:all
- description: (deprecated) Obfuscated access to all resources of a team
  flows:
  - clientCredentials
  scope: tardis:user:obfuscated
- description: (deprecated) Read access to all resources of a team
  flows:
  - clientCredentials
  scope: tardis:user:read
slug: deutsche-telekom-scopes
source_filename: deutsche-telekom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/controlplane-rover-server-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/controlplane-rover-server-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/auth/realms/realm//protocol/openid-connect/token\n  description: OAuth2 client_credentials flow\nscopes:\n- scope: tardis:admin:all\n  description: Admin access to all resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:admin:obfuscated\n  description: Admin obfuscated access to all resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:admin:read\n  description: Admin read access to all resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:hub:all\n  description: Access to all resources of a hub\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:hub:obfuscated\n  description: Obfuscated access to all resources of a hub\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:hub:read\n  description: Read access to all resources of a hub\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:supervisor:read\n  description: (deprecated) Admin obfuscated access to all resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:team:all\n  description: Access to all resources of a team\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:team:obfuscated\n  description: Obfuscated access to all resources of a team\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:team:read\n\
  \  description: Read access to all resources of a team\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:user:all\n  description: (deprecated) Access to all resources of a team\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:user:obfuscated\n  description: (deprecated) Obfuscated access to all resources of a team\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n- scope: tardis:user:read\n  description: (deprecated) Read access to all resources of a team\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/controlplane-rover-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-telekom/refs/heads/main/scopes/deutsche-telekom-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Telecommunications
- Telco
- Mobile Network Operator
- CPaaS
- Network API
- 5G
- Cloud
- Identity
- Number Verification
- Open Gateway
- CAMARA
- T-Systems
- T-Mobile
- Magenta
- MagentaBusiness
- API Gateway
- Open Source
- Germany
- Europe
token_urls:
- https://example.com/auth/realms/realm//protocol/openid-connect/token
---
