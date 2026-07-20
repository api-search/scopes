---
authorization_urls: []
description: ''
docs: https://curanahealth.com/interoperability-api/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Curana Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Curana Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Curana Health
provider_slug: curana-health
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: curana-health-scopes
source_filename: curana-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://curanahealth.com/wp-content/uploads/2026/04/3rd_PARTY_CMS_APIS_v2.2.pdf\ndocs: https://curanahealth.com/interoperability-api/\nmodel: >-\n  Access tokens carry explicitly-declared scopes that determine the resources an\n  application may access; wildcards are not supported. The Third-Party Application Owner\n  User Guide documents two scope groups. Exact scope strings are not reproduced verbatim\n  here to avoid fabrication; each group is described by the FHIR resources it governs and\n  the scope count published in the guide.\nscope_groups:\n- name: Public Access\n  count: 8\n  authorization: none (public Provider Directory per CMS-9115-F)\n  covers_resources:\n  - Practitioner\n  - PractitionerRole\n  - Organization\n  - Location\n  - InsurancePlan\n  - MedicationKnowledge\n  - Medication\n  - List\n- name: Patient Access\n  count: 12\n  authorization: OAuth 2.0 member consent required\n  covers_resources:\n  - Patient\n\
  \  - Coverage\n  - ExplanationOfBenefit\n  - Condition\n  - AllergyIntolerance\n  - Immunization\n  - CarePlan\n  - CareTeam\n  - Goal\n  - Observation\n  - Procedure\n  - MedicationRequest\n  - DocumentReference\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curana-health/refs/heads/main/scopes/curana-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Digital Health
- Healthcare
- FHIR
- Interoperability
- Medicare Advantage
- Senior Living
- Patient Access
- Value-Based Care
- CMS-9115-F
token_urls: []
---
