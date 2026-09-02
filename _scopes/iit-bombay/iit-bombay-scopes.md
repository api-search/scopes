---
api_specs:
- filename: iit-bombay-instiapp-api-openapi.yml
  format: yaml
  label: InstiApp API
  slug: instiapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/openapi/iit-bombay-instiapp-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Iit Bombay Scopes
name_suffix: OAuth Scopes
note: Two of IIT Bombay's three institution-operated auth surfaces declare scopes. The Gymkhana Profiles list below is transcribed verbatim from the institution's own published documentation (searched, not inferred); the IITB Central SSO list is read from its live OIDC discovery document (probed). The InstiApp API declares no scopes at all — its specification carries a single HTTP Basic scheme and no oauth2 flow — so no scope set is asserted for it.
overview: 'Indian Institute of Technology Bombay uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Indian Institute of Technology Bombay
provider_slug: iit-bombay
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: iit-bombay-scopes
source_filename: iit-bombay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://gymkhana.iitb.ac.in/profiles/doc/\nnote: >-\n  Two of IIT Bombay's three institution-operated auth surfaces declare scopes. The Gymkhana\n  Profiles list below is transcribed verbatim from the institution's own published documentation\n  (searched, not inferred); the IITB Central SSO list is read from its live OIDC discovery\n  document (probed). The InstiApp API declares no scopes at all — its specification carries a\n  single HTTP Basic scheme and no oauth2 flow — so no scope set is asserted for it.\nsurfaces:\n\n- api: Gymkhana Profiles OAuth API\n  x-operator: institution\n  base: https://gymkhana.iitb.ac.in/profiles/\n  method: searched\n  source: https://gymkhana.iitb.ac.in/profiles/doc/\n  delivery: space-separated `scope` query parameter on the authorize request\n  default_when_omitted: basic\n  count: 10\n  scopes:\n  - name: basic\n    grants: User id from the SSO server (not the LDAP id).\n    default: true\n\
  \  - name: profile\n    grants: first_name, last_name and account type.\n  - name: picture\n    grants: Profile picture.\n  - name: sex\n    grants: Sex — Male, Female or Other.\n  - name: ldap\n    grants: LDAP username and e-mail address.\n    sensitivity: identifies the individual against the institutional directory\n  - name: phone\n    grants: Contact number, including additional numbers.\n    sensitivity: personal contact data\n  - name: insti_address\n    grants: Address inside the institute.\n    sensitivity: personal location data\n  - name: program\n    grants: Roll number, department, course, joining year and graduation year.\n    sensitivity: student record data\n  - name: secondary_emails\n    grants: Alternate e-mail addresses.\n    sensitivity: personal contact data\n  - name: send_mail\n    grants: Permission for the application to send the user e-mail via the SSO server.\n    kind: write / action scope\n  observations: >-\n    This is a genuinely granular consent model\
  \ for a student-operated service — ten scopes with\n    contact, directory identity and student-record data each separated rather than bundled into\n    a single \"profile\" grant. It is also the only place in IIT Bombay's public footprint where\n    student-record fields (roll number, department, graduation year) are exposed under explicit\n    user consent, which is the fact that matters for the education regime.\n\n- api: IITB Central SSO (OpenID Connect)\n  x-operator: institution\n  base: https://sso.iitb.ac.in\n  method: probed\n  source: https://sso.iitb.ac.in/.well-known/openid-configuration\n  probe_status: 200\n  count: 1\n  scopes:\n  - name: openid\n    grants: >-\n      Authentication only. The discovery document advertises scopes_supported: [\"openid\"] and\n      nothing further — no profile, email or offline_access. Claims beyond the subject are\n      obtained from the userinfo endpoint (https://sso.iitb.ac.in/user, probed 401\n      unauthenticated) rather than requested\
  \ by scope.\n  observations: >-\n    A single-scope OIDC provider. Correct and minimal for a campus identity broker, and worth\n    noting that the institution's central SSO deliberately exposes LESS through scopes than the\n    student body's Profiles service does.\n\n- api: InstiApp API\n  x-operator: institution\n  base: https://gymkhana.iitb.ac.in/instiapp/api\n  method: derived\n  source: openapi/iit-bombay-instiapp-api-openapi.yml\n  count: 0\n  scopes: []\n  observations: >-\n    No scopes are declared. components.securitySchemes holds one entry, Basic (http/basic),\n    applied globally. Authorisation in this API is enforced by per-body roles inside the\n    application (see the roles tag and the BodyRole schema), not by OAuth scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iit-bombay/refs/heads/main/scopes/iit-bombay-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- India
- Institute of Technology
- Research
- Identity
- Single Sign-On
- OpenID Connect
- Campus Life
- Research Repository
- Open-Source
token_urls: []
---
