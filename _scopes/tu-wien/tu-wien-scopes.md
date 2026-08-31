---
api_specs:
- filename: tu-wien-fundify-api-openapi.yml
  format: yaml
  label: FUNDify — RIS Synergy Funding API
  slug: fundify-funding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-wien/refs/heads/main/openapi/tu-wien-fundify-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Tu Wien Scopes
name_suffix: OAuth Scopes
note: No TU Wien surface publishes a scope catalogue. The entries below are the access boundaries we could actually observe, expressed as scopes; they are OUR reading of observed behaviour, not TU Wien's declaration.
overview: 'TU Wien uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TU Wien
provider_slug: tu-wien
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tu-wien-scopes
source_filename: tu-wien-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: derived\nsource: openapi/_original/tu-wien-fundify-api-openapi.yml + probed OIDC discovery document\nnote: >-\n  No TU Wien surface publishes a scope catalogue. The entries below are the access boundaries we\n  could actually observe, expressed as scopes; they are OUR reading of observed behaviour, not\n  TU Wien's declaration.\nscopes:\n  - name: researchdata:read\n    surface: tu-wien:researchdata-api\n    x-operator: institution\n    grant: anonymous\n    covers: [ GET /api/records, GET /api/communities, GET /api/vocabularies/*, GET /api/affiliations, GET /api/funders ]\n    evidence: probed 200 on 2026-08-30\n  - name: researchdata:names\n    surface: tu-wien:researchdata-api\n    x-operator: institution\n    grant: authenticated\n    covers: [ GET /api/names ]\n    evidence: probed 403 anonymously on 2026-08-30\n  - name: researchdata:write\n    surface: tu-wien:researchdata-api\n    x-operator: institution\n    grant: personal access\
  \ token (bearer)\n    covers: [ draft creation, file upload, curation request submission ]\n    evidence: stated at https://researchdata.tuwien.ac.at/tuw/about/api (200)\n  - name: fundify:funding.read\n    surface: tu-wien:fundify-funding\n    x-operator: institution\n    grant: OIDC bearer token\n    covers:\n      - GET /api/ris-synergy/funding/v1/fundings\n      - GET /api/ris-synergy/funding/v1/fundings/{fundingRisId}\n      - GET /api/ris-synergy/funding/v1/annotated-calls/university/{universityRisId}\n      - GET /api/ris-synergy/funding/v1/annotated-calls/university/{universityRisId}/call/{callRisId}\n    evidence: probed 401 anonymously on 2026-08-30\noidc_scopes_advertised:\n  source: https://ris-synergy.csd.tuwien.ac.at/auth/realms/ris-synergy/.well-known/openid-configuration\n  status: 200\n  note: >-\n    The realm advertises the Keycloak default scope set (openid, profile, email, roles, and the\n    standard OIDC extras). No RIS Synergy resource scopes are advertised there.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-wien/refs/heads/main/scopes/tu-wien-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Technical University
- Austria
- Europe
- Research Data
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- Research Computing
- InvenioRDM
- DataCite
- ORCID
- SAML
- RIS Synergy
token_urls: []
---
