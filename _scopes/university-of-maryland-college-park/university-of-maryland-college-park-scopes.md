---
api_specs:
- filename: university-of-maryland-college-park-libraries-website-tools-openapi.yml
  format: yaml
  label: UMD Libraries Website Tools API
  slug: libraries-website-tools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-maryland-college-park/refs/heads/main/openapi/university-of-maryland-college-park-libraries-website-tools-openapi.yml
authorization_urls: []
description: Scope inventory for the University of Maryland's institution-operated API surfaces. There are no scopes to inventory. The library and repository surfaces are keyless and read-only, so authorisation there is all-or-nothing at the endpoint rather than partitioned by scope; the one credentialed surface, the campus Enterprise GIS, gates access with an ArcGIS token whose privileges come from a UMD Portal account role, which is not a scope either. This record exists so the absence is a measured finding rather than an untested assumption.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Maryland College Park Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Maryland College Park uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Maryland College Park
provider_slug: university-of-maryland-college-park
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: university-of-maryland-college-park-scopes
source_filename: university-of-maryland-college-park-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live requests plus the OpenAPI at https://api.www.lib.umd.edu/api/libtools/openapi.json\nx-operator: institution\nprovider: University of Maryland College Park\nproviderId: university-of-maryland-college-park\ndescription: >-\n  Scope inventory for the University of Maryland's institution-operated API surfaces. There are\n  no scopes to inventory. The library and repository surfaces are keyless and read-only, so\n  authorisation there is all-or-nothing at the endpoint rather than partitioned by scope; the one\n  credentialed surface, the campus Enterprise GIS, gates access with an ArcGIS token whose privileges\n  come from a UMD Portal account role, which is not a scope either. This record exists so the absence\n  is a measured finding rather than an untested assumption.\nscopes: []\nfindings:\n- surface: UMD Libraries Website Tools API\n  scopes_declared: 0\n  reason: no_auth\n  detail: >-\n    No securitySchemes in the contract\
  \ and no credential accepted or required on any of the 13\n    GET operations.\n- surface: OAI-PMH endpoints (fcrepo, av, archives)\n  scopes_declared: 0\n  reason: protocol_has_no_scopes\n  detail: >-\n    OAI-PMH 2.0 partitions harvesting by setSpec, not by authorisation scope. ListSets is open\n    on all three endpoints.\n- surface: UMD Enterprise GIS — ArcGIS REST Services\n  scopes_declared: 0\n  reason: token_not_scoped\n  detail: >-\n    ArcGIS Server tokens carry the privileges of the Portal account that requested them; there is no\n    scope parameter on generateToken and no per-service scope vocabulary to enumerate. The service\n    catalog root is readable with no token at all, and every folder beneath it returns error 499.\n- surface: UMD Shibboleth Identity Provider\n  scopes_declared: 0\n  reason: not_an_oauth_server\n  detail: >-\n    SAML 2.0 releases attributes under entity categories, not OAuth scopes. UMD asserts the\n    InCommon and REFEDS Research and Scholarship\
  \ categories, which govern attribute release to\n    federated service providers rather than API authorisation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-maryland-college-park/refs/heads/main/scopes/university-of-maryland-college-park-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United States
- Maryland
- Public Research University
- Land Grant
- Big Ten
- Library
- Research Data
- Digital Collections
- Identity Federation
- OAI-PMH
- Open Data
- Geospatial
token_urls: []
---
