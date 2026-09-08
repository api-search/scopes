---
api_specs:
- filename: elsevier-scopus-swagger.json
  format: json
  label: Elsevier Scopus APIs
  slug: elsevier-scopus-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-scopus-swagger.json
- filename: elsevier-sciencedirect-swagger.json
  format: json
  label: Elsevier ScienceDirect APIs
  slug: elsevier-sciencedirect-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-sciencedirect-swagger.json
- filename: elsevier-scival-swagger.json
  format: json
  label: Elsevier SciVal API
  slug: elsevier-scival-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-scival-swagger.json
- filename: elsevier-engineering-village-swagger.json
  format: json
  label: Elsevier Engineering Village API
  slug: elsevier-engineering-village-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-engineering-village-swagger.json
- filename: elsevier-retrieval-swagger.json
  format: json
  label: Elsevier Retrieval APIs
  slug: elsevier-retrieval-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-retrieval-swagger.json
- filename: elsevier-metadata-swagger.json
  format: json
  label: Elsevier Metadata APIs
  slug: elsevier-metadata-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-metadata-swagger.json
- filename: elsevier-abstract-api-openapi.yml
  format: yaml
  label: Elsevier Abstract API
  slug: elsevier-abstract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-abstract-api-openapi.yml
- filename: elsevier-search-api-openapi.yml
  format: yaml
  label: Elsevier Search API
  slug: elsevier-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-search-api-openapi.yml
authorization_urls: []
description: Elsevier runs a real OAuth 2.0 / OpenID Connect authorization server at https://id.elsevier.com (PingFederate), and it serves both RFC 8414 and OpenID Discovery metadata anonymously. The 35 scopes below are transcribed verbatim from scopes_supported in that document, fetched 2026-09-06 (HTTP 200, content-type text/plain).
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Elsevier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elsevier uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elsevier
provider_slug: elsevier
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: elsevier-scopes
source_filename: elsevier-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://id.elsevier.com/.well-known/openid-configuration\nsupporting_sources:\n- https://id.elsevier.com/.well-known/oauth-authorization-server\n- 'https://dev.elsevier.com/apikey/manage (302 -> id.elsevier.com/as/authorization.oauth2, the redirect that identifies id.elsevier.com as the authorization server behind the developer portal)'\n- https://dev.elsevier.com/tecdoc_api_authentication.html\ndocs: null\nprovider: Elsevier\nproviderId: elsevier\ndescription: >-\n  Elsevier runs a real OAuth 2.0 / OpenID Connect authorization server at\n  https://id.elsevier.com (PingFederate), and it serves both RFC 8414 and OpenID Discovery\n  metadata anonymously. The 35 scopes below are transcribed verbatim from\n  scopes_supported in that document, fetched 2026-09-06 (HTTP 200,\n  content-type text/plain).\nscope_model: identity-platform\nread_this_first: >-\n  THESE ARE NOT API SCOPES. Every scope the authorization server advertises governs\
  \ identity\n  and profile release — who the signed-in person is, which institution they are associated\n  with, whether their email is confirmed — not which Research Products API operation a token\n  may call. Access to api.elsevier.com is still governed by the X-ELS-APIKey plus the\n  institutional entitlement model described in authentication/elsevier-authentication.yml,\n  and Elsevier publishes no scope, permission or role reference for those APIs anywhere.\n  Recording the identity scopes here without that sentence would credit Elsevier with a\n  fine-grained API authorization model it does not publish.\nauthorization_server:\n  issuer: https://id.elsevier.com\n  software: PingFederate\n  discovery:\n  - path: /.well-known/openid-configuration\n    status: 200\n    file: ../well-known/elsevier-id-openid-configuration.json\n  - path: /.well-known/oauth-authorization-server\n    status: 200\n    file: ../well-known/elsevier-id-oauth-authorization-server.json\n  authorization_endpoint:\
  \ https://id.elsevier.com/as/authorization.oauth2\n  token_endpoint: https://id.elsevier.com/as/token.oauth2\n  introspection_endpoint: https://id.elsevier.com/as/introspect.oauth2\n  revocation_endpoint: https://id.elsevier.com/as/revoke_token.oauth2\n  userinfo_endpoint: https://id.elsevier.com/idp/userinfo.openid\n  registration_endpoint: https://id.elsevier.com/as/clients.oauth2\n  device_authorization_endpoint: https://id.elsevier.com/as/device_authz.oauth2\n  jwks_uri: https://id.elsevier.com/pf/JWKS\n  grant_types_supported:\n  - implicit\n  - authorization_code\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:pingidentity.com:oauth2:grant_type:validate_bearer\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:saml2-bearer\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:openid:params:grant-type:ciba\n  pkce_methods:\n  - plain\n  - S256\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - none\n  notes:\n  - >-\n    The implicit and password grants are still advertised; both are discouraged by OAuth 2.1\n    and neither should be chosen by a new integration.\n  - >-\n    id_token_signing_alg_values_supported includes \"none\", which an id_token validator must\n    reject explicitly.\nscope_count: 35\nscopes:\n- name: openid\n  standard: true\n  description: OpenID Connect — request an id_token.\n- name: profile\n  standard: true\n  description: Standard OIDC profile claims (name, given_name, family_name, picture, updated_at).\n- name: email\n  standard: true\n  description: Standard OIDC email and email_verified claims.\n- name: address\n  standard: true\n  description: Standard OIDC address claim.\n- name: phone\n  standard: true\n  description: Standard OIDC phone claim.\n- name: els_universal_identity\n  standard: false\n  description: Elsevier universal\
  \ identity information (els_universal_identity_info claim).\n- name: els_universal_access\n  standard: false\n  description: Elsevier universal access attributes.\n- name: els_auth_info\n  standard: false\n  description: >-\n    Authentication context — auth_time, auth_token, auth_failure. Requested by the developer\n    portal's own client (client_id ELSAPI-PROD) on the sign-in redirect.\n- name: els_idp_info\n  standard: false\n  description: Identity-provider metadata for the session (idp_info claim).\n- name: els_analytics_info\n  standard: false\n  description: Analytics attributes attached to the identity (analytics_info claim). Also requested by ELSAPI-PROD.\n- name: els_idp_analytics_attrs\n  standard: false\n  description: Identity-provider analytics attributes (idp_analytics_attrs claim).\n- name: els_user_roles\n  standard: false\n  description: Roles held by the user (user_roles claim).\n- name: els_sa_discover\n  standard: false\n  description: Seamless-access / institution-discovery\
  \ attribute release.\n- name: individual_identity\n  standard: false\n  description: Individual (person-level) identity, as distinct from institutional association.\n- name: institutional_association\n  standard: false\n  description: The institution the user is associated with (inst_assoc, inst_acct_* claims).\n- name: universal\n  standard: false\n  description: Elsevier universal identity umbrella scope.\n- name: urn:com:elsevier:idp:policy:product:indv_identity\n  standard: false\n  description: >-\n    Policy scope requiring individual identity to be established. Requested by ELSAPI-PROD on\n    the developer-portal sign-in.\n- name: urn:com:elsevier:idp:policy:product:inst_assoc\n  standard: false\n  description: Policy scope requiring institutional association to be established.\n- name: urn:com:elsevier:idp:policy:product:force_sign_in\n  standard: false\n  description: Policy scope forcing an interactive sign-in rather than silent session reuse.\n- name: urn:com:elsevier:idp:policy:product:user_roles\n\
  \  standard: false\n  description: Policy scope releasing user roles.\n- name: urn:com:elsevier:idp:policy:product:salutation\n  standard: false\n  description: Policy scope releasing the salutation claim.\n- name: urn:com:elsevier:idp:policy:product:formal_email\n  standard: false\n  description: Policy scope releasing the formal email address.\n- name: urn:com:elsevier:idp:policy:feature:attribute:country\n  standard: false\n  description: Policy scope releasing the country attribute.\n- name: urn:idp:policy:universal:attribute:name\n  standard: false\n  description: Policy scope releasing the name attribute.\n- name: urn:idp:policy:feature:security:password:strongPassword\n  standard: false\n  description: Policy scope asserting the strong-password requirement was met.\n- name: urn:idp:policy:product:confirmation:emailconfirmation\n  standard: false\n  description: Email-confirmation policy, generic.\n- name: urn:idp:policy:product:confirmation:EAPI:emailconfirmation\n  standard: false\n\
  \  description: >-\n    Email-confirmation policy scoped to EAPI — the Elsevier developer/API portal. This is the\n    scope that ties this authorization server to dev.elsevier.com.\n- name: urn:idp:policy:product:confirmation:SD:emailconfirmation\n  standard: false\n  description: Email-confirmation policy scoped to ScienceDirect.\n- name: urn:idp:policy:product:confirmation:OSC:emailconfirmation\n  standard: false\n  description: Email-confirmation policy scoped to OSC.\n- name: urn:idp:policy:product:confirmation:MDY:emailconfirmation\n  standard: false\n  description: Email-confirmation policy scoped to MDY (Mendeley).\n- name: urn:idp:policy:product:confirmation:IDMIG:emailconfirmation\n  standard: false\n  description: Email-confirmation policy scoped to the identity-migration product.\n- name: urn:idp:policy:product:SD:idp_user_linking_attribute\n  standard: false\n  description: ScienceDirect user-linking attribute release.\n- name: urn:idp:policy:product:PURE:idp_user_linking_attribute\n\
  \  standard: false\n  description: Pure user-linking attribute release.\n- name: Demo_rel2020.11\n  standard: false\n  description: >-\n    A demonstration scope left in the production advertisement. Recorded because it is in the\n    provider's own document, not because it is usable.\n- name: Demo_rel2020.12\n  standard: false\n  description: A second demonstration scope, as above.\ngaps:\n- >-\n  No scope in this list maps to a Research Products API operation. There is no\n  scopes_supported entry for Scopus, ScienceDirect content, SciVal, Embase, Engineering\n  Village or SUSHI.\n- >-\n  Elsevier's own auth guide says \"We offer an oauth implementation for developers wanting to\n  integrate ScienceDirect and/or Scopus content into client-side applications requiring access\n  to user level (rather than institutional) content\", but publishes no client-registration\n  path, no grant walkthrough and no scope for it. The mechanism is discoverable here; the\n  product documentation for it\
  \ is not.\n- >-\n  api.elsevier.com serves no /.well-known/oauth-protected-resource, so a client that finds a\n  401 there has no RFC 9728 pointer back to this authorization server. The link between the\n  two was established here by following the developer portal's sign-in redirect, not by any\n  document Elsevier publishes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/scopes/elsevier-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Content
- Journals
- Medical
- Research
- Scientific
- Technical
token_urls: []
---
