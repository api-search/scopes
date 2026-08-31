---
api_specs:
- filename: yale-search-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Search API
  slug: yale-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-search-api-openapi.yml
- filename: yale-documents-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Documents API
  slug: yale-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-documents-api-openapi.yml
- filename: yale-facets-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Facets API
  slug: yale-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-facets-api-openapi.yml
- filename: yale-related-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Related API
  slug: yale-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-related-api-openapi.yml
- filename: yale-configuration-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Configuration API
  slug: yale-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-configuration-api-openapi.yml
- filename: yale-federation-api-openapi.yml
  format: yaml
  label: Yale University Federation API
  slug: yale-federation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-federation-api-openapi.yml
- filename: yale-iiif-api-openapi.yml
  format: yaml
  label: Yale University IIIF API
  slug: yale-iiif-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-iiif-api-openapi.yml
- filename: yale-info-api-openapi.yml
  format: yaml
  label: Yale University Info API
  slug: yale-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-info-api-openapi.yml
authorization_urls: []
description: 'Authorization granularity across Yale University''s surfaces. This artifact records an ABSENCE deliberately rather than inventing a scope vocabulary: Yale''s public tier has no authorization layer to describe, and Yale''s private tier partitions access by provisioning decision rather than by a machine-readable scope.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Yale Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Yale University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yale University
provider_slug: yale
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: yale-scopes
source_filename: yale-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: >-\n  Derived from authentication/yale-authentication.yml, which is itself probed. No OAuth\n  authorization server, no scope document and no consent screen was found on any Yale-operated\n  host on 2026-08-19.\ndescription: >-\n  Authorization granularity across Yale University's surfaces. This artifact records an ABSENCE\n  deliberately rather than inventing a scope vocabulary: Yale's public tier has no authorization\n  layer to describe, and Yale's private tier partitions access by provisioning decision rather\n  than by a machine-readable scope.\nscopes:\n  model: none\n  oauth2: not_found\n  openid_connect: not_found\n  note: >-\n    No .well-known/oauth-authorization-server, no .well-known/openid-configuration and no scope\n    enumeration was found on lux.collections.yale.edu, dataverse.yale.edu,\n    collections.library.yale.edu or developers.yale.edu.\nauthorization_partitions:\n- surface: LUX Collections Discovery\
  \ API\n  x-operator: institution\n  partition: none\n  detail: Anonymous read of the whole published corpus. No per-caller authorization exists.\n- surface: Yale Dataverse Repository API\n  x-operator: institution\n  partition: publication state\n  detail: >-\n    Authorization is binary and derived from content state, not from a scope: published content is\n    world-readable, unpublished drafts require an API token bound to a NetID-authenticated account.\n    Dataverse's role model (admin, curator, contributor, file downloader) sits behind that token\n    and is not exposed on any public endpoint.\n- surface: Yale Portal APIs\n  x-operator: institution\n  partition: per-API key registration\n  detail: >-\n    A developer registers an application in the Yale Developer Portal and names the specific APIs\n    it needs. The API key is therefore scoped by enumeration at issue time rather than by an OAuth\n    scope string presented per request.\n- surface: Yale Enterprise (SOA) Services\n\
  \  x-operator: institution\n  partition: service account plus data governance policy\n  detail: >-\n    Yale states each SOA service has \"specific request and data governance policies\" and access is\n    requested per service (People Hub, COA, GetSupervisoryOrgs). The partition is contractual and\n    human-reviewed, not machine-readable.\n- surface: Yale Identity Federation\n  x-operator: institution\n  partition: SAML attribute release\n  detail: >-\n    The closest thing Yale operates to a scope model is attribute release from the Shibboleth IdP\n    to federated service providers, negotiated per relying party through InCommon. The released\n    attribute set is not published in the public metadata document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/scopes/yale-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- Ivy League
- Research
- Research Data
- Research Repository
- Identity Federation
- Library
- Cultural Heritage
- Linked Data
- IIIF
- Course Catalog
token_urls: []
---
