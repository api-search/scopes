---
api_specs:
- filename: covatic-audience-builder-openapi.yml
  format: yaml
  label: Covatic Audience Builder API
  slug: covatic-audience-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/openapi/covatic-audience-builder-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Covatic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Covatic uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Covatic
provider_slug: covatic
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: covatic-scopes
source_filename: covatic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  The Covatic Audience Builder OpenAPI declares no oauth2 securityScheme and therefore\n  no per-operation scopes — every protected operation carries a bare HTTP Bearer\n  requirement. The only published scope vocabulary for Covatic is the standard OIDC set\n  advertised by its AWS Cognito user pool's discovery document. There is no Covatic\n  resource-server scope namespace (no `audiences:read`, `campaigns:write`, or similar)\n  in anything public.\nscheme: openIdConnect\nissuer: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_mQWqhJueg\nauthorization_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/authorize\ntoken_endpoint: https://clienttoolsapi.auth.eu-west-2.amazoncognito.com/oauth2/token\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OIDC scope; requests\
  \ an ID token for the authenticated Covatic platform user.\n  source: openid-configuration.scopes_supported\n- name: email\n  description: Releases the user's email address claim.\n  source: openid-configuration.scopes_supported\n- name: phone\n  description: Releases the user's phone number claim.\n  source: openid-configuration.scopes_supported\n- name: profile\n  description: Releases standard profile claims for the user.\n  source: openid-configuration.scopes_supported\nresource_server_scopes:\n  declared: false\n  note: >-\n    Cognito resource servers can define custom scopes (e.g. `covatic/campaigns.read`)\n    and they would appear in `scopes_supported`. None do, so authorization inside the\n    API is enforced by role and tenant (client_id) rather than by OAuth scope.\nauthorization_notes: >-\n  Coarse-grained access is managed through company/client association and roles —\n  /api/v1/user/create-users-with-roles, /api/v1/user/update-user-association,\n  /api/v1/user/clients/default/{default_client_id}.\
  \ The role names are not published.\ngaps_for_the_provider:\n- Define a Cognito resource server with read/write scopes per resource family\n  (profiles, traits, campaigns, users, company) so tokens can be least-privilege.\n- Declare an `oauth2` or `openIdConnect` securityScheme in the OpenAPI and attach\n  scopes per operation, instead of a bare HTTPBearer.\ncross_links:\n  authentication: authentication/covatic-authentication.yml\n  openid_configuration: well-known/covatic-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covatic/refs/heads/main/scopes/covatic-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising Technology
- AdTech
- Audience Intelligence
- Data Management Platform
- Connected TV
- Privacy
- On-Device Processing
- Attribution
- Audio
- Campaigns
- Retargeting
- Publishing
- Broadcasting
- Media
- B Corp
- United Kingdom
token_urls: []
---
