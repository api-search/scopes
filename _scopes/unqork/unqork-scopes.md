---
api_specs:
- filename: unqork-customer-api-openapi.yml
  format: yaml
  label: Unqork Customer API
  slug: unqork-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/openapi/unqork-customer-api-openapi.yml
authorization_urls: []
description: 'Unqork''s Customer API is OAuth 2.0, but it is NOT scope-based. The OpenAPI declares exactly one scope — the placeholder `none` with the description `N/A` — on both flows, and no operation requests a scope in its `security[]` requirement. Authorization is instead RBAC: what a token can do is decided by the Express or Creator roles bound to the credential that minted it, in Administration → API Access Management. This file records that honestly rather than presenting a one-entry placeholder list as a scope surface.'
docs: https://docs.unqork.io/docs/api-access-management
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: searched
name: Unqork Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Unqork publishes 1 OAuth 2.0 scope via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unqork API on a user''s behalf.


  Tokens are issued from https://{subdomain}.unqork.io/api/1.0/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unqork
provider_slug: unqork
schemes:
- applied: 'Globally — the document declares `security: [{OAuth2: []}]` at the root, so all 93 operations require a bearer token. No operation names a scope.'
  flows:
  - flow: clientCredentials
    rfc: RFC 6749 §1.3.4
    spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token
    tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token
  - caveat: The resource-owner password credentials grant is removed in OAuth 2.1 and discouraged by RFC 9700. Prefer clientCredentials.
    enabled_by_default: false
    enablement: Administration → Environment Administration → Unqork API → "Enable OAuth2 Password Grant". Once enabled, every Unqork user can exchange their platform username/password for an access token.
    flow: password
    rfc: RFC 6749 §1.3.3
    spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token
    tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token
  name: OAuth2
  source: openapi/unqork-customer-api-openapi.yml
  token_lifetime_seconds: 3600
scope_count: 1
scope_names:
- none
scopes:
- description: N/A
  flows:
  - clientCredentials
  - password
  scope: none
slug: unqork-scopes
source_filename: unqork-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: openapi/unqork-customer-api-openapi.yml\ndocs: https://docs.unqork.io/docs/api-access-management\ndescription: >-\n  Unqork's Customer API is OAuth 2.0, but it is NOT scope-based. The OpenAPI\n  declares exactly one scope — the placeholder `none` with the description `N/A` —\n  on both flows, and no operation requests a scope in its `security[]`\n  requirement. Authorization is instead RBAC: what a token can do is decided by\n  the Express or Creator roles bound to the credential that minted it, in\n  Administration → API Access Management. This file records that honestly rather\n  than presenting a one-entry placeholder list as a scope surface.\n\nauthorization_model: rbac\nscope_based: false\n\nschemes:\n  - name: OAuth2\n    source: openapi/unqork-customer-api-openapi.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token\n        spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token\n\
  \        rfc: RFC 6749 §1.3.4\n      - flow: password\n        tokenUrl: https://{subdomain}.unqork.io/api/1.0/oauth2/access_token\n        spec_tokenUrl: https://xyzfinancial.unqork.io/api/1.0/oauth2/access_token\n        rfc: RFC 6749 §1.3.3\n        enabled_by_default: false\n        enablement: >-\n          Administration → Environment Administration → Unqork API →\n          \"Enable OAuth2 Password Grant\". Once enabled, every Unqork user can\n          exchange their platform username/password for an access token.\n        caveat: >-\n          The resource-owner password credentials grant is removed in OAuth 2.1\n          and discouraged by RFC 9700. Prefer clientCredentials.\n    token_lifetime_seconds: 3600\n    applied: >-\n      Globally — the document declares `security: [{OAuth2: []}]` at the root, so\n      all 93 operations require a bearer token. No operation names a scope.\n\nscopes:\n  - scope: none\n    description: N/A\n    placeholder: true\n    flows: [clientCredentials,\
  \ password]\n    sources: [openapi/unqork-customer-api-openapi.yml]\n    note: >-\n      Declared in both flow `scopes` maps. It is a placeholder required by the\n      OpenAPI schema, not a grantable permission — requesting it confers nothing\n      and omitting it costs nothing.\n\npermission_model:\n  mechanism: Role-based access control (RBAC)\n  docs: https://docs.unqork.io/docs/api-access-management\n  surfaces:\n    - name: Express\n      credential_requires: At least one Express Role\n      role_admin: https://docs.unqork.io/docs/express-role-administration\n      permissions_reference: https://docs.unqork.io/docs/express-permissions\n      governs: End-user-facing resources — submissions, workflow execution\n    - name: Creator\n      credential_requires: At least one Creator Role\n      role_admin: https://docs.unqork.io/docs/creator-role-administration\n      permissions_reference: https://docs.unqork.io/docs/creator-permissions\n      governs: Design-time resources — modules,\
  \ applications, promotions, credentials\n  per_operation_authorization: >-\n    Operation descriptions in the OpenAPI carry an \"### Authorization Required:\"\n    line naming the role needed (e.g. \"Designer Administrator\"). That prose is the\n    de-facto permission reference for the API — there is no machine-readable\n    permission map.\n  least_privilege: >-\n    Because there are no scopes, a token cannot be narrowed at request time.\n    Least privilege must be provisioned: create a credential bound to the\n    narrowest role that satisfies the job, one credential per integration.\n  credential_binding:\n    expiration_days: {min: 1, max: 730, ui_default: 90}\n    lockout: Five failed client-secret attempts lock the credential for 30 minutes\n    revocable: true (Creator credentials)\n    statuses: [ACTIVE, EXPIRES SOON, EXPIRED, REVOKED, LOCKED]\n\ndiscovery:\n  oauth_authorization_server_metadata: false\n  note: >-\n    No RFC 8414 /.well-known/oauth-authorization-server document\
  \ is served on any\n    Unqork host, so the token endpoint and supported grants are discoverable only\n    from the OpenAPI securityScheme description and the docs.\n\nrelated:\n  authentication: authentication/unqork-authentication.yml\n  conventions: conventions/unqork-conventions.yml\n  well_known: well-known/unqork-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unqork/refs/heads/main/scopes/unqork-scopes.yml
summary_line: 1 scope · clientCredentials/password
tags:
- Company
- No-Code
- Low-Code
- Application Development
- Enterprise Software
- Platform-as-a-Service
- Workflows
- Financial-Services
- Insurance
- Government
- Application Modernization
token_urls:
- https://{subdomain}.unqork.io/api/1.0/oauth2/access_token
---
