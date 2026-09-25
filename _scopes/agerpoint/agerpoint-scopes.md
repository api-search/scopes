---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agerpoint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agerpoint uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agerpoint
provider_slug: agerpoint
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agerpoint-scopes
source_filename: agerpoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://agerpoint.us.auth0.com/.well-known/openid-configuration\napi: Agerpoint Cloud API\ndocs: null\nsummary: >-\n  The only scope list Agerpoint publishes anywhere is the OIDC scope set advertised by its Auth0\n  authorization server. These are identity scopes, not Agerpoint Cloud API permissions. Auth0 resource\n  servers carry their own per-API scopes, but Agerpoint does not publish the scope reference for the\n  https://cloudapi.agerpoint.com audience and there is no OpenAPI or RFC 9728 protected-resource document\n  from which to derive it, so the API's authorization model is not publicly knowable.\nresource_server_scopes_published: false\nresource_server_audience: https://cloudapi.agerpoint.com\nscopes:\n- name: openid\n  description: Issue an OpenID Connect ID token for the authenticated subject.\n  kind: oidc\n- name: profile\n  description: Basic profile claims (name, nickname, picture, created_at).\n  kind: oidc\n\
  - name: email\n  description: Email address claim.\n  kind: oidc\n- name: email_verified\n  description: Email verification status claim.\n  kind: oidc\n- name: offline_access\n  description: Issue a refresh token for long-lived access.\n  kind: oidc\n- name: name\n  description: Full name claim.\n  kind: oidc\n- name: given_name\n  description: Given name claim.\n  kind: oidc\n- name: family_name\n  description: Family name claim.\n  kind: oidc\n- name: nickname\n  description: Nickname claim.\n  kind: oidc\n- name: picture\n  description: Profile picture URL claim.\n  kind: oidc\n- name: created_at\n  description: Account creation timestamp claim.\n  kind: oidc\n- name: identities\n  description: Linked identity-provider identities claim.\n  kind: oidc\n- name: phone\n  description: Phone number claim.\n  kind: oidc\n- name: address\n  description: Address claim.\n  kind: oidc\nscope_count: 14\ngaps:\n- >-\n  Agerpoint Cloud API scopes (the permissions that actually gate /api/Captures,\
  \ /api/Projects,\n  /api/PipelineJobs and the rest) are not published. Recovering them would require an authenticated\n  token introspection against the tenant, which this pipeline does not perform.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agerpoint/refs/heads/main/scopes/agerpoint-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Agriculture
- Geospatial
- Remote Sensing
- Digital Twin
- LiDAR
- Point Cloud
- Carbon Measurement
- Forestry
- Machine Learning
- Spatial Analytics
- Company
token_urls: []
---
