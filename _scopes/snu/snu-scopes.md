---
api_specs:
- filename: snu-s-space-oai-pmh-openapi.yml
  format: yaml
  label: S-Space OAI-PMH Repository Interface
  slug: s-space-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/openapi/snu-s-space-oai-pmh-openapi.yml
- filename: snu-kossda-oai-pmh-openapi.yml
  format: yaml
  label: KOSSDA OAI-PMH Repository Interface
  slug: kossda-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/openapi/snu-kossda-oai-pmh-openapi.yml
- filename: snu-s-space-opensearch-openapi.yml
  format: yaml
  label: S-Space OpenSearch Interface
  slug: s-space-opensearch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/openapi/snu-s-space-opensearch-openapi.yml
authorization_urls: []
description: Seoul National University publishes no OAuth 2.0 or OIDC authorization server, so there are no scopes in the OAuth sense and none are invented here. The nearest real equivalent — the attribute-release contract that governs what SNU's Identity Provider discloses about a person to a relying party — is recorded below, because for a university that IS the authorization surface.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Snu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Seoul National University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Seoul National University
provider_slug: snu
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: snu-scopes
source_filename: snu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Derived from authentication/snu-authentication.yml and\n  authentication/snu-kafe-saml-idp-metadata.xml, plus negative probes for OAuth/OIDC\n  discovery documents on www.snu.ac.kr and api.snu.ac.kr (2026-08-19).\ndescription: >-\n  Seoul National University publishes no OAuth 2.0 or OIDC authorization server, so there\n  are no scopes in the OAuth sense and none are invented here. The nearest real\n  equivalent — the attribute-release contract that governs what SNU's Identity Provider\n  discloses about a person to a relying party — is recorded below, because for a\n  university that IS the authorization surface.\noauth:\n  present: false\n  evidence: >-\n    https://www.snu.ac.kr/.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server both return 404; api.snu.ac.kr returns 403 at\n    the root and 404 on every path probed.\nsaml_attribute_release:\n  entity_id: https://kafegw.snu.ac.kr/idp/simplesamlphp\n\
  \  scope: snu.ac.kr\n  entity_categories:\n    - id: http://refeds.org/category/research-and-scholarship\n      name: REFEDS Research and Scholarship\n      description: >-\n        By supporting the R&S entity category, SNU's IdP commits to releasing the R&S\n        minimal attribute bundle — persistent non-reassigned identifier, person name,\n        email address, and eduPersonScopedAffiliation — to any R&S-tagged Service\n        Provider in the federation without a bilateral agreement. This is the closest\n        thing SNU operates to a published authorization scope, and it is the mechanism\n        by which an SNU identity works at a research service run by someone else.\n      source: authentication/snu-kafe-saml-idp-metadata.xml\n  assurance:\n    - id: https://refeds.org/sirtfi\n      name: Sirtfi v1\n      description: >-\n        Security Incident Response Trust Framework for Federated Identity. SNU asserts\n        Sirtfi compliance and publishes a security contact (ym0427@snu.ac.kr)\
  \ in its\n        metadata — a real, machine-readable incident-response commitment.\n      source: authentication/snu-kafe-saml-idp-metadata.xml\n  name_id_formats:\n    - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n  notes: >-\n    Only the transient NameID format is advertised, so SNU does not hand a relying party\n    a stable subject identifier through NameID; persistent correlation, where R&S applies,\n    comes through released attributes instead.\npublic_surfaces:\n  - url: https://s-space.snu.ac.kr/oai/request\n    scopes: []\n    note: Anonymous. No authorization model — every record the repository publishes is world-readable.\n  - url: https://kossda.snu.ac.kr/oai/request\n    scopes: []\n    note: Anonymous.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snu/refs/heads/main/scopes/snu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- South Korea
- Research
- Research Data
- Institutional Repository
- Research Repository
- Identity Federation
- OAI-PMH
- SAML
- Open Access
- Library
- National University
token_urls: []
---
