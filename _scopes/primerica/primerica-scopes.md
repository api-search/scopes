---
authorization_urls: []
description: OAuth 2.0 / OIDC scopes Primerica's own authorization servers advertise in their anonymous discovery documents, plus the two application scopes Primerica publishes in the MyPrimerica authorize URL on its public client-portal page. There is no published scope reference for third parties because there is no third-party API programme.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Primerica Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Primerica uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Primerica
provider_slug: primerica
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: primerica-scopes
source_filename: primerica-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://login.my.primerica.com/oauth2/aus8qhl8ufh9Bx3Dn697/.well-known/openid-configuration,\n  https://login.my.primerica.com/.well-known/openid-configuration,\n  https://login.primericaonline.com/.well-known/openid-configuration,\n  https://gtw.primericaonline.com/.well-known/openid-configuration,\n  https://www.primerica.com/public/primerica-client-portals.html (published authorize URL)\nspecification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Primerica\nproviderId: primerica\ndescription: >-\n  OAuth 2.0 / OIDC scopes Primerica's own authorization servers advertise in their anonymous discovery\n  documents, plus the two application scopes Primerica publishes in the MyPrimerica authorize URL on its\n  public client-portal page. There is no published scope reference for third parties because there is no\n  third-party API programme.\ndocs: null\nnotes: >-\n  `client-portal:write` and `cm.readonly`\
  \ are the only Primerica-authored (non-platform-default) scopes\n  visible on the public surface. Everything else in scopes_supported is an Okta or Layer7 platform\n  default. Descriptions below are recorded only where Primerica or the standard defines them; no\n  description has been invented.\nscope_count: 8\nscopes:\n  - name: openid\n    server: myprimerica-client-portal\n    standard: OpenID Connect Core 1.0\n    description: Requests an ID token; required for OIDC.\n  - name: profile\n    server: myprimerica-client-portal\n    standard: OpenID Connect Core 1.0\n    description: Standard OIDC profile claims.\n  - name: email\n    server: myprimerica-client-portal\n    standard: OpenID Connect Core 1.0\n    description: Standard OIDC email and email_verified claims.\n  - name: offline_access\n    server: myprimerica-client-portal\n    standard: OpenID Connect Core 1.0\n    description: Requests a refresh token.\n  - name: client-portal:write\n    server: myprimerica-client-portal\n\
  \    standard: null\n    first_party: true\n    description: >-\n      Primerica-defined application scope requested by the MyPrimerica SPA. Write access to the client\n      portal surface. No published definition — recorded verbatim from the authorize URL Primerica\n      publishes at https://www.primerica.com/public/primerica-client-portals.html\n  - name: cm.readonly\n    server: myprimerica-client-portal\n    standard: null\n    first_party: true\n    description: >-\n      Primerica-defined application scope requested by the MyPrimerica SPA alongside the `cm` BFF\n      endpoint (https://gtw.primericaonline.com/prod/exp/pc2/bff). Read-only. No published definition.\n  - name: device_sso\n    server: myprimerica-client-portal\n    standard: Okta platform default\n    description: Okta device single sign-on.\n  - name: openid_client_registration\n    server: layer7-gateway\n    standard: Layer7 OAuth Toolkit default\n    description: Dynamic client registration scope advertised by\
  \ the gateway OIDC provider.\nplatform_default_scopes:\n  note: >-\n    The client-portal authorization server also advertises the full Okta `okta.myAccount.*` scope family\n    (16 scopes) and the org server advertises address, phone and groups. These are Okta platform\n    defaults, not Primerica product scopes, and are not counted above.\n  okta_myaccount:\n    - okta.myAccount.read\n    - okta.myAccount.manage\n    - okta.myAccount.profile.read\n    - okta.myAccount.profile.manage\n    - okta.myAccount.email.read\n    - okta.myAccount.email.manage\n    - okta.myAccount.phone.read\n    - okta.myAccount.phone.manage\n    - okta.myAccount.authenticators.read\n    - okta.myAccount.authenticators.manage\n    - okta.myAccount.appAuthenticator.read\n    - okta.myAccount.appAuthenticator.manage\n    - okta.myAccount.appAuthenticator.maintenance.read\n    - okta.myAccount.appAuthenticator.maintenance.manage\n    - okta.myAccount.oktaApplications.read\n    - okta.myAccount.organization.read\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primerica/refs/heads/main/scopes/primerica-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Financial Services
- Life Insurance
- Identity
- Authentication
- OpenID Connect
- API Gateway
token_urls: []
---
