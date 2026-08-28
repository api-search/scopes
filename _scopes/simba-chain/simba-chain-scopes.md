---
api_specs:
- filename: simba-chain-member-service-openapi.json
  format: json
  label: SIMBA Blocks Member Service API
  slug: simba-chain-member-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/openapi/simba-chain-member-service-openapi.json
- filename: simba-chain-member-service-validator-openapi.json
  format: json
  label: SIMBA Blocks Authentication Service API
  slug: simba-chain-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/openapi/simba-chain-member-service-validator-openapi.json
authorization_urls:
- https://blocks.simbachain.com/api/member-service-validator/oauth/authorize
description: 'SIMBA does NOT use OAuth scopes to express API authorization. The OpenAPI declares an authorizationCode flow with an EMPTY scopes map, and the authorization server advertises only the three standard OIDC identity scopes. All real authorization is carried by SIMBA''s own role-and-permission model, resolved per identity at GET /identity/{simba_id}/permissions/ and enforced by OPA middleware inside the platform (Blocks v24.1.1: "Implemented OPA middleware AuthZ"). An integrator sizing least-privilege access should read Roles and Permissions, not scopes.'
docs: https://docs.simbachain.com/documentation/simba-build/managing-an-organization/user-roles-and-permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Simba Chain Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SIMBA Chain uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://blocks.simbachain.com/api/member-service-validator/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SIMBA Chain
provider_slug: simba-chain
schemes:
- flows:
  - authorizationUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/authorize
    flow: authorizationCode
    scopes_declared_in_spec: 0
    tokenUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/token
  name: OAuth2AuthorizationCodeBearer
  source: openapi/simba-chain-member-service-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: simba-chain-scopes
source_filename: simba-chain-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  Baseline derived by 0-working/derive-oauth-scopes.py from\n  openapi/simba-chain-member-service-openapi.json, then upgraded from the provider's own live OpenID\n  Connect discovery document at\n  https://blocks.simbachain.com/api/member-service-validator/oauth/.well-known/openid-configuration\n  (HTTP 200, fetched 2026-08-27, saved verbatim to well-known/simba-chain-openid-configuration.json)\n  and from https://docs.simbachain.com/documentation/getting-started/obtaining-api-keys and\n  /simba-build/managing-an-organization/user-roles-and-permissions\ndocs: https://docs.simbachain.com/documentation/simba-build/managing-an-organization/user-roles-and-permissions\ndescription: >-\n  SIMBA does NOT use OAuth scopes to express API authorization. The OpenAPI declares an\n  authorizationCode flow with an EMPTY scopes map, and the authorization server advertises only the\n  three standard OIDC identity scopes. All real authorization\
  \ is carried by SIMBA's own\n  role-and-permission model, resolved per identity at\n  GET /identity/{simba_id}/permissions/ and enforced by OPA middleware inside the platform\n  (Blocks v24.1.1: \"Implemented OPA middleware AuthZ\"). An integrator sizing least-privilege access\n  should read Roles and Permissions, not scopes.\nschemes:\n  - name: OAuth2AuthorizationCodeBearer\n    source: openapi/simba-chain-member-service-openapi.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/authorize\n        tokenUrl: https://blocks.simbachain.com/api/member-service-validator/oauth/token\n        scopes_declared_in_spec: 0\ngrant_types_supported: [authorization_code, refresh_token, client_credentials]\ncode_challenge_methods_supported: [S256]\nscopes:\n  - name: openid\n    type: oidc-identity\n    description: Standard OpenID Connect scope requesting an ID token.\n    source: scopes_supported in the OIDC\
  \ discovery document.\n  - name: email\n    type: oidc-identity\n    description: Releases the email and email_verified claims.\n    source: scopes_supported in the OIDC discovery document.\n  - name: profile\n    type: oidc-identity\n    description: Releases the profile claims (first_name, last_name, name).\n    source: scopes_supported in the OIDC discovery document.\nclaims_supported:\n  - sub\n  - simba-id\n  - identity-urn\n  - simba_id\n  - identity_urn\n  - email\n  - email_verified\n  - first_name\n  - last_name\n  - name\n  - exp\n  - iat\n  - jti\n  - iss\n  - aud\n  - azp\n  - auth-flow\n  - auth-time\n  - typ\n  - fingerprint\n  - scope\nauthorization_model:\n  mechanism: roles and permissions (RBAC with attribute-scoped permissions), not OAuth scopes\n  permission_shape:\n    fields: [name, description, service, resource, action, is_org_scoped, resource_attributes, urls, effect]\n    note: >-\n      A Permission is a service/resource/action triple with an allow-or-deny `effect`,\
  \ optional\n      resource_attributes and the URL patterns it governs — closer to a policy statement than a scope.\n  role_kinds: [global, org-scoped, domain-scoped, custom]\n  role_inheritance: true\n  lookup_operations:\n    - get_permissions_permissions__get\n    - get_permission_permissions__permission_id__get\n    - get_identity_permissions_by_simba_id_identity__simba_id__permissions__get\n    - get_identities_permissions_identity_permissions__get\n    - get_roles_roles__get\n    - get_org_scoped_roles_organisations__organisation_name__roles__get\n  assignment_operations:\n    - update_organisation_user_account_roles_organisations__organisation_name__users__user_account_id__roles__put\n    - add_organisation_user_account_roles_organisations__organisation_name__users__user_account_id__roles_add__post\n    - remove_organisation_user_account_roles_organisations__organisation_name__users__user_account_id__roles_remove__delete\n    - update_client_credential_roles_organisations__organisation_name__client_credentials__client_id__roles__put\n\
  \    - update_device_app_roles_organisations__organisation_name__device_apps__device_app_name__roles__put\n  enforcement: OPA middleware (Open Policy Agent) inside the Blocks platform\n  docs: https://docs.simbachain.com/documentation/simba-build/managing-an-organization/user-roles-and-permissions\napplication_level_permissions:\n  note: >-\n    The dynamic contract API adds a second, separate authorization layer: a \"permissioned application\"\n    checks a remote user's group against the method being called, which is what error codes 2001-2010\n    report (NO_PERMISSIONS, NO_USER, METHOD_ACCESS_DENIED, WRITE_BLOCKCHAIN_DENIED, and so on). See\n    errors/simba-chain-problem-types.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simba-chain/refs/heads/main/scopes/simba-chain-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Blockchain
- Supply Chain
- Traceability
- Digital Product Passport
- Smart Contracts
- Identity
- Verifiable Credentials
- Defense
- Government
- Data Management
token_urls:
- https://blocks.simbachain.com/api/member-service-validator/oauth/token
---
