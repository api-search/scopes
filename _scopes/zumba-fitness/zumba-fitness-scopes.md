---
authorization_urls:
- https://www.zumba.com/oauth/authorize
description: ''
docs: https://www.zumba.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Zumba Fitness Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zumba Fitness publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zumba Fitness API on a user''s behalf.


  Tokens are issued from https://www.zumba.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zumba Fitness
provider_slug: zumba-fitness
schemes: []
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: Required to initiate an OpenID Connect flow; issues an ID token identifying the end user (sub claim).
  flows: []
  scope: openid
- description: Grants access to the user's email and email_verified claims.
  flows: []
  scope: email
- description: Grants access to basic profile claims (given_name, family_name, pid).
  flows: []
  scope: profile
slug: zumba-fitness-scopes
source_filename: zumba-fitness-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.zumba.com/.well-known/openid-configuration (scopes_supported)\ndocs: https://www.zumba.com/.well-known/openid-configuration\nissuer: https://www.zumba.com\nauthorization_endpoint: https://www.zumba.com/oauth/authorize\ntoken_endpoint: https://www.zumba.com/oauth/access_token\nscopes:\n- name: openid\n  description: Required to initiate an OpenID Connect flow; issues an ID token identifying the end user (sub claim).\n- name: email\n  description: Grants access to the user's email and email_verified claims.\n- name: profile\n  description: Grants access to basic profile claims (given_name, family_name, pid).\nclaims_supported:\n- sub\n- iss\n- aud\n- iat\n- exp\n- auth_time\n- nonce\n- email\n- email_verified\n- given_name\n- family_name\n- pid\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zumba-fitness/refs/heads/main/scopes/zumba-fitness-scopes.yml
summary_line: 3 scopes
tags:
- Company
token_bound: false
token_urls:
- https://www.zumba.com/oauth/access_token
---
