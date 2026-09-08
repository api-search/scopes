---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Infact Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'InFact uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: InFact
provider_slug: infact
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: infact-scopes
source_filename: infact-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://cran.r-project.org/package=HPZoneAPI (HPZoneAPI 1.3.0, MIT, published 2026-04-09) — R\n  client for the HPZone API; its own documentation states the client_id/client_secret are \"as supplied\n  by InFact\"\napi: HPZone API (GraphQL)\nprovider: InFact\nflow: oauth2 client_credentials\ntoken_endpoint: https://connect.govconext.nl/oidc/token\nnotes:\n- HPZone carries TWO named scopes. They are supplied to the token endpoint by the OAuth2 client-credentials\n  flow AND echoed on each data request as a custom `scope:` HTTP header, per the published R client.\n- 'The scope boundary is a data-protection boundary, not a functional one: every one of the 248 documented\n  fields is readable under `extended`, while `standard` withholds the 92 fields that carry directly-identifying\n  or special-category personal data (name, GP details, ethnic origin, clinical conditions, staff identifiers).'\n- Scope names are configurable per\
  \ deployment (HPZone_setup(standard=, extended=)); \"standard\" and \"extended\"\n  are the package defaults and the values used by the Dutch national deployment.\nscopes:\n- name: standard\n  description: Read access to the pseudonymised subset of every HPZone entity — epidemiological, workflow\n    and geographic fields with directly-identifying and special-category personal data withheld.\n  field_count: 156\n- name: extended\n  description: Read access to the complete field set, including directly-identifying personal data (names,\n    GP practice and address, telephone) and special-category health data (clinical conditions, ethnic\n    origin) on Cases and Contacts.\n  field_count: 248\nby_endpoint:\n- endpoint: Actions\n  fields_total: 15\n  readable_with_standard: 15\n  requires_extended: 0\n  extended_only_fields: []\n- endpoint: Cases\n  fields_total: 113\n  readable_with_standard: 58\n  requires_extended: 55\n  extended_only_fields:\n  - Aanvullende_informatie_over_de_melder\n\
  \  - Additional_comments_on_the_nature_of_the_contact_with_index_case\n  - Age_in_months\n  - Case_manager_identifier\n  - Diabetes_mellitus\n  - Entered_by_identifier\n  - Ethnic_origin\n  - Family_name\n  - First_name\n  - Full_name\n  - Gp\n  - Gp_address1\n  - Gp_address2\n  - Gp_address3\n  - Gp_address4\n  - Gp_postcode\n  - Gp_practice_die_de_casus_gediagnosticeerd_heeft\n  - Gp_telephone\n  - Hartaandoening\n  - Huisarts_die_de_casus_gediagnosticeerd_heeft\n  - Immuungecompromitteerd\n  - Import_source\n  - Indicate_other_risk_factors\n  - Intravenous_drug_user\n  - Investigating_officer\n  - Investigating_officer_identifier\n  - Latitude\n  - Leveraandoening\n  - Longitude\n  - Luchtwegaandoening\n  - Maligniteit\n  - Midwife\n  - Midwife_address1\n  - Midwife_address2\n  - Midwife_address3\n  - Midwife_address4\n  - Midwife_postcode\n  - Midwife_practice\n  - Midwife_telephone\n  - Mogelijk_declarabele_zorg\n  - Mogelijke_bron_in_Nederland_buitenshuis\n  - Mogelijke_bron_in_buitenland\n\
  \  - Mogelijke_bron_in_zorginstelling_in_Nederland\n  - Newborn\n  - Nieraandoening\n  - Number_or_building\n  - Practice\n  - Pregnant\n  - Relationship_to_the_above_case\n  - Salmonella_subspecies\n  - Sputumkweek_gedaan\n  - Tussenvoegsel\n  - Works_in_education\n  - Works_in_health_care\n  - Works_with_food\n- endpoint: Contacts\n  fields_total: 60\n  readable_with_standard: 23\n  requires_extended: 37\n  extended_only_fields:\n  - Age_in_months\n  - Any_underlying_medical_condition\n  - Case_manager_identifier\n  - Entered_by_identifier\n  - Ethnic_origin\n  - Family_name\n  - First_name\n  - Full_name\n  - Gp\n  - Gp_address1\n  - Gp_address2\n  - Gp_address3\n  - Gp_address4\n  - Gp_postcode\n  - Gp_telephone\n  - Indicate_other_risk_factors\n  - Intravenous_drug_user\n  - Investigating_officer\n  - Investigating_officer_identifier\n  - Midwife\n  - Midwife_address1\n  - Midwife_address2\n  - Midwife_address3\n  - Midwife_address4\n  - Midwife_postcode\n  - Midwife_practice\n  -\
  \ Midwife_telephone\n  - Mogelijk_declarabele_zorg\n  - Newborn\n  - Number_or_building\n  - Practice\n  - Pregnant\n  - Relationship_to_the_above_case\n  - Tussenvoegsel\n  - Works_in_education\n  - Works_in_health_care\n  - Works_with_food\n- endpoint: Contexts\n  fields_total: 12\n  readable_with_standard: 12\n  requires_extended: 0\n  extended_only_fields: []\n- endpoint: Enquiries\n  fields_total: 18\n  readable_with_standard: 18\n  requires_extended: 0\n  extended_only_fields: []\n- endpoint: Situations\n  fields_total: 30\n  readable_with_standard: 30\n  requires_extended: 0\n  extended_only_fields: []\ndocs: null\ndocs_note: InFact publishes no public scope reference. The scope model above is read from the published\n  CRAN client and its HPZone_necessary_scope() field table; the provider-side documentation is customer-only\n  (see x-coverage in apis.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infact/refs/heads/main/scopes/infact-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Health
- Public Health
- Healthcare
- Epidemiology
- Disease Surveillance
- Outbreak Management
- Contact Tracing
- Electronic Health Records
- openEHR
- GraphQL
- Government
token_urls: []
---
