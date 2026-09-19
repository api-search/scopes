---
api_specs:
- filename: audatex-audaconnect-api-openapi.yml
  format: yaml
  label: Audatex AudaConnect API
  slug: audatex-audaconnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-audaconnect-api-openapi.yml
- filename: audatex-audaconnect-bms-api-openapi.yml
  format: yaml
  label: Audatex AudaConnect BMS API
  slug: audatex-audaconnect-bms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-audaconnect-bms-api-openapi.yml
- filename: audatex-api-gateway-openapi.yml
  format: yaml
  label: Audatex API Gateway (Intelligent Vehicle Inspection)
  slug: audatex-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-api-gateway-openapi.yml
- filename: audatex-gic-integration-api-openapi.yml
  format: yaml
  label: Audatex GIC API
  slug: audatex-gic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-gic-integration-api-openapi.yml
- filename: audatex-dashboard-assignment-api-openapi.yml
  format: yaml
  label: Solera Dashboard Assignment API
  slug: audatex-dashboard-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/openapi/audatex-dashboard-assignment-api-openapi.yml
authorization_urls:
- https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20
description: ''
docs: https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/help
flows:
- implicit
- password
kind: oauth-scopes
layout: scope
method: searched
name: Audatex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Audatex publishes 27 OAuth 2.0 scopes via the implicit and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Audatex API on a user''s behalf.


  Tokens are issued from https://dispatch-login-demo.audatex.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Audatex
provider_slug: audatex
schemes:
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20
    flow: implicit
  name: oauth2
  source: openapi/audatex-audaconnect-api-openapi.yml
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20
    flow: implicit
  name: oauth2
  source: openapi/audatex-audaconnect-bms-api-openapi.yml
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/audatex-dashboard-assignment-api-openapi.yml
- description: Authorization using the JWT Bearer scheme
  flows:
  - flow: password
    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token
  name: oauth2
  source: openapi/audatex-gic-integration-api-openapi.yml
scope_count: 27
scope_names:
- Assessment.Detail+ImageAccess
- Assessment.EditAssessmentAdminData
- Assessment.ImageAdmin
- Assessment.MailReport
- Assessment.MainIndex
- BMS.Basic
- BMS.Extended
- BMS.Parts
- BMS.PartsOrders
- Internal.DataServices
- Internal.HistoryCheckService
- Manage.Suppliers
- Parts.GetParts
- Parts.UpdateParts
- ReferenceData.Company
- ReferenceData.My
- ReferenceData.System
- ReferenceData.SystemAdmin
- System.Notifications
- System.PushNotifications
- TLA.CreateQuote
- Vehicle.Lookup
- Vehicle.LookupDetailed
- Vehicle.Valuation
- b2b.fnol.api
- readAccess
- writeAccess
scopes:
- description: ''
  flows:
  - implicit
  scope: Assessment.Detail+ImageAccess
- description: ''
  flows:
  - implicit
  scope: Assessment.EditAssessmentAdminData
- description: ''
  flows:
  - implicit
  scope: Assessment.ImageAdmin
- description: Creates a PDF for a mail.
  flows:
  - implicit
  scope: Assessment.MailReport
- description: ''
  flows:
  - implicit
  scope: Assessment.MainIndex
- description: Basic access to assessment data for your BMS application
  flows:
  - implicit
  scope: BMS.Basic
- description: Extened access to assessment data for your BMS application
  flows:
  - implicit
  scope: BMS.Extended
- description: Access to BMS Parts Apis
  flows:
  - implicit
  scope: BMS.Parts
- description: Access to BMS Parts Orders Apis
  flows:
  - implicit
  scope: BMS.PartsOrders
- description: ''
  flows: []
  scope: Internal.DataServices
- description: ''
  flows: []
  scope: Internal.HistoryCheckService
- description: ''
  flows:
  - implicit
  scope: Manage.Suppliers
- description: ''
  flows:
  - implicit
  scope: Parts.GetParts
- description: ''
  flows:
  - implicit
  scope: Parts.UpdateParts
- description: Read access to basic info on your company
  flows:
  - implicit
  scope: ReferenceData.Company
- description: Read access to your basic info e.g. email, user name
  flows:
  - implicit
  scope: ReferenceData.My
- description: ''
  flows:
  - implicit
  scope: ReferenceData.System
- description: ''
  flows:
  - implicit
  scope: ReferenceData.SystemAdmin
- description: Create subscriptions and poll for notifications
  flows:
  - implicit
  scope: System.Notifications
- description: Create subscriptions and receive push notifications
  flows:
  - implicit
  scope: System.PushNotifications
- description: Create Total Loss Avoidance quotes
  flows:
  - implicit
  scope: TLA.CreateQuote
- description: ''
  flows:
  - implicit
  scope: Vehicle.Lookup
- description: ''
  flows:
  - implicit
  scope: Vehicle.LookupDetailed
- description: Perform CAP valuations
  flows:
  - implicit
  scope: Vehicle.Valuation
- description: Audatex Assignment API Access
  flows:
  - password
  scope: b2b.fnol.api
- description: ''
  flows: []
  scope: readAccess
- description: ''
  flows: []
  scope: writeAccess
slug: audatex-scopes
source_filename: audatex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/audatex-audaconnect-api-openapi.yml, openapi/audatex-audaconnect-bms-api-openapi.yml, openapi/audatex-dashboard-assignment-api-openapi.yml,\n  openapi/audatex-gic-integration-api-openapi.yml; scope descriptions and the space-delimited scope parameter confirmed\n  against the AudaConnect developers' guide https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/help; identity-server\n  scopes_supported read from https://dispatch-login-demo.audatex.com/.well-known/openid-configuration (2026-09-17)\nschemes:\n- name: oauth2\n  source: openapi/audatex-audaconnect-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20\n  description: OAuth2 Implicit Grant\n- name: oauth2\n  source: openapi/audatex-audaconnect-bms-api-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://audaconnect.ax-aee.co.uk/AudaAPI.Portal/Oauth20\n  description: OAuth2\
  \ Implicit Grant\n- name: oauth2\n  source: openapi/audatex-dashboard-assignment-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\n- name: oauth2\n  source: openapi/audatex-gic-integration-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: https://dispatch-login-demo.audatex.com/connect/token\n  description: Authorization using the JWT Bearer scheme\nscopes:\n- scope: Assessment.Detail+ImageAccess\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Assessment.EditAssessmentAdminData\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Assessment.ImageAdmin\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Assessment.MailReport\n  description: Creates a PDF for a mail.\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n\
  - scope: Assessment.MainIndex\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: BMS.Basic\n  description: Basic access to assessment data for your BMS application\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-bms-api-openapi.yml\n- scope: BMS.Extended\n  description: Extened access to assessment data for your BMS application\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-bms-api-openapi.yml\n- scope: BMS.Parts\n  description: Access to BMS Parts Apis\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-bms-api-openapi.yml\n- scope: BMS.PartsOrders\n  description: Access to BMS Parts Orders Apis\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-bms-api-openapi.yml\n- scope: Internal.DataServices\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Internal.HistoryCheckService\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope:\
  \ Manage.Suppliers\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Parts.GetParts\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Parts.UpdateParts\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: ReferenceData.Company\n  description: Read access to basic info on your company\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: ReferenceData.My\n  description: Read access to your basic info e.g. email, user name\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: ReferenceData.System\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: ReferenceData.SystemAdmin\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: System.Notifications\n  description: Create subscriptions and poll for\
  \ notifications\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: System.PushNotifications\n  description: Create subscriptions and receive push notifications\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: TLA.CreateQuote\n  description: Create Total Loss Avoidance quotes\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Vehicle.Lookup\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Vehicle.LookupDetailed\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: Vehicle.Valuation\n  description: Perform CAP valuations\n  flows:\n  - implicit\n  sources:\n  - openapi/audatex-audaconnect-api-openapi.yml\n- scope: b2b.fnol.api\n  description: Audatex Assignment API Access\n  flows:\n  - password\n  sources:\n  - openapi/audatex-dashboard-assignment-api-openapi.yml\n  - openapi/audatex-gic-integration-api-openapi.yml\n\
  - scope: readAccess\n  sources:\n  - openapi/audatex-dashboard-assignment-api-openapi.yml\n  - openapi/audatex-gic-integration-api-openapi.yml\n- scope: writeAccess\n  sources:\n  - openapi/audatex-dashboard-assignment-api-openapi.yml\n  - openapi/audatex-gic-integration-api-openapi.yml\ndocs: https://audaconnect.ax-aee.co.uk/AudaAPI.BMSAPI/home/help\nnotes: AudaConnect scopes are requested space-delimited and URL-encoded (scope=BMS.Basic BMS.Extended) and are granted\n  per registered client application after Audatex approval. readAccess / writeAccess appear only in the GIC and\n  Dashboard Assignment global security requirement and are NOT declared in either spec's securitySchemes nor in\n  the identity server's scopes_supported — a spec defect, recorded as-is. The dispatch-login OpenID Connect discovery\n  document advertises 34 scopes_supported (openid, profile, email, offline_access, b2b.fnol.api, b2b.admin.api,\n  b2b.fnol.documents, b2b.lien.api, mobile.inspection.api, estimatics.api,\
  \ hqclaims.api, vinhistory.api, gofnol.api,\n  ...); only b2b.fnol.api is bound to a published OpenAPI, so the others are listed for reference below and not\n  counted as API scopes.\nidentity_server_scopes_supported:\n- user.organization\n- cosec\n- email\n- profile\n- user.entity\n- openid\n- user.profile\n- user.office\n- address\n- marketdata.web.api\n- eagle.api\n- omadi\n- api1\n- b2b.admin.api\n- novo.claims.manager\n- mobile.inspection.api\n- review.api\n- novo.estimating\n- b2b.fnol.api\n- fnol.test\n- b2b.fnol.transformer\n- a2e.admin.api\n- gofnol.api\n- vinhistory.api\n- gotime\n- SMAppServices\n- b2b.fnol.documents\n- estimatics.api\n- hqclaims.api\n- hqorg.AL\n- hqorg.SF\n- b2b.lien.api\n- b2b.lien.report\n- offline_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audatex/refs/heads/main/scopes/audatex-scopes.yml
summary_line: 27 scopes · implicit/password
tags:
- Automotive
- Claims Processing
- Insurance
- Repair Management
- Vehicle Data
- Collision Repair
- Vehicle Inspection
token_urls:
- https://dispatch-login-demo.audatex.com/connect/token
---
