---
authorization_urls: []
description: 'OAuth scopes Bloomberg actually advertises in its published authorization-server metadata. There is no public scope reference page — these are read verbatim from scopes_supported. Note the shape of the finding: every scope Bloomberg publishes is an IDENTITY scope. The Data License data-plane entitlements (which catalogs, datasets and fields a client may read) are provisioned per contract in the Bloomberg Enterprise Console and are NOT expressed as OAuth scopes, so an agent cannot reason about its own data authority from the token.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bloomberg Data Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bloomberg Data uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bloomberg Data
provider_slug: bloomberg-data
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: bloomberg-data-scopes
source_filename: bloomberg-data-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Bloomberg Data\nproviderId: bloomberg-data\ngenerated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://bsso.blpprofessional.com/.well-known/oauth-authorization-server (200) and\n  https://www.bloomberg.com/.well-known/openid-configuration (200)\ndocs: null\ndescription: >-\n  OAuth scopes Bloomberg actually advertises in its published authorization-server metadata.\n  There is no public scope reference page — these are read verbatim from scopes_supported.\n  Note the shape of the finding: every scope Bloomberg publishes is an IDENTITY scope. The\n  Data License data-plane entitlements (which catalogs, datasets and fields a client may\n  read) are provisioned per contract in the Bloomberg Enterprise Console and are NOT\n  expressed as OAuth scopes, so an agent cannot reason about its own data authority from\n  the token.\nauthorization_servers:\n  - issuer: https://bsso.blpprofessional.com\n\
  \    applies_to:\n      - Bloomberg Data License API\n    scopes:\n      - name: openid\n        description: OpenID Connect — request an ID token.\n      - name: profile\n        description: Standard OIDC profile claims.\n      - name: email\n        description: Standard OIDC email claim.\n      - name: name\n        description: Subject display name claim.\n      - name: firmid\n        description: Bloomberg firm identifier for the authenticated principal.\n      - name: employeeid\n        description: Bloomberg employee identifier for the authenticated principal.\n      - name: bbprofile\n        description: Bloomberg profile claim set.\n  - issuer: https://www.bloomberg.com\n    applies_to:\n      - bloomberg.com account identity (not the Data License data plane)\n    scopes:\n      - name: openid\n        description: OpenID Connect — request an ID token.\n      - name: user\n        description: bloomberg.com user profile.\n      - name: entitlements\n        description: bloomberg.com\
  \ subscription entitlements.\ngrant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:saml2-bearer\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:openid:params:grant-type:ciba\n  - urn:pingidentity.com:oauth2:grant_type:validate_bearer\ntoken_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\ngaps:\n  - No published scope-to-operation mapping; data entitlements are contractual, not scoped.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-data/refs/heads/main/scopes/bloomberg-data-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Financial-Services
- Market Data
- News
- Real-Time Data
- Trading
token_urls: []
---
