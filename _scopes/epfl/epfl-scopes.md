---
api_specs:
- filename: epfl-actu.yaml
  format: yaml
  label: EPFL Actu News API
  slug: actu-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/_original/epfl-actu.yaml
- filename: epfl-memento.yaml
  format: yaml
  label: EPFL Memento Events API
  slug: memento-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/_original/epfl-memento.yaml
- filename: epfl-getprime-api-openapi.yml
  format: yaml
  label: EPFL GETprime qPCR Primer API
  slug: getprime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/openapi/epfl-getprime-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Epfl Scopes
name_suffix: OAuth Scopes
note: EPFL operates NO OAuth 2.0 or OpenID Connect authorization server that is reachable from the public internet — no /.well-known/openid-configuration is served on any EPFL host probed on 2026-08-19, and neither public API declares an oauth2 security scheme. So there are no OAuth scopes to record, and inventing some would be fabrication. What EPFL does operate is a SAML attribute-release surface, and that is the institution's real authorization vocabulary. It is published in the SWITCHaai federation metadata and is recorded here in its place.
overview: 'EPFL uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EPFL
provider_slug: epfl
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: epfl-scopes
source_filename: epfl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  openapi/_original/epfl-actu.yaml, openapi/_original/epfl-memento.yaml,\n  and the SWITCHaai federation metadata aggregate\n  https://metadata.aai.switch.ch/metadata.switchaai.xml\nx-operator: institution\nnote: >-\n  EPFL operates NO OAuth 2.0 or OpenID Connect authorization server that is reachable from the\n  public internet — no /.well-known/openid-configuration is served on any EPFL host probed on\n  2026-08-19, and neither public API declares an oauth2 security scheme. So there are no OAuth\n  scopes to record, and inventing some would be fabrication. What EPFL does operate is a SAML\n  attribute-release surface, and that is the institution's real authorization vocabulary. It is\n  published in the SWITCHaai federation metadata and is recorded here in its place.\noauth:\n  present: false\n  evidence: >-\n    No oauth2 or openIdConnect securityScheme in any EPFL contract; the only schemes the public\n    APIs declare\
  \ are DRF tokenAuth (apiKey in header, \"Authorization: Token <key>\") and\n    basicAuth. Both public APIs are read-only and answer unauthenticated (Allow: GET, HEAD,\n    OPTIONS).\nsaml_attribute_release:\n  federation: SWITCHaai (SWITCH edu-ID), exported to eduGAIN\n  idp_entity_id: https://idp.epfl.ch/idp/shibboleth\n  idp_entity_categories:\n  - http://refeds.org/category/research-and-scholarship\n  - https://refeds.org/sirtfi\n  service_providers:\n  - entity_id: https://tequila.epfl.ch/shibboleth\n    operator: institution\n    status: stale\n    status_note: >-\n      Registered in the federation aggregate, but tequila.epfl.ch does not resolve in public DNS as\n      of 2026-08-19 (empty answer from 8.8.8.8 and 1.1.1.1). The attribute-release request below is\n      real published metadata; the service behind it is not publicly reachable.\n    acs: https://tequila.epfl.ch/Shibboleth.sso/SAML2/POST\n    requested_attributes:\n    - {friendly_name: uid, oid: urn:oid:0.9.2342.19200300.100.1.1}\n\
  \    - {friendly_name: email, oid: urn:oid:0.9.2342.19200300.100.1.3}\n    - {friendly_name: givenName, oid: urn:oid:2.5.4.42}\n    - {friendly_name: surname, oid: urn:oid:2.5.4.4}\n    - {friendly_name: displayName, oid: urn:oid:2.16.840.1.113730.3.1.241}\n    - {friendly_name: eduPersonAffiliation, oid: 'urn:oid:1.3.6.1.4.1.5923.1.1.1.1'}\n    - {friendly_name: eduPersonTargetedID, oid: 'urn:oid:1.3.6.1.4.1.5923.1.1.1.10'}\n    - {friendly_name: eduPersonPrimaryOrgUnitDN, oid: 'urn:oid:1.3.6.1.4.1.5923.1.1.1.8'}\n    - {friendly_name: swissEduPersonUniqueID, oid: 'urn:oid:2.16.756.1.2.5.1.1.1'}\n    - {friendly_name: swissEduPersonHomeOrganization, oid: 'urn:oid:2.16.756.1.2.5.1.1.4'}\n    - {friendly_name: swissEduPersonHomeOrganizationType, oid: 'urn:oid:2.16.756.1.2.5.1.1.5'}\n    - {friendly_name: swissEduPersonStudyBranch3, oid: 'urn:oid:2.16.756.1.2.5.1.1.8'}\n    - {friendly_name: swissEduPersonStudyLevel, oid: 'urn:oid:2.16.756.1.2.5.1.1.9'}\n    - {friendly_name: swissEduPersonStaffCategory,\
  \ oid: 'urn:oid:2.16.756.1.2.5.1.1.10'}\n    - {friendly_name: swissEduPersonMatriculationNumber, oid: 'urn:oid:2.16.756.1.2.5.1.1.11'}\n    - {friendly_name: swissEduPersonCardUID, oid: 'urn:oid:2.16.756.1.2.5.1.1.12'}\n  - entity_id: https://companion.epfl.ch/shibboleth\n    operator: institution\n    status: live\n    status_note: 'companion.epfl.ch resolves to 128.178.218.80 and returns HTTP 200 (probed 2026-08-19).'\n    acs: https://companion.epfl.ch/Shibboleth.sso/SAML2/POST\n    requested_attributes:\n    - {friendly_name: eduPersonAffiliation, oid: 'urn:oid:1.3.6.1.4.1.5923.1.1.1.1'}\n    - {friendly_name: eduPersonScopedAffiliation, oid: 'urn:oid:1.3.6.1.4.1.5923.1.1.1.9'}\n    - {friendly_name: eduPersonTargetedID, oid: 'urn:oid:1.3.6.1.4.1.5923.1.1.1.10'}\n    - {friendly_name: email, oid: urn:oid:0.9.2342.19200300.100.1.3}\n    - {friendly_name: givenName, oid: urn:oid:2.5.4.42}\n    - {friendly_name: surname, oid: urn:oid:2.5.4.4}\n    - {friendly_name: swissEduPersonUniqueID,\
  \ oid: 'urn:oid:2.16.756.1.2.5.1.1.1'}\n    - {friendly_name: swissEduPersonHomeOrganization, oid: 'urn:oid:2.16.756.1.2.5.1.1.4'}\n    - {friendly_name: swissEduPersonHomeOrganizationType, oid: 'urn:oid:2.16.756.1.2.5.1.1.5'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epfl/refs/heads/main/scopes/epfl-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Technical University
- Research
- Research Repository
- Open Access
- Identity Federation
- News
- Event
- Switzerland
- Europe
token_urls: []
---
