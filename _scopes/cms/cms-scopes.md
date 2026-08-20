---
api_specs:
- filename: cms-bcda-openapi.yml
  format: yaml
  label: CMS Beneficiary Claims Data API (BCDA)
  slug: cms-beneficiary-claims-data-api-bcda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bcda-openapi.yml
- filename: cms-ab2d-openapi.yml
  format: yaml
  label: CMS AB2D API (Claims Data to Part D Sponsors)
  slug: cms-ab2d-api-claims-data-to-part-d-sponsors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-ab2d-openapi.yml
- filename: cms-api-reference-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services API Reference API
  slug: cms-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-api-reference-api-openapi.yml
- filename: cms-bulk-data-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Bulk Data API
  slug: cms-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bulk-data-api-openapi.yml
- filename: cms-code-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Code Search API
  slug: cms-code-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-code-search-api-openapi.yml
- filename: cms-cost-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Cost Search API
  slug: cms-cost-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-cost-search-api-openapi.yml
- filename: cms-enrollments-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Enrollments API
  slug: cms-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-enrollments-api-openapi.yml
- filename: cms-geography-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Geography API
  slug: cms-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-geography-api-openapi.yml
- filename: cms-households-eligibility-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Households & Eligibility API
  slug: cms-households-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-households-eligibility-api-openapi.yml
- filename: cms-insurance-issuers-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Issuers API
  slug: cms-insurance-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-issuers-api-openapi.yml
- filename: cms-insurance-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Plans API
  slug: cms-insurance-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-plans-api-openapi.yml
- filename: cms-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Plans API
  slug: cms-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-plans-api-openapi.yml
- filename: cms-provider-drug-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Provider & Drug Coverage API
  slug: cms-provider-drug-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-provider-drug-coverage-api-openapi.yml
- filename: cms-capability-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Capability API
  slug: centers-for-medicare-and-medicaid-services-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-capability-api-openapi.yml
- filename: cms-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Coverage API
  slug: centers-for-medicare-and-medicaid-services-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-coverage-api-openapi.yml
- filename: cms-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services ExplanationOfBenefit API
  slug: centers-for-medicare-and-medicaid-services-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-explanationofbenefit-api-openapi.yml
- filename: cms-patient-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Patient API
  slug: centers-for-medicare-and-medicaid-services-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-patient-api-openapi.yml
authorization_urls:
- https://api.bluebutton.cms.gov/v2/o/authorize
description: ''
docs: https://bluebutton.cms.gov/api-documentation/authorization/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cms Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Centers for Medicare and Medicaid Services publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Centers for Medicare and Medicaid Services API on a user''s behalf.


  Tokens are issued from https://api.bluebutton.cms.gov/v2/o/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Centers for Medicare and Medicaid Services
provider_slug: cms
schemes:
- api: CMS Blue Button 2.0 API
  description: OAuth 2.0 authorization code flow with mandatory PKCE, used by Medicare enrollees to grant a third-party application access to their own claims data.
  flows:
  - authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize
    client_type: confidential only — public clients and the implicit grant are NOT supported
    flow: authorizationCode
    pkce: required (S256 only)
    revocationUrl: https://api.bluebutton.cms.gov/v2/o/revoke_token
    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token
    userinfoUrl: https://api.bluebutton.cms.gov/v2/connect/userinfo
  name: oauth2
  sandbox_flows:
  - authorizationUrl: https://sandbox.bluebutton.cms.gov/v2/o/authorize
    tokenUrl: https://sandbox.bluebutton.cms.gov/v2/o/token
  source: openapi/_original/cms-cms-blue-button-2-openapi.yml
scope_count: 6
scope_names:
- patient/Patient.rs
- patient/Coverage.rs
- patient/ExplanationOfBenefit.rs
- launch/patient
- openid
- profile
scopes:
- description: Read and search my general patient and demographic information.
  flows:
  - authorizationCode
  scope: patient/Patient.rs
- description: Read and search my Medicare and supplemental coverage information.
  flows:
  - authorizationCode
  scope: patient/Coverage.rs
- description: Read and search my Medicare claim information.
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.rs
- description: Patient launch context (SMART App Launch).
  flows:
  - authorizationCode
  scope: launch/patient
- description: Retrieve information about the currently logged-in user (OpenID Connect).
  flows:
  - authorizationCode
  scope: openid
- description: Access the /UserInfo endpoint (OpenID Connect).
  flows:
  - authorizationCode
  scope: profile
slug: cms-scopes
source_filename: cms-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: openapi/_original/cms-cms-blue-button-2-openapi.yml\ndocs: https://bluebutton.cms.gov/api-documentation/authorization/\ndiscovery: https://api.bluebutton.cms.gov/.well-known/openid-configuration\nupgrade_note: >-\n  Upgraded 2026-08-15 from derived to searched. The 2026-07-11 derived pass captured only the three\n  `.read` scopes present in the spec; the CMS authorization documentation publishes the `.rs` (read +\n  search) aliases CMS actually uses in its own examples, the SMART launch context scope, and the\n  OpenID Connect scopes — none of which appear in any harvested spec.\nsummary: >-\n  Only ONE CMS API has an OAuth scope surface: Blue Button 2.0, the beneficiary-consent API. It uses\n  HL7 FHIR (SMART on FHIR) scopes, all patient-context and all read-only — there is no write scope\n  anywhere in the CMS estate. BCDA, AB2D and DPC use bearer tokens whose authority is derived from\n  programme attribution rather than\
  \ from scopes, and the Marketplace / PPL surface is API-key only.\nschemes:\n  - name: oauth2\n    api: CMS Blue Button 2.0 API\n    source: openapi/_original/cms-cms-blue-button-2-openapi.yml\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize\n        tokenUrl: https://api.bluebutton.cms.gov/v2/o/token\n        revocationUrl: https://api.bluebutton.cms.gov/v2/o/revoke_token\n        userinfoUrl: https://api.bluebutton.cms.gov/v2/connect/userinfo\n        pkce: required (S256 only)\n        client_type: confidential only — public clients and the implicit grant are NOT supported\n    sandbox_flows:\n      - authorizationUrl: https://sandbox.bluebutton.cms.gov/v2/o/authorize\n        tokenUrl: https://sandbox.bluebutton.cms.gov/v2/o/token\n    description: >-\n      OAuth 2.0 authorization code flow with mandatory PKCE, used by Medicare enrollees to grant a\n      third-party application access to their own claims data.\n\
  scopes:\n  - scope: patient/Patient.rs\n    alias: patient/Patient.read\n    description: Read and search my general patient and demographic information.\n    resource: Patient\n    access: read+search\n    flows:\n      - authorizationCode\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\n      - openapi/_original/cms-cms-blue-button-2-openapi.yml\n  - scope: patient/Coverage.rs\n    alias: patient/Coverage.read\n    description: Read and search my Medicare and supplemental coverage information.\n    resource: Coverage\n    access: read+search\n    flows:\n      - authorizationCode\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\n      - openapi/_original/cms-cms-blue-button-2-openapi.yml\n  - scope: patient/ExplanationOfBenefit.rs\n    alias: patient/ExplanationOfBenefit.read\n    description: Read and search my Medicare claim information.\n    resource: ExplanationOfBenefit\n    access: read+search\n    flows:\n  \
  \    - authorizationCode\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\n      - openapi/_original/cms-cms-blue-button-2-openapi.yml\n  - scope: launch/patient\n    description: Patient launch context (SMART App Launch).\n    access: context\n    flows:\n      - authorizationCode\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\n  - scope: openid\n    description: Retrieve information about the currently logged-in user (OpenID Connect).\n    access: identity\n    flows:\n      - authorizationCode\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\n      - https://api.bluebutton.cms.gov/.well-known/openid-configuration\n  - scope: profile\n    description: Access the /UserInfo endpoint (OpenID Connect).\n    access: identity\n    flows:\n      - authorizationCode\n    sources:\n      - https://bluebutton.cms.gov/api-documentation/authorization/\nenrollee_controls:\n  - control: personal-information\
  \ block\n    description: >-\n      Two things independently block an application's access to /Patient and /UserInfo even when the\n      scope was granted: the developer declining to collect enrollee personal information at production\n      approval, and the enrollee choosing during Medicare.gov authentication not to share personal\n      data. An application must be able to operate without the Patient resource — CMS documents pulling\n      the patient id from the authorization response or from the EOB/Coverage bundles instead.\n    source: https://bluebutton.cms.gov/api-documentation/authorization/\n  - control: revocation\n    description: >-\n      An enrollee can revoke access at any time. The API then returns 404 \"Data Access Grant was not\n      found\". A grant expiry returns 400 invalid_grant with a message directing the enrollee to\n      re-authenticate.\n    source: https://bluebutton.cms.gov/api-documentation/authorization/\nnon_oauth_apis:\n  - api: CMS Beneficiary Claims\
  \ Data API (BCDA)\n    model: bearer token via SSAS client credentials; authority derives from ACO attribution, no scopes\n  - api: CMS AB2D API (Claims Data to Part D Sponsors)\n    model: OAuth 2.0 bearer token via Okta; authority derives from PDP contract, no scopes\n  - api: CMS Data at the Point of Care (DPC) API\n    model: SMART on FHIR Backend Services (JWT client assertion); no user-facing scopes\n  - api: Healthcare.gov Marketplace API\n    model: apikey query parameter; no scopes\n  - api: CMS Procedure Price Lookup (PPL) API\n    model: apiKey + amaLicense headers; no scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/scopes/cms-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Medicare
- Medicaid
- Healthcare
- Health Insurance
- FHIR
- Federal-Government
- Drug Spending
- Provider Data
- Quality Measures
- Claims Data
token_urls:
- https://api.bluebutton.cms.gov/v2/o/token
---
