---
authorization_urls:
- https://{hostname}:{port}/psft/oauth/authorize
description: ''
docs: https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Peoplesoft Scopes
name_suffix: OAuth Scopes
note: PeopleSoft OAuth 2.0 (PeopleTools 8.58+) publishes no scope catalog; authorization is enforced by PeopleSoft permission lists and roles tied to the user ID in the token's sub claim, with any scopes defined per deployment in the external identity provider (see https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html).
overview: 'PeopleSoft uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{hostname}:{port}/psft/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PeopleSoft
provider_slug: peoplesoft
schemes:
- flows:
  - authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{hostname}:{port}/psft/oauth/token
  name: oauth2
  source: openapi/application-services-framework.yml
- flows:
  - authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{hostname}:{port}/psft/oauth/token
  name: oauth2
  source: openapi/rest-api.yml
scope_count: 0
scope_names: []
scopes: []
slug: peoplesoft-scopes
source_filename: peoplesoft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/application-services-framework.yml, openapi/rest-api.yml\ndocs: https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html\nnote: PeopleSoft OAuth 2.0 (PeopleTools 8.58+) publishes no scope catalog; authorization\n  is enforced by PeopleSoft permission lists and roles tied to the user ID in the\n  token's sub claim, with any scopes defined per deployment in the external identity\n  provider (see https://docs.oracle.com/cd/F30998_01/pt858pbr2/eng/pt/tsec/concept_UnderstandingOAuth2_0.html).\nschemes:\n- name: oauth2\n  source: openapi/application-services-framework.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize\n    tokenUrl: https://{hostname}:{port}/psft/oauth/token\n- name: oauth2\n  source: openapi/rest-api.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{hostname}:{port}/psft/oauth/authorize\n\
  \    tokenUrl: https://{hostname}:{port}/psft/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/scopes/peoplesoft-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
token_urls:
- https://{hostname}:{port}/psft/oauth/token
---
