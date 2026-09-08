---
api_specs:
- filename: express-gateway-apps-api-openapi.yml
  format: yaml
  label: Express Gateway Apps API
  slug: express-gateway-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-apps-api-openapi.yml
- filename: express-gateway-credentials-api-openapi.yml
  format: yaml
  label: Express Gateway Credentials API
  slug: express-gateway-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-credentials-api-openapi.yml
- filename: express-gateway-scopes-api-openapi.yml
  format: yaml
  label: Express Gateway Scopes API
  slug: express-gateway-scopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-scopes-api-openapi.yml
- filename: express-gateway-users-api-openapi.yml
  format: yaml
  label: Express Gateway Users API
  slug: express-gateway-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/openapi/express-gateway-users-api-openapi.yml
authorization_urls: []
description: 'Express Gateway''s scope model. This artifact is unusual for its type: there is no fixed catalog of scope strings to enumerate, because Express Gateway does not define scopes — the OPERATOR does. A scope in Express Gateway is a free-form tag the operator declares on the gateway, attaches to API endpoints, and grants to consumer credentials. What the provider publishes is the mechanism, and that is what is recorded here.'
docs: https://www.express-gateway.io/docs/credential-management/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Express Gateway Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Express Gateway uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Express Gateway
provider_slug: express-gateway
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: express-gateway-scopes
source_filename: express-gateway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://www.express-gateway.io/docs/credential-management/\nprovider: Express Gateway\nproviderId: express-gateway\ndescription: >-\n  Express Gateway's scope model. This artifact is unusual for its type: there is\n  no fixed catalog of scope strings to enumerate, because Express Gateway does not\n  define scopes — the OPERATOR does. A scope in Express Gateway is a free-form tag\n  the operator declares on the gateway, attaches to API endpoints, and grants to\n  consumer credentials. What the provider publishes is the mechanism, and that is\n  what is recorded here.\ndocs: https://www.express-gateway.io/docs/credential-management/\nmodel: operator-defined\nscope_count: 0\nscope_count_note: >-\n  Zero is correct and is not a gap. There is no vendor-published scope list to\n  count; every scope in a running gateway was named by whoever configured it.\nmechanism:\n  declaration:\n    detail: Scopes are declared on the gateway\
  \ before they can be granted.\n    admin_api:\n    - POST /scopes (create in bulk)\n    - PUT /scopes/{scope} (create one)\n    - GET /scopes (list)\n    - GET /scopes/{scope} (existence check, 404 when absent)\n    - DELETE /scopes/{scope}\n    cli:\n    - eg scopes create\n    - eg scopes list\n    - eg scopes info\n    - eg scopes remove\n    docs: https://www.express-gateway.io/docs/admin/scopes/\n  grant:\n    detail: >-\n      Scopes are granted to a credential, not to a user or app directly. Any\n      credential type — basic-auth, key-auth or oauth2 — can carry scopes.\n    admin_api:\n    - PUT /credentials/{type}/{id}/scopes (replace the whole set)\n    - PUT /credentials/{type}/{id}/scopes/{scope} (add one)\n    - DELETE /credentials/{type}/{id}/scopes/{scope} (remove one)\n    cli:\n    - eg credential:scopes set\n    - eg credential:scopes add\n    - eg credential:scopes remove\n    docs: https://www.express-gateway.io/docs/credential-management/\n  enforcement:\n    detail:\
  \ >-\n      An API endpoint is marked with the scopes it requires; a request carrying a\n      credential without a matching scope is rejected by the authorization policy.\n      Scopes work across all three credential types, so the same tag governs key\n      auth and OAuth 2.0 alike.\n    docs: https://www.express-gateway.io/docs/core-concepts/\noauth2:\n  standard: RFC 6749\n  authorization_endpoint: /oauth2/authorize\n  token_endpoint: /oauth2/token\n  method_note: >-\n    Both endpoints accept POST only. Express Gateway acts as both authorization\n    server and resource server.\n  grants:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - password\n  scope_parameter: >-\n    The client passes `scope` in the authorization request; the consent UI prompts\n    the user to allow the client access to those scopes, and the resulting token\n    carries them.\n  docs: https://www.express-gateway.io/docs/policies/oauth2/\n  discovery:\n    oauth_authorization_server_metadata:\
  \ false\n    openid_configuration: false\n    detail: >-\n      No RFC 8414 authorization-server metadata and no OpenID configuration\n      document. Probed on www.express-gateway.io and express-gateway.io — both\n      /.well-known/oauth-authorization-server and\n      /.well-known/openid-configuration returned 404. This is expected: the\n      authorization server is the operator's own gateway instance, not a host\n      Express Gateway runs.\n  openid_connect:\n    supported: false\n    detail: \"\\\"OpenID 1.0 Policy\\\" is listed on the project roadmap as short-term work that never shipped.\"\n    docs: https://www.express-gateway.io/docs/roadmap/\nscopes: []\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express-gateway/refs/heads/main/scopes/express-gateway-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Composition
- API Gateway
- BFF
- Open Source
- Microservices
- Authentication
- Node.js
- Reverse Proxy
token_urls: []
---
