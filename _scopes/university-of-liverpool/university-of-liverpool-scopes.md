---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Liverpool Scopes
name_suffix: OAuth Scopes
note: The only scope vocabulary the University of Liverpool publishes machine-readably is the one advertised by its own AD FS authorization server's OpenID Connect discovery document. Read verbatim from that document on 2026-09-01. The scholarly surfaces (OAI-PMH, EPrints REST) are anonymous and have no scope model at all; the Canvas, Elements, Alma/Primo and Talis scopes belong to those vendors' products and are deliberately not restated here.
overview: 'University of Liverpool uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Liverpool
provider_slug: university-of-liverpool
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-liverpool-scopes
source_filename: university-of-liverpool-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://fs.liverpool.ac.uk/adfs/.well-known/openid-configuration\nnote: >-\n  The only scope vocabulary the University of Liverpool publishes machine-readably is the one\n  advertised by its own AD FS authorization server's OpenID Connect discovery document. Read\n  verbatim from that document on 2026-09-01. The scholarly surfaces (OAI-PMH, EPrints REST) are\n  anonymous and have no scope model at all; the Canvas, Elements, Alma/Primo and Talis scopes belong\n  to those vendors' products and are deliberately not restated here.\nissuer: https://fs.liverpool.ac.uk/adfs\noperator: institution\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n- name: profile\n  description: Standard OIDC profile claims.\n- name: email\n  description: Standard OIDC email claim.\n- name: allatclaims\n  description: AD FS scope returning all claims configured for the relying party.\n- name: aza\n  description:\
  \ AD FS broker/primary-refresh-token scope used by Microsoft client stacks.\n- name: user_impersonation\n  description: AD FS delegated access on behalf of the signed-in user.\n- name: logon_cert\n  description: AD FS certificate-based logon scope.\n- name: winhello_cert\n  description: AD FS Windows Hello for Business certificate enrolment scope.\n- name: vpn_cert\n  description: AD FS VPN certificate issuance scope.\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- client_credentials\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- implicit\n- password\n- srv_challenge\n- urn:ietf:params:oauth:grant-type:device_code\n- device_code\nresponse_types_supported:\n- code\n- id_token\n- code id_token\n- id_token token\n- code token\n- code id_token token\nself_service_registration: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-liverpool/refs/heads/main/scopes/university-of-liverpool-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Russell Group
- United Kingdom
- Research
- Research Repository
- Research Data
- Open Access
- OAI-PMH
- EPrints
- Identity Federation
- Library
- Metadata
token_urls: []
---
