---
api_specs:
- filename: university-of-gottingen-gdz-oai-pmh-openapi.yml
  format: yaml
  label: GDZ OAI-PMH Metadata Harvesting
  slug: gdz-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-gdz-oai-pmh-openapi.yml
- filename: university-of-gottingen-ediss-oai-pmh-openapi.yml
  format: yaml
  label: eDiss Göttingen OAI-PMH Metadata Harvesting
  slug: ediss-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-ediss-oai-pmh-openapi.yml
- filename: university-of-gottingen-sub-iiif-openapi.yml
  format: yaml
  label: SUB Göttingen IIIF Image and Presentation
  slug: sub-iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-sub-iiif-openapi.yml
authorization_urls: []
description: The University of Göttingen defines no API scopes. Its three verified institution-operated surfaces are read-only and anonymous, so there is nothing to scope; the authorisation that does exist is SAML attribute release through DFN-AAI, which is an entitlement model rather than an OAuth scope model. This file exists so that the absence is recorded rather than inferred.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: generated
name: University Of Gottingen Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Göttingen uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Göttingen
provider_slug: university-of-gottingen
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-gottingen-scopes
source_filename: university-of-gottingen-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: University of Göttingen\nproviderId: university-of-gottingen\ngenerated: '2026-08-30'\nmethod: generated\nx-evidence-method: probed\nsource: Live probes of the institution's endpoints on 2026-08-30.\ndescription: >-\n  The University of Göttingen defines no API scopes. Its three verified institution-operated\n  surfaces are read-only and anonymous, so there is nothing to scope; the authorisation that does\n  exist is SAML attribute release through DFN-AAI, which is an entitlement model rather than an\n  OAuth scope model. This file exists so that the absence is recorded rather than inferred.\nscopes: []\nauthorization_model:\n  type: saml-attribute-release\n  detail: >-\n    Access decisions for institutional services are made from SAML attributes released by\n    entityID https://shibboleth-idp.uni-goettingen.de/uni/shibboleth under DFN-AAI policy —\n    eduPersonScopedAffiliation and entitlement rather\
  \ than named API scopes. The entity carries\n    entity categories 4;11;76;112 in the eduGAIN technical database, which is where the\n    release policy is expressed.\n  evidence:\n  - url: https://technical.edugain.org/api.php?action=list_entities&format=json\n    status: 200\nnotes: >-\n  The Stud.IP deployment's REST API uses OAuth consumer credentials issued by the institution but\n  publishes no scope list and no registration flow; anonymous callers receive\n  \"401 Unauthorized (no consumer)\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/scopes/university-of-gottingen-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Germany
- German U15
- Public Research University
- Research Data
- Digital Library
- IIIF
- OAI-PMH
- Identity Federation
- Research Repository
token_urls: []
---
