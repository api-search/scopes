---
api_specs:
- filename: nus-identity-openapi.yml
  format: yaml
  label: NUS Federated Identity Service (VAFS)
  slug: identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/openapi/nus-identity-openapi.yml
authorization_urls: []
description: The complete set of OAuth 2.0 / OpenID Connect scopes the National University of Singapore's own authorization server advertises to clients, plus the claims it will assert. These were read from the institution's live discovery document, not inferred. NUS publishes no prose documentation of these scopes anywhere public — the discovery document is the only description of them that exists on the open internet.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Nus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'National University of Singapore uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: National University of Singapore
provider_slug: nus
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: nus-scopes
source_filename: nus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  scopes_supported and claims_supported read verbatim from\n  https://vafs.nus.edu.sg/adfs/.well-known/openid-configuration (HTTP 200, fetched 2026-08-19)\nprovider: National University of Singapore\nproviderId: nus\nx-operator: institution\ndescription: >-\n  The complete set of OAuth 2.0 / OpenID Connect scopes the National University of Singapore's\n  own authorization server advertises to clients, plus the claims it will assert. These were\n  read from the institution's live discovery document, not inferred. NUS publishes no prose\n  documentation of these scopes anywhere public — the discovery document is the only\n  description of them that exists on the open internet.\nauthorization_server: https://vafs.nus.edu.sg/adfs\nscopes:\n- name: openid\n  standard: true\n  description: Requests an ID token; required for any OpenID Connect flow against this provider.\n- name: profile\n  standard: true\n  description: Requests\
  \ the end user's basic profile claims.\n- name: email\n  standard: true\n  description: Requests the end user's email address claim.\n- name: allatclaims\n  standard: false\n  vendor: Microsoft ADFS\n  description: >-\n    ADFS-specific scope that asks the provider to place all claims from the access token into\n    the ID token as well. Broad by construction — grant it deliberately, not by default.\n- name: user_impersonation\n  standard: false\n  vendor: Microsoft ADFS\n  description: >-\n    Permits a client to act on behalf of the signed-in user against a downstream NUS resource.\n    The highest-consequence scope this provider advertises.\n- name: aza\n  standard: false\n  vendor: Microsoft ADFS\n  description: Broker/primary-refresh-token scope used by Microsoft device authentication brokers.\n- name: logon_cert\n  standard: false\n  vendor: Microsoft ADFS\n  description: Requests a logon certificate for the authenticated user.\n- name: vpn_cert\n  standard: false\n  vendor: Microsoft\
  \ ADFS\n  description: Requests a VPN client certificate for the authenticated user.\n- name: winhello_cert\n  standard: false\n  vendor: Microsoft ADFS\n  description: Requests a Windows Hello for Business certificate for the authenticated user.\nclaims_supported:\n- aud\n- iss\n- iat\n- exp\n- auth_time\n- nonce\n- at_hash\n- c_hash\n- sub\n- upn\n- unique_name\n- pwd_url\n- pwd_exp\n- mfa_auth_time\n- sid\n- nbf\nnotes: >-\n  Three of the nine advertised scopes (logon_cert, vpn_cert, winhello_cert) mint credentials\n  rather than grant data access, and two more (allatclaims, user_impersonation) are broad by\n  design. Only three are standard OIDC scopes. An agent integrating with NUS should request\n  `openid profile email` and nothing else; the remainder exist for Microsoft device and VPN\n  enrolment flows and have no third-party use case.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nus/refs/heads/main/scopes/nus-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Singapore
- Research
- Identity Federation
- Research Repository
- Course Catalog
- Open Access
- Learning Management
token_urls: []
---
