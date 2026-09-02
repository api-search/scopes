---
api_specs:
- filename: nthu-oauth-api-openapi.yml
  format: yaml
  label: NTHU Academic Information System OAuth 2.0 Service
  slug: nthu-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/nthu-oauth-api-openapi.yml
- filename: nthu-data-api.yaml
  format: yaml
  label: NTHU Data API
  slug: nthu-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/openapi/_original/nthu-data-api.yaml
authorization_urls:
- https://oauth.ccxp.nthu.edu.tw/v1.1/authorize.php
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Nthu Scopes
name_suffix: OAuth Scopes
note: Scope strings are National Tsing Hua University's, transcribed verbatim from the scope parameter documented in the university's OAuth interface manual; the descriptions are ours. Scopes are requested space-separated on /authorize.php and echoed back space-separated in the token response. Which scopes a client may actually request is decided per application by the data-owning unit.
overview: 'National Tsing Hua University publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the National Tsing Hua University API on a user''s behalf.


  Tokens are issued from https://oauth.ccxp.nthu.edu.tw/v1.1/token.php.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: National Tsing Hua University
provider_slug: nthu
schemes:
- flows:
  - authorizationUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/authorize.php
    flow: authorizationCode
    tokenUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/token.php
  name: nthuOAuth
  source: https://oauth.ccxp.nthu.edu.tw/v1.1/doc/
  x-operator: institution
scope_count: 6
scope_names:
- userid
- name
- email
- inschool
- cid
- lmsid
scopes:
- description: The NTHU Academic Information System account identifier.
  flows:
  - authorizationCode
  scope: userid
- description: The account holder's Chinese name; the resource endpoint also returns name_en.
  flows:
  - authorizationCode
  scope: name
- description: The account holder's institutional email address.
  flows:
  - authorizationCode
  scope: email
- description: Current affiliation status — true for employed, enrolled or reinstated accounts, false for departed, graduated, withdrawn or cross-institution visiting accounts.
  flows:
  - authorizationCode
  scope: inschool
- description: National identification number. The most sensitive field the service can release; governed by Taiwan's Personal Data Protection Act and released only on data-owner approval.
  flows:
  - authorizationCode
  scope: cid
- description: The account holder's learning-management-platform identifier.
  flows:
  - authorizationCode
  scope: lmsid
slug: nthu-scopes
source_filename: nthu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: https://oauth.ccxp.nthu.edu.tw/v1.1/doc/\nnote: >-\n  Scope strings are National Tsing Hua University's, transcribed verbatim from the scope parameter\n  documented in the university's OAuth interface manual; the descriptions are ours. Scopes are\n  requested space-separated on /authorize.php and echoed back space-separated in the token response.\n  Which scopes a client may actually request is decided per application by the data-owning unit.\nschemes:\n- name: nthuOAuth\n  x-operator: institution\n  source: https://oauth.ccxp.nthu.edu.tw/v1.1/doc/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/authorize.php\n    tokenUrl: https://oauth.ccxp.nthu.edu.tw/v1.1/token.php\nscopes:\n- scope: userid\n  description: The NTHU Academic Information System account identifier.\n  sensitivity: identifier\n  flows: [authorizationCode]\n- scope: name\n  description: The account holder's Chinese\
  \ name; the resource endpoint also returns name_en.\n  sensitivity: personal\n  flows: [authorizationCode]\n- scope: email\n  description: The account holder's institutional email address.\n  sensitivity: personal\n  flows: [authorizationCode]\n- scope: inschool\n  description: >-\n    Current affiliation status — true for employed, enrolled or reinstated accounts, false for\n    departed, graduated, withdrawn or cross-institution visiting accounts.\n  sensitivity: affiliation\n  flows: [authorizationCode]\n- scope: cid\n  description: >-\n    National identification number. The most sensitive field the service can release; governed by\n    Taiwan's Personal Data Protection Act and released only on data-owner approval.\n  sensitivity: national_id\n  flows: [authorizationCode]\n- scope: lmsid\n  description: The account holder's learning-management-platform identifier.\n  sensitivity: identifier\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nthu/refs/heads/main/scopes/nthu-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Education
- Higher Education
- University
- Taiwan
- Public Research University
- Identity
- Authentication
- Open Data
- Campus
- Course Catalog
- Research Repository
- Library
token_urls:
- https://oauth.ccxp.nthu.edu.tw/v1.1/token.php
---
