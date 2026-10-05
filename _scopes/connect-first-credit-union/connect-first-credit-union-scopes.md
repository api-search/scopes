---
authorization_urls: []
description: ''
docs: ''
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: searched
name: Connect First Credit Union Scopes
name_suffix: OAuth Scopes
note: The only OAuth scopes advertised are the two standard OIDC scopes exposed by Umbraco member authentication. No banking/data-access scopes exist; there is no public developer authorization surface.
overview: 'connectFirst Credit Union publishes 2 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the connectFirst Credit Union API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: connectFirst Credit Union
provider_slug: connect-first-credit-union
schemes: []
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: Standard OpenID Connect scope requesting an ID token for the member.
  flows: []
  scope: openid
- description: Requests a refresh token so the member session can be renewed without re-authentication.
  flows: []
  scope: offline_access
slug: connect-first-credit-union-scopes
source_filename: connect-first-credit-union-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.connectfirstcu.com/.well-known/openid-configuration\nnote: >-\n  The only OAuth scopes advertised are the two standard OIDC scopes exposed by\n  Umbraco member authentication. No banking/data-access scopes exist; there is no\n  public developer authorization surface.\nissuer: https://www.connectfirstcu.com/\nflow: authorization_code\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token for the member.\n  standard: true\n- name: offline_access\n  description: Requests a refresh token so the member session can be renewed without re-authentication.\n  standard: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connect-first-credit-union/refs/heads/main/scopes/connect-first-credit-union-scopes.yml
summary_line: 2 scopes · authorization_code
tags:
- Financial Services
- Banking
- Canada
- Credit Union
- Alberta
- Cooperative
token_bound: false
token_urls: []
---
