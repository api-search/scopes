---
api_specs:
- filename: certifid-accountverifications-api-openapi.yml
  format: yaml
  label: CertifID Account Verifications API
  slug: certifid-accountverifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-accountverifications-api-openapi.yml
- filename: certifid-banklookup-api-openapi.yml
  format: yaml
  label: CertifID Bank Lookup API
  slug: certifid-banklookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-banklookup-api-openapi.yml
- filename: certifid-collectrequest-api-openapi.yml
  format: yaml
  label: CertifID Collect Request API
  slug: certifid-collectrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-collectrequest-api-openapi.yml
- filename: certifid-confirmrequest-api-openapi.yml
  format: yaml
  label: CertifID Confirm Request API
  slug: certifid-confirmrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-confirmrequest-api-openapi.yml
- filename: certifid-disbursements-api-openapi.yml
  format: yaml
  label: CertifID Disbursements API
  slug: certifid-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-disbursements-api-openapi.yml
- filename: certifid-identityrequest-api-openapi.yml
  format: yaml
  label: CertifID Identity Request API
  slug: certifid-identityrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-identityrequest-api-openapi.yml
- filename: certifid-integration-api-openapi.yml
  format: yaml
  label: CertifID Integration API
  slug: certifid-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-integration-api-openapi.yml
- filename: certifid-lenders-api-openapi.yml
  format: yaml
  label: CertifID Lenders API
  slug: certifid-lenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-lenders-api-openapi.yml
- filename: certifid-location-api-openapi.yml
  format: yaml
  label: CertifID Location API
  slug: certifid-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-location-api-openapi.yml
- filename: certifid-payoffordering-api-openapi.yml
  format: yaml
  label: CertifID Payoff Ordering API
  slug: certifid-payoffordering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-payoffordering-api-openapi.yml
- filename: certifid-sendrequest-api-openapi.yml
  format: yaml
  label: CertifID Send Request API
  slug: certifid-sendrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-sendrequest-api-openapi.yml
- filename: certifid-test-api-openapi.yml
  format: yaml
  label: CertifID Test API
  slug: certifid-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-test-api-openapi.yml
- filename: certifid-underwriter-api-openapi.yml
  format: yaml
  label: CertifID Underwriter API
  slug: certifid-underwriter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-underwriter-api-openapi.yml
- filename: certifid-users-api-openapi.yml
  format: yaml
  label: CertifID Users API
  slug: certifid-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-users-api-openapi.yml
- filename: certifid-wiringinstructions-api-openapi.yml
  format: yaml
  label: CertifID Wiring Instructions API
  slug: certifid-wiringinstructions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/openapi/certifid-wiringinstructions-api-openapi.yml
authorization_urls:
- https://auth.certifid.com/authorize?audience=https://api.certifid.com&connection=CertifID-Users-DB
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Certifid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CertifID publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CertifID API on a user''s behalf.


  Tokens are issued from https://auth.certifid.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CertifID
provider_slug: certifid
schemes:
- flows:
  - authorizationUrl: https://auth.certifid.com/authorize?audience=https://api.certifid.com&connection=CertifID-Users-DB
    flow: authorizationCode
    tokenUrl: https://auth.certifid.com/oauth/token
  name: oauth2
  source: openapi/certifid-v2-apis-openapi.json
scope_count: 12
scope_names:
- CertifIDUser
- PayoffProtectProduct
- RequestCreator
- RequestProduct
- ResourceAccessToken|read:disbursements|id|DisbursementVerification
- ResourceAccessToken|read:payofforder|payoffOrderId|PayoffOrder
- ResourceAccessToken|read:requests|disbursementId|DisbursementVerification
- ResourceAccessToken|read:requests|requestId|CollectRequest
- ResourceAccessToken|read:requests|requestId|ConfirmRequest
- ResourceAccessToken|read:requests|requestId|IdentityRequest
- ResourceAccessToken|read:requests|requestId|SendRequest
- ResourceAccessToken|read:requests|resourceId|CompanyWiringInfo
scopes:
- description: ''
  flows: []
  scope: CertifIDUser
- description: ''
  flows: []
  scope: PayoffProtectProduct
- description: ''
  flows: []
  scope: RequestCreator
- description: ''
  flows: []
  scope: RequestProduct
- description: ''
  flows: []
  scope: ResourceAccessToken|read:disbursements|id|DisbursementVerification
- description: ''
  flows: []
  scope: ResourceAccessToken|read:payofforder|payoffOrderId|PayoffOrder
- description: ''
  flows: []
  scope: ResourceAccessToken|read:requests|disbursementId|DisbursementVerification
- description: ''
  flows: []
  scope: ResourceAccessToken|read:requests|requestId|CollectRequest
- description: ''
  flows: []
  scope: ResourceAccessToken|read:requests|requestId|ConfirmRequest
- description: ''
  flows: []
  scope: ResourceAccessToken|read:requests|requestId|IdentityRequest
- description: ''
  flows: []
  scope: ResourceAccessToken|read:requests|requestId|SendRequest
- description: ''
  flows: []
  scope: ResourceAccessToken|read:requests|resourceId|CompanyWiringInfo
slug: certifid-scopes
source_filename: certifid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/certifid-v2-apis-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/certifid-v2-apis-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.certifid.com/authorize?audience=https://api.certifid.com&connection=CertifID-Users-DB\n    tokenUrl: https://auth.certifid.com/oauth/token\nscopes:\n- scope: CertifIDUser\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: PayoffProtectProduct\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: RequestCreator\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: RequestProduct\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:disbursements|id|DisbursementVerification\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:payofforder|payoffOrderId|PayoffOrder\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:requests|disbursementId|DisbursementVerification\n\
  \  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:requests|requestId|CollectRequest\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:requests|requestId|ConfirmRequest\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:requests|requestId|IdentityRequest\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:requests|requestId|SendRequest\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n- scope: ResourceAccessToken|read:requests|resourceId|CompanyWiringInfo\n  sources:\n  - openapi/certifid-v2-apis-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certifid/refs/heads/main/scopes/certifid-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Company
- Wire Fraud Prevention
- Real Estate
- Title Insurance
- Identity Verification
- Business Verification
- Payments
- Fraud Prevention
- Escrow and Settlement
- Financial Services
- Security
token_urls:
- https://auth.certifid.com/oauth/token
---
