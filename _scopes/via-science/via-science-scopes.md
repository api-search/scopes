---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Via Science Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Via Science uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Via Science
provider_slug: via-science
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: via-science-scopes
source_filename: via-science-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  scopes_supported read verbatim from the anonymously-served OpenID Connect discovery\n  documents at https://auth.solvewithvia.com/auth/realms/qt/.well-known/openid-configuration\n  (HTTP 200) and https://auth.solvewithvia.com/auth/realms/ztf_demo/.well-known/openid-configuration\n  (HTTP 200), fetched 2026-09-02.\nname: VIA (Via Science, Inc.) — OAuth 2.0 / OIDC scopes\ndocs: null\ndocs_note: >-\n  VIA publishes no scope or permissions reference page. Everything below is read from the\n  realm discovery documents. The scope set is the Keycloak default profile — VIA has not\n  declared product-specific scopes (no `qt:transfer`, `ztf:*` or similar) on any realm that\n  answers anonymously, so an integrator cannot see a resource-permission model from outside.\n\nrealms:\n  - realm: qt\n    product: Quantum Transfer (QT)\n    issuer: https://auth.solvewithvia.com/auth/realms/qt\n  - realm: ztf_demo\n    product: Zero Trust\
  \ Fabric (ZTF) demo\n    issuer: https://auth.solvewithvia.com/auth/realms/ztf_demo\n\nscopes:\n  - name: openid\n    description: Required OpenID Connect scope; requests an ID token.\n    realms: [qt, ztf_demo]\n    standard: OpenID Connect Core 1.0\n  - name: profile\n    description: Standard OIDC profile claims (name, given_name, family_name, preferred_username).\n    realms: [qt, ztf_demo]\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description: Standard OIDC email claims.\n    realms: [qt, ztf_demo]\n    standard: OpenID Connect Core 1.0\n  - name: address\n    description: Standard OIDC address claim.\n    realms: [qt, ztf_demo]\n    standard: OpenID Connect Core 1.0\n  - name: phone\n    description: Standard OIDC phone_number claims.\n    realms: [qt, ztf_demo]\n    standard: OpenID Connect Core 1.0\n  - name: offline_access\n    description: Requests a refresh token usable while the user is offline.\n    realms: [qt, ztf_demo]\n    standard: OpenID Connect Core\
  \ 1.0\n  - name: roles\n    description: Keycloak client/realm role mappings in the token.\n    realms: [qt, ztf_demo]\n    standard: Keycloak default client scope\n  - name: web-origins\n    description: Injects allowed CORS web origins into the token.\n    realms: [qt, ztf_demo]\n    standard: Keycloak default client scope\n  - name: acr\n    description: Authentication Context Class Reference claim; carries the step-up level.\n    realms: [qt, ztf_demo]\n    standard: Keycloak default client scope\n  - name: basic\n    description: Minimal claim set (sub, iss, aud, exp, iat, auth_time).\n    realms: [qt, ztf_demo]\n    standard: Keycloak default client scope\n  - name: microprofile-jwt\n    description: Eclipse MicroProfile JWT claims (upn, groups).\n    realms: [qt, ztf_demo]\n    standard: Keycloak optional client scope\n  - name: service_account\n    description: Claims for client_credentials service-account tokens.\n    realms: [qt, ztf_demo]\n    standard: Keycloak optional client\
  \ scope\n\nscope_count: 12\nproduct_specific_scopes: 0\n\nacr_values_supported: ['0', '1']\nacr_note: >-\n  acr 0/1 is the hook ZTF step-up authentication uses — a sensitive operation is gated on a\n  higher authentication context, satisfied by a VIA Wallet signature rather than a second\n  password factor.\n\numa2:\n  supported: true\n  resource_registration_endpoint: https://auth.solvewithvia.com/auth/realms/ztf_demo/authz/protection/resource_set\n  permission_endpoint: https://auth.solvewithvia.com/auth/realms/ztf_demo/authz/protection/permission\n  policy_endpoint: https://auth.solvewithvia.com/auth/realms/ztf_demo/authz/protection/uma-policy\n  note: >-\n    UMA 2.0 is enabled on the realm, so fine-grained resource permissions exist at runtime\n    even though no static scope catalog is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/via-science/refs/heads/main/scopes/via-science-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Security
- Identity
- Authentication
- Zero Trust
- Decentralized Identity
- Verifiable Credentials
- Post-Quantum Cryptography
- Encryption
- File Transfer
- Defense
- Artificial Intelligence
- Blockchain
- OpenID Connect
token_urls: []
---
