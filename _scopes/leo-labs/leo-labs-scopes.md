---
api_specs:
- filename: leo-labs-platform-openapi.yml
  format: yaml
  label: LeoLabs Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leo-labs/refs/heads/main/openapi/leo-labs-platform-openapi.yml
authorization_urls: []
description: ''
docs: https://auth.leolabs.space/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Leo Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LeoLabs uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LeoLabs
provider_slug: leo-labs
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: leo-labs-scopes
source_filename: leo-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.leolabs.space/.well-known/openid-configuration\ndocs: https://auth.leolabs.space/.well-known/openid-configuration\napplies_to: LeoLabs Platform / documentation interactive sign-in (Okta org authorization\n  server). The v1 Platform API itself is authenticated with a LeoLabs access key + secret\n  key pair and exposes NO OAuth scope surface — see authentication/leo-labs-authentication.yml.\nauthorization_server:\n  provider: Okta\n  issuer: https://auth.leolabs.space\n  authorization_endpoint: https://auth.leolabs.space/oauth2/v1/authorize\n  token_endpoint: https://auth.leolabs.space/oauth2/v1/token\n  userinfo_endpoint: https://auth.leolabs.space/oauth2/v1/userinfo\n  jwks_uri: https://auth.leolabs.space/oauth2/v1/keys\n  registration_endpoint: https://auth.leolabs.space/oauth2/v1/clients\n  pkce_methods:\n  - S256\n  grant_types:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n\
  \  - urn:openid:params:grant-type:ciba\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\nscopes:\n- name: openid\n  description: Required for OpenID Connect; requests an ID token.\n- name: email\n  description: The user's email address and its verification status.\n- name: profile\n  description: Default profile claims for the user.\n- name: address\n  description: The user's postal address claim.\n- name: phone\n  description: The user's phone number claim.\n- name: offline_access\n  description: Issues a refresh token so the client can renew access without the user present.\n- name: groups\n  description: The Okta groups the user belongs to.\nnotes:\n- These are the standard OpenID Connect and Okta org-authorization-server scopes advertised\n  by LeoLabs' discovery document. LeoLabs does not publish product-specific API scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leo-labs/refs/heads/main/scopes/leo-labs-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Space
- Satellites
- Space Situational Awareness
- Space Traffic Management
- Orbital Data
- Radar
- Aerospace
- Defense
- Geospatial
token_urls: []
---
