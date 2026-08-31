---
api_specs:
- filename: university-of-southampton-open-data-linked-data-openapi.yml
  format: yaml
  label: University of Southampton Open Data Service (Linked Data)
  slug: open-data-linked-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/openapi/university-of-southampton-open-data-linked-data-openapi.yml
- filename: university-of-southampton-eprints-oai-pmh-openapi.yml
  format: yaml
  label: ePrints Soton OAI-PMH Interface
  slug: eprints-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/openapi/university-of-southampton-eprints-oai-pmh-openapi.yml
- filename: university-of-southampton-eprints-rest-openapi.yml
  format: yaml
  label: ePrints Soton REST Interface
  slug: eprints-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/openapi/university-of-southampton-eprints-rest-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Southampton Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Southampton uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Southampton
provider_slug: university-of-southampton
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-southampton-scopes
source_filename: university-of-southampton-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Access boundaries observed on 2026-08-30. Recorded because the absence of scopes is itself the\n  finding: none of the University's public surfaces implements an authorization model.\nsummary: >-\n  No OAuth scopes, API keys, plans or quotas exist on any institution-operated surface. Access is\n  binary and anonymous — a resource is either open to everyone or closed to everyone. The only\n  authorization model in the estate is SAML attribute release from the Shibboleth IdP, which\n  governs access to licensed resources and internal systems, not to any API.\n\nscopes:\n\n- surface: Open Data Service\n  x-operator: institution\n  model: anonymous_open\n  scopes: []\n  detail: >-\n    Fully open under the Open Government Licence. No key, no registration, no quota, no\n    rate-limit headers observed.\n\n- surface: ePrints Soton OAI-PMH\n  x-operator: institution\n  model: anonymous_open\n  scopes: []\n  detail: >-\n \
  \   Open harvesting. The repository's metadataPolicy grants free re-use of metadata for\n    not-for-profit purposes with attribution; its dataPolicy permits transient harvesting of full\n    items but requires permission for permanent harvesting and forbids commercial resale. That is\n    a licence boundary, not a technical scope — it is not enforced by the endpoint.\n  policy_boundaries:\n  - Metadata: free re-use, any medium, attribution via OAI identifier.\n  - Full items: transient robot harvesting permitted; permanent harvesting requires permission.\n  - Full items: commercial resale prohibited without formal permission of copyright holders.\n\n- surface: ePrints Soton REST\n  x-operator: institution\n  model: anonymous_open\n  scopes: []\n  detail: Open read of the eprint, user and subject datasets. No write surface is exposed.\n\n- surface: Shibboleth SAML Identity Provider\n  x-operator: institution\n  model: saml_attribute_release\n  scopes: []\n  detail: >-\n    Authorization\
  \ is expressed as SAML attribute release policy per registered service provider,\n    negotiated through the Jisc UK Access Management Federation, not as OAuth scopes. The\n    AttributeAuthorityDescriptor exposes SOAP AttributeQuery at\n    https://webauth.soton.ac.uk:8443/idp/profile/SAML2/SOAP/AttributeQuery. An application cannot\n    obtain an assertion or query attributes without first being registered in the federation, so\n    there is no self-service developer path.\n\n- surface: Elsevier Pure tenancy\n  x-operator: tenant\n  model: closed\n  scopes: []\n  detail: >-\n    Public web services return 403. Where Pure's REST API is enabled it is gated by an api-key\n    header, but that is Elsevier's model and it is switched off on this tenancy.\n\n- surface: Figshare tenancy\n  x-operator: tenant\n  model: vendor_managed\n  scopes: []\n  detail: >-\n    Figshare's own OAuth model applies; it is the vendor's authorization surface, not the\n    University's, and no Southampton-specific\
  \ scope set exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-southampton/refs/heads/main/scopes/university-of-southampton-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Russell Group
- United Kingdom
- Open Data
- Linked Data
- Research Repository
- Identity Federation
- OAI-PMH
- Research
- Course Catalog
token_urls: []
---
