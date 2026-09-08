---
api_specs:
- filename: centene-fhir-patient-access-openapi.json
  format: json
  label: Centene FHIR Patient Access API
  slug: centene-fhir-patient-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-fhir-patient-access-openapi.json
- filename: centene-fhir-provider-directory-openapi.json
  format: json
  label: Centene FHIR Provider Directory API
  slug: centene-fhir-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-fhir-provider-directory-openapi.json
- filename: centene-provider-rtr-fhir-pdex-openapi.json
  format: json
  label: Centene Provider RTR - FHIR PDEX Directory API
  slug: centene-fhir-pdex-rtr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-rtr-fhir-pdex-openapi.json
- filename: centene-provider-rtr-demographics-openapi.json
  format: json
  label: Centene Provider RTR Demographics API
  slug: centene-provider-rtr-demographics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-rtr-demographics-openapi.json
- filename: centene-pces-openapi.yaml
  format: yaml
  label: Centene Provider Carrier Entity Search (PCES) API
  slug: centene-pces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-pces-openapi.yaml
- filename: centene-pces-extract-openapi.yaml
  format: yaml
  label: Centene Provider Carrier Entity Search (PCES) Extract API
  slug: centene-pces-extract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-pces-extract-openapi.yaml
- filename: centene-provider-search-suggest-openapi.yaml
  format: yaml
  label: Centene Provider Search Suggest API
  slug: centene-provider-search-suggest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-search-suggest-openapi.yaml
- filename: centene-product-mapping-v2-openapi.yaml
  format: yaml
  label: Centene Product Mapping V2 API
  slug: centene-product-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-product-mapping-v2-openapi.yaml
- filename: centene-edi-core-realtime-openapi.json
  format: json
  label: Centene LWC EDI CORE Real Time Service
  slug: centene-edi-core-realtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-edi-core-realtime-openapi.json
- filename: centene-ccm-communication-openapi.json
  format: json
  label: Centene CCM Communication API
  slug: centene-ccm-communication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-ccm-communication-openapi.json
- filename: centene-ccm-sms-userresponse-openapi.json
  format: json
  label: Centene CCM SMS User Response Webhook
  slug: centene-ccm-sms-userresponse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-ccm-sms-userresponse-openapi.json
- filename: centene-healow-health-openapi.yaml
  format: yaml
  label: Centene Healow Health API
  slug: centene-healow-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-healow-health-openapi.yaml
authorization_urls: []
description: ''
docs: https://partners.centene.com/apiDetail/2718669d-6e2e-42b5-8c90-0a82f13a30ba
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Centene Scopes
name_suffix: OAuth Scopes
note: Read from Centene's own OpenID Provider Metadata document, served anonymously at partners.centene.com/.well-known/openid-configuration and again from the issuer https://sso.entrykeyid.com. This supersedes the single `resource.READ` scope derivable from the two Provider RTR OpenAPI oauth2 blocks - the discovery document publishes 74 scopes, including the complete SMART on FHIR v2 patient-compartment read family the CMS Patient Access API actually uses. Centene's Patient Access getting-started guide confirms the member authorization flow requests `patient/*.read` and `openid`, and returns a token whose granted scope string is `Patient/*.read launch/patient offline_access`.
overview: 'Centene uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Centene
provider_slug: centene
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: centene-scopes
source_filename: centene-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://partners.centene.com/.well-known/openid-configuration\ndocs: https://partners.centene.com/apiDetail/2718669d-6e2e-42b5-8c90-0a82f13a30ba\nprovider: Centene\nproviderId: centene\nnote: >-\n  Read from Centene's own OpenID Provider Metadata document, served anonymously at\n  partners.centene.com/.well-known/openid-configuration and again from the issuer\n  https://sso.entrykeyid.com. This supersedes the single `resource.READ` scope derivable from the\n  two Provider RTR OpenAPI oauth2 blocks - the discovery document publishes 74 scopes,\n  including the complete SMART on FHIR v2 patient-compartment read family the CMS Patient Access\n  API actually uses. Centene's Patient Access getting-started guide confirms the member\n  authorization flow requests `patient/*.read` and `openid`, and returns a token whose granted\n  scope string is `Patient/*.read launch/patient offline_access`.\nauthorization_server:\n  issuer: https://sso.entrykeyid.com\n\
  \  authorization_endpoint: https://sso.entrykeyid.com/as/authorization.oauth2\n  token_endpoint: https://sso.entrykeyid.com/as/token.oauth2\n  jwks_uri: https://sso.entrykeyid.com/pf/JWKS\n  userinfo_endpoint: https://sso.entrykeyid.com/idp/userinfo.openid\n  introspection_endpoint: https://sso.entrykeyid.com/as/introspect.oauth2\n  revocation_endpoint: https://sso.entrykeyid.com/as/revoke_token.oauth2\n  registration_endpoint: https://sso.entrykeyid.com/as/clients.oauth2\n  sandbox_issuer: https://sandbox.entrykeyid.com\n  pkce: [S256, plain]\n  software: Ping Identity PingFederate\ngrant_types_supported:\n  - \"implicit\"\n  - \"authorization_code\"\n  - \"refresh_token\"\n  - \"password\"\n  - \"client_credentials\"\n  - \"urn:pingidentity.com:oauth2:grant_type:validate_bearer\"\n  - \"urn:ietf:params:oauth:grant-type:jwt-bearer\"\n  - \"urn:ietf:params:oauth:grant-type:saml2-bearer\"\n  - \"urn:ietf:params:oauth:grant-type:device_code\"\n  - \"urn:ietf:params:oauth:grant-type:token-exchange\"\
  \n  - \"urn:openid:params:grant-type:ciba\"\nscope_count: 74\nsmart_on_fhir:\n  implementation_guide: HL7 SMART App Launch Framework 2.0.0\n  launch_modes_supported: [standalone]\n  launch_modes_not_supported: [ehr-launch]\n  note: >-\n    Centene's own getting-started guide states the API implements the SMART standalone launch flow\n    only, and explicitly does not implement SMART EHR Launch.\n  scopes:\n  - scope: \"patient/*.read\"\n    description: \"SMART on FHIR - read every FHIR resource in the authorizing patient compartment.\"\n  - scope: \"patient/AllergyIntolerance.read\"\n    description: \"SMART on FHIR - read AllergyIntolerance resources in the authorizing patient compartment.\"\n  - scope: \"patient/CarePlan.read\"\n    description: \"SMART on FHIR - read CarePlan resources in the authorizing patient compartment.\"\n  - scope: \"patient/CareTeam.read\"\n    description: \"SMART on FHIR - read CareTeam resources in the authorizing patient compartment.\"\n  - scope: \"patient/Coverage.read\"\
  \n    description: \"SMART on FHIR - read Coverage resources in the authorizing patient compartment.\"\n  - scope: \"patient/DiagnosticReport.read\"\n    description: \"SMART on FHIR - read DiagnosticReport resources in the authorizing patient compartment.\"\n  - scope: \"patient/Encounter.read\"\n    description: \"SMART on FHIR - read Encounter resources in the authorizing patient compartment.\"\n  - scope: \"patient/ExplanationOfBenefit.read\"\n    description: \"SMART on FHIR - read ExplanationOfBenefit resources in the authorizing patient compartment.\"\n  - scope: \"patient/Gaps.read\"\n    description: \"SMART on FHIR - read Gaps resources in the authorizing patient compartment.\"\n  - scope: \"patient/Goal.read\"\n    description: \"SMART on FHIR - read Goal resources in the authorizing patient compartment.\"\n  - scope: \"patient/Immunization.read\"\n    description: \"SMART on FHIR - read Immunization resources in the authorizing patient compartment.\"\n  - scope: \"patient/Location.read\"\
  \n    description: \"SMART on FHIR - read Location resources in the authorizing patient compartment.\"\n  - scope: \"patient/Medication.read\"\n    description: \"SMART on FHIR - read Medication resources in the authorizing patient compartment.\"\n  - scope: \"patient/MedicationRequest.read\"\n    description: \"SMART on FHIR - read MedicationRequest resources in the authorizing patient compartment.\"\n  - scope: \"patient/Observation.read\"\n    description: \"SMART on FHIR - read Observation resources in the authorizing patient compartment.\"\n  - scope: \"patient/Organization.read\"\n    description: \"SMART on FHIR - read Organization resources in the authorizing patient compartment.\"\n  - scope: \"patient/Patient.read\"\n    description: \"SMART on FHIR - read Patient resources in the authorizing patient compartment.\"\n  - scope: \"patient/Practitioner.read\"\n    description: \"SMART on FHIR - read Practitioner resources in the authorizing patient compartment.\"\n  - scope: \"\
  patient/Procedure.read\"\n    description: \"SMART on FHIR - read Procedure resources in the authorizing patient compartment.\"\n  - scope: \"patient/Provenance.read\"\n    description: \"SMART on FHIR - read Provenance resources in the authorizing patient compartment.\"\nplatform_scopes:\n  note: >-\n    The remaining scopes in scopes_supported belong to the shared EntryKey ID tenant - identity\n    administration, profile claims, event and data-platform scopes. They are published by the same\n    authorization server but are not part of the public interoperability API surface. Recorded as\n    fetched; descriptions are not published by Centene.\n  scopes:\n  - scope: \"FName\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"Idaas\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"LName\"\n    description: \"Published\
  \ in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"LastLoginTime\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"MDM_UMPI.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"PCSentitlements\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"PingUUID\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"address\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"cn\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope:\
  \ \"email\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"guid\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"hniAliasName\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"hniIsDisabled\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"hniUserType\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"hniuid\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Accounts.delete\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID\
  \ provider; description not published.\"\n  - scope: \"idaas/Clients.create\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Clients.delete\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Clients.edit\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Clients.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Clients.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Identities.create\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n\
  \  - scope: \"idaas/Identities.delete\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Identities.edit\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Identities.proof\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Identities.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Identities.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Profiles.create\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Profiles.delete\"\
  \n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Profiles.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Profiles.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"idaas/Registration.create\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"memberOf\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"name\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"openid\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID\
  \ OpenID provider; description not published.\"\n  - scope: \"pcs/entitlements.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"pcs/entitlements.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"phone\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"prisma-microseg\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"prisma-microseg/Ruleset.delete\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"prisma-microseg/Ruleset.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\
  \n  - scope: \"prisma-microseg/Ruleset.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"profile\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"resource.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"resource.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"service\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"sn\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"snowflake/Data.read\"\n    description: \"Published in scopes_supported by\
  \ the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"user_type\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"web/member/delete\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"xp/Events.create\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"xp/Events.delete\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"xp/Events.read\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n  - scope: \"xp/Events.write\"\n    description: \"Published in scopes_supported by the Centene EntryKey ID OpenID provider; description not published.\"\n\
  per_api_scopes:\n  note: >-\n    The partner portal's own API catalogue records the scopes and grant types each published API\n    requires. Read anonymously from external-api.my.centene.com/partner-portal/apis.\n  entries:\n    - api: FHIR - Patient Access\n      grant_types: ['Authorization Code (Resource Server)']\n      scopes: ['patient/*.read', openid]\n      audience: patientaccess\n    - api: FHIR - Provider Directory\n      grant_types: []\n      scopes: []\n      authentication: none\n      note: Public and unauthenticated. No scope surface.\n    - api: Provider RTR - FHIR PDEX Directory API (External)\n      grant_types: ['Client Credentials (Service Account)']\n      scopes: [resource.read, openid]\n      audience: prtrdemographic\n    - api: Provider RTR - Demographics API\n      grant_types: ['Client Credentials (Service Account)']\n      scopes: [resource.read]\n      audience: prtrdemographic\n    - api: Provider Carrier Entity Search (PCES) API\n      grant_types: ['Client\
  \ Credentials (Service Account)']\n      scopes: [openid, resource.read]\n      audience: ewsext\n    - api: Product Mapping V2\n      grant_types: ['Authorization Code (Resource Server)', 'Authorization Code + PKCE (SPA)', 'Client Credentials (Service Account)']\n      scopes: [openid]\n      audience: ewsext\n    - api: LWC EDI CORE REAL TIME SERVICE\n      grant_types: ['Client Credentials (Service Account)']\n      scopes: [resource.read, profile, openid]\n      audience: edicorertservice\nderived_from_spec:\n  note: >-\n    Retained from the OpenAPI derivation for traceability. Both Provider RTR specs declare a single\n    clientCredentials flow with one scope.\n  token_url: https://stage.entrykeyid.com/as/token.oauth2\n  scopes:\n    - scope: resource.READ\n      description: read access\n      sources:\n        - openapi/centene-provider-rtr-demographics-openapi.json\n        - openapi/centene-provider-rtr-fhir-pdex-openapi.json\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/scopes/centene-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- Insurance
- Managed Care
- FHIR
- HL7
- CMS Interoperability
- Patient Access
- Provider Directory
- Payer
- Medicaid
- Medicare
- Interoperability
- SMART on FHIR
- PDEX
- CARIN Blue Button
- US Core
- Formulary
- X12
- EDI
- Fortune 500
token_urls: []
---
