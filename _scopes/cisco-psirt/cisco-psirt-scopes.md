---
api_specs:
- filename: cisco-psirt-current-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Current Endpoints API
  slug: cisco-psirt-current-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-current-endpoints-api-openapi.yml
- filename: cisco-psirt-obsolete-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Obsolete Endpoints API
  slug: cisco-psirt-obsolete-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml
- filename: cisco-psirt-sunset-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Sunset Endpoints API
  slug: cisco-psirt-sunset-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-sunset-endpoints-api-openapi.yml
authorization_urls: []
description: 'The openVuln API uses OAuth 2.0 client credentials but has effectively NO scope model. Cisco publishes no scopes reference, no permissions page, and no per-endpoint scope requirements; the OpenAPI declares the token only as an HTTP bearer (no oauth2 securityScheme, therefore no flows.scopes map to derive from). The single scope value in existence is the one visible in Cisco''s own published token response — "customscope" — which is granted uniformly to every application registered against this API. Entitlement here is binary: your application is either subscribed to the Cisco PSIRT openVuln API or it is not.'
docs: https://developer.cisco.com/docs/psirt/authentication/
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cisco Psirt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cisco PSIRT openVuln API publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cisco PSIRT openVuln API API on a user''s behalf.


  Tokens are issued from https://id.cisco.com/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cisco PSIRT openVuln API
provider_slug: cisco-psirt
schemes:
- flows:
  - authorizationUrl: null
    flow: clientCredentials
    tokenUrl: https://id.cisco.com/oauth2/default/v1/token
  name: cisco-oauth2-client-credentials
  source: https://developer.cisco.com/docs/psirt/authentication/
scope_count: 2
scope_names:
- customscope
- read:advisories
scopes:
- description: The scope Cisco's identity service returns in the access token for a registered openVuln API application. Not documented as a named permission; observed verbatim in the token response Cisco publishes in its own authentication guide ("scope":"customscope").
  flows:
  - clientCredentials
  scope: customscope
- description: Attached to 28 of the 30 operations as a security[] requirement on the psirt_openvuln_api_auth scheme. Since that scheme is type http / scheme bearer rather than oauth2, OpenAPI assigns this list no semantics — it is decorative in the contract as published, and it is NOT the scope the token endpoint actually returns.
  flows: []
  scope: read:advisories
slug: cisco-psirt-scopes
source_filename: cisco-psirt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://developer.cisco.com/docs/psirt/authentication/\ndocs: https://developer.cisco.com/docs/psirt/authentication/\ndescription: >-\n  The openVuln API uses OAuth 2.0 client credentials but has effectively NO scope\n  model. Cisco publishes no scopes reference, no permissions page, and no\n  per-endpoint scope requirements; the OpenAPI declares the token only as an HTTP\n  bearer (no oauth2 securityScheme, therefore no flows.scopes map to derive from).\n  The single scope value in existence is the one visible in Cisco's own published\n  token response — \"customscope\" — which is granted uniformly to every application\n  registered against this API. Entitlement here is binary: your application is\n  either subscribed to the Cisco PSIRT openVuln API or it is not.\nderivation_note: >-\n  0-working/derive-oauth-scopes.py was run and returned zero oauth2 schemes and\n  zero scopes, because the spec models the token as http/bearer.\
  \ This file is the\n  SEARCHED upgrade from the docs and must not be overwritten by that derived pass.\nschemes:\n  - name: cisco-oauth2-client-credentials\n    source: https://developer.cisco.com/docs/psirt/authentication/\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://id.cisco.com/oauth2/default/v1/token\n        authorizationUrl: null\nscopes:\n  - scope: customscope\n    description: >-\n      The scope Cisco's identity service returns in the access token for a\n      registered openVuln API application. Not documented as a named permission;\n      observed verbatim in the token response Cisco publishes in its own\n      authentication guide (\"scope\":\"customscope\").\n    flows: [clientCredentials]\n    sources: ['https://developer.cisco.com/docs/psirt/authentication/']\n    granularity: application-wide\n    authoritative: true\n  - scope: read:advisories\n    description: >-\n      Attached to 28 of the 30 operations as a security[] requirement on the\n\
  \      psirt_openvuln_api_auth scheme. Since that scheme is type http / scheme\n      bearer rather than oauth2, OpenAPI assigns this list no semantics — it is\n      decorative in the contract as published, and it is NOT the scope the token\n      endpoint actually returns.\n    flows: []\n    sources:\n      - openapi/cisco-psirt-current-endpoints-api-openapi.yml\n      - openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml\n      - openapi/cisco-psirt-sunset-endpoints-api-openapi.yml\n    granularity: per-operation-declared\n    authoritative: false\n    operations_declaring_it: 28\n    operations_without_it: [\"/all/firstpublished\", \"/all/lastpublished\"]\nscope_count: 2\nper_operation_scopes: declared-but-not-enforceable\ndiscrepancy:\n  finding: >-\n    The spec's per-operation scope (read:advisories) and the identity service's\n    issued scope (customscope) are different strings, and only the latter is real.\n  impact: >-\n    An integrator wiring an OAuth2 client from the\
  \ spec would request a scope the\n    token endpoint does not grant. Worth reporting to Cisco: modelling the scheme\n    as oauth2/clientCredentials with a flows.scopes map would make the contract\n    self-consistent.\n  spec_evidence: 'openapi/_original/cisco-psirt-openvuln-openapi.json paths./all.get.security[0].psirt_openvuln_api_auth'\n  docs_evidence: 'https://developer.cisco.com/docs/psirt/authentication/ — token response \"scope\":\"customscope\"'\nentitlement_model:\n  type: api-subscription\n  detail: >-\n    Access is granted at registration time by selecting \"Cisco PSIRT openVuln API\"\n    in the Cisco API Console application form, not by requesting scopes at token\n    time. There is no consent screen and no user-delegated authorization — the\n    grant type is client credentials only.\n  console: https://apiconsole.cisco.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/scopes/cisco-psirt-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Security
- Vulnerability Management
- Threat Intelligence
- Disclosure
- Compliance
- Networking
token_urls:
- https://id.cisco.com/oauth2/default/v1/token
---
