---
authorization_urls: []
description: ''
docs: https://platform.relativity.com/RelativityOne/Content/REST_API/REST_API_authentication.htm
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Relativity Scopes
name_suffix: OAuth Scopes
note: Relativity does not publish granular OAuth permission scopes; the OAuth2 client Scopes property cannot be set by users (defaults cover only id_token/access_token/refresh_token per flow), and API access is governed by the client's assigned context user and Relativity permissions (https://platform.relativity.com/RelativityOne/Content/BD_Identity/OAuth2_Client_Manager__REST_.htm).
overview: 'Relativity publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Relativity API on a user''s behalf.


  Tokens are issued from https://auth.relone.preview.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Relativity
provider_slug: relativity
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.relone.preview.com/oauth/token
  name: oauth2
  source: openapi/relativity-glacier-openapi.yml
scope_count: 1
scope_names:
- SystemUserInfo
scopes:
- description: The only scope value shown in Relativity's documented OAuth2 client credentials token request (grant_type=client_credentials&scope=SystemUserInfo) against the /Relativity/Identity/connect/token endpoint; no description or additional permission scopes are published.
  flows: []
  scope: SystemUserInfo
slug: relativity-scopes
source_filename: relativity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/relativity-glacier-openapi.yml\ndocs: https://platform.relativity.com/RelativityOne/Content/REST_API/REST_API_authentication.htm\nnote: Relativity does not publish granular OAuth permission scopes; the OAuth2 client\n  Scopes property cannot be set by users (defaults cover only id_token/access_token/refresh_token\n  per flow), and API access is governed by the client's assigned context user and\n  Relativity permissions (https://platform.relativity.com/RelativityOne/Content/BD_Identity/OAuth2_Client_Manager__REST_.htm).\nschemes:\n- name: oauth2\n  source: openapi/relativity-glacier-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.relone.preview.com/oauth/token\nscopes:\n- scope: SystemUserInfo\n  description: The only scope value shown in Relativity's documented OAuth2 client\n    credentials token request (grant_type=client_credentials&scope=SystemUserInfo)\n    against the /Relativity/Identity/connect/token\
  \ endpoint; no description or additional\n    permission scopes are published.\n  sources:\n  - https://platform.relativity.com/RelativityOne/Content/REST_API/REST_API_authentication.htm\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/scopes/relativity-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- eDiscovery
- Legal
- Document Review
- Legal Technology
- Data Processing
- AI Review
- Litigation
- Compliance
token_urls:
- https://auth.relone.preview.com/oauth/token
---
