---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Atandt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AT&T publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AT&T API on a user''s behalf.


  Tokens are issued from https://devex-web.att.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AT&T
provider_slug: atandt
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://devex-web.att.com/oauth/token
  name: oauth2
  source: openapi/atandt-enterprise-connectivity-apis.yaml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.att.com/oauth/v4/token
  name: oauth2
  source: openapi/atandt-network-apis.yaml
scope_count: 2
scope_names:
- enterprise
- network
scopes:
- description: Access AT&T enterprise connectivity APIs
  flows:
  - clientCredentials
  scope: enterprise
- description: Access AT&T network APIs
  flows:
  - clientCredentials
  scope: network
slug: atandt-scopes
source_filename: atandt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/atandt-enterprise-connectivity-apis.yaml, openapi/atandt-network-apis.yaml\nschemes:\n- name: oauth2\n  source: openapi/atandt-enterprise-connectivity-apis.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://devex-web.att.com/oauth/token\n- name: oauth2\n  source: openapi/atandt-network-apis.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.att.com/oauth/v4/token\nscopes:\n- scope: enterprise\n  description: Access AT&T enterprise connectivity APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/atandt-enterprise-connectivity-apis.yaml\n- scope: network\n  description: Access AT&T network APIs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/atandt-network-apis.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atandt/refs/heads/main/scopes/atandt-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Fortune 100
- Telecommunications
- Fortune 100
- Wireless
- Wireline
- Broadband
- Enterprise
- 5G
- Network
token_urls:
- https://devex-web.att.com/oauth/token
- https://api.att.com/oauth/v4/token
---
