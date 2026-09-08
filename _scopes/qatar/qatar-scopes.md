---
api_specs:
- filename: qatar-qu-sso-oidc-openapi.yml
  format: yaml
  label: Qatar University Single Sign-On (OpenID Connect / OAuth 2.0)
  slug: qu-sso-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/openapi/qatar-qu-sso-oidc-openapi.yml
- filename: qatar-qupress-oai-pmh-openapi.yml
  format: yaml
  label: QU Press Open Journal System OAI-PMH API
  slug: qupress-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/openapi/qatar-qupress-oai-pmh-openapi.yml
authorization_urls: []
description: 'Qatar University declares an authorization scope model on exactly one surface — its own OpenID Connect provider at sso.qu.edu.qa. Five scopes are supported, and they are the five standard OpenID Connect scopes with nothing institution-specific added: no scope distinguishes a student from staff, no scope names a system, and there is no read/write split. Thirty claims are supported, including the non-standard `groups` and `upn`, which is where any role information would actually travel.

  Every other surface in the profile is either anonymous (the QU Press OAI-PMH endpoint Qatar University operates, plus the QSpace endpoints its hosting provider operates) or gated by institutional affiliation with no published scope model.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Qatar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Qatar University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qatar University
provider_slug: qatar
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: qatar-scopes
source_filename: qatar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Evangelist Scopes\nspecificationVersion: '0.1'\nx-method: derived  # authorship, for build-provenance-manifest.py — API Evangelist wrote this file; see `method:` below for how the facts in it were obtained\nprovider: Qatar University\nproviderId: qatar\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Read directly from the `scopes_supported` and `claims_supported` arrays of the live OpenID\n  Connect discovery document at\n  https://sso.qu.edu.qa/oauth2/token/.well-known/openid-configuration (HTTP 200, 2026-09-01),\n  archived at examples/qatar-qu-sso-openid-configuration.json. Not inferred, not generated:\n  this is the provider's own declaration, transcribed.\ndescription: >-\n  Qatar University declares an authorization scope model on exactly one surface — its own\n  OpenID Connect provider at sso.qu.edu.qa. Five scopes are supported, and they are the five\n  standard OpenID Connect scopes with nothing institution-specific added: no scope\n  distinguishes\
  \ a student from staff, no scope names a system, and there is no read/write\n  split. Thirty claims are supported, including the non-standard `groups` and `upn`, which is\n  where any role information would actually travel.\n\n  Every other surface in the profile is either anonymous (the QU Press OAI-PMH endpoint Qatar\n  University operates, plus the QSpace endpoints its hosting provider operates) or gated by\n  institutional affiliation with no published scope model.\nsurfaces:\n  - aid: 'qatar:qu-sso-oidc'\n    operator: institution\n    url: https://sso.qu.edu.qa\n    model: oauth2-openid-connect\n    scopes:\n      - name: openid\n        standard: 'OpenID Connect Core 1.0'\n        description: Required to request an ID token. Marks the request as an OpenID Connect request.\n      - name: profile\n        standard: 'OpenID Connect Core 1.0'\n        description: >-\n          Default profile claims — name, family_name, given_name, middle_name, nickname,\n          preferred_username,\
  \ picture, website, gender, birthdate, zoneinfo, locale, updated_at.\n      - name: email\n        standard: 'OpenID Connect Core 1.0'\n        description: email and email_verified claims.\n      - name: address\n        standard: 'OpenID Connect Core 1.0'\n        description: The address claim — formatted, street_address, locality, region, postal_code, country.\n      - name: phone\n        standard: 'OpenID Connect Core 1.0'\n        description: phone_number and phone_number_verified claims.\n    claims_supported:\n      - sub\n      - iss\n      - acr\n      - name\n      - given_name\n      - family_name\n      - middle_name\n      - nickname\n      - preferred_username\n      - profile\n      - picture\n      - website\n      - gender\n      - birthdate\n      - zoneinfo\n      - locale\n      - updated_at\n      - email\n      - email_verified\n      - address\n      - formatted\n      - street_address\n      - locality\n      - region\n      - postal_code\n      - country\n \
  \     - phone_number\n      - phone_number_verified\n      - groups\n      - upn\n    non_standard_claims:\n      - name: groups\n        note: >-\n          Not an OpenID Connect Core claim. In a WSO2 deployment this carries the user's\n          directory group membership, and it is the only route by which role or affiliation\n          information reaches a relying party — there is no scope that expresses it.\n      - name: upn\n        note: >-\n          User Principal Name, an Active Directory / Microsoft convention rather than an\n          OpenID Connect claim. Its presence indicates the identity store behind this provider\n          is an AD or LDAP directory.\n    gaps:\n      - >-\n        No institution-specific scopes. A university's interesting authorizations —\n        eduPersonAffiliation, student vs staff vs faculty, enrolment, entitlement — are not\n        expressible in this scope set. eduPerson attributes travel, if at all, over the SAML\n        side of the same provider,\
  \ where the published metadata declares no attribute release.\n      - >-\n        No read/write or least-privilege distinction on any scope.\n      - >-\n        Dynamic Client Registration is advertised, but with only these five scopes available\n        a dynamically registered client cannot request anything narrower than \"everything\n        about this person\".\n  - aid: 'qatar:qspace'\n    operator: tenant\n    model: none\n    note: >-\n      Anonymous OAI-PMH harvesting and anonymous DSpace 7.6 read operations. No scope model;\n      access is all-or-nothing and it is all. DSpace's own authorization model (EPerson, Group,\n      ResourcePolicy) governs writes, but it is not exposed as OAuth scopes and no public\n      account can reach it. Operator is tenant: qspace.qu.edu.qa CNAMEs to\n      qataru.cname.openrepository.com, a commercial hosted-DSpace service.\n  - aid: 'qatar:qupress-oai'\n    operator: institution\n    model: none\n    note: >-\n      Anonymous OAI-PMH harvesting\
  \ across nine journals. The adjacent OJS REST API uses a\n      per-user API token, not scopes, and is 403 to the public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/scopes/qatar-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Qatar
- Middle East
- Research
- Identity Federation
- Scholarly Publishing
- Research Repository
- Open Access
- OAI-PMH
- SAML
- OpenID Connect
token_urls: []
---
