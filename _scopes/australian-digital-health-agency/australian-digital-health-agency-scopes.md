---
authorization_urls:
- https://api.healthterminologies.gov.au/oauth2/login
description: ''
docs: https://api.healthterminologies.gov.au/integration/R4/fhir/.well-known/smart-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Australian Digital Health Agency Scopes
name_suffix: OAuth Scopes
note: The NCTS FHIR terminology server authenticates with SMART-on-FHIR OAuth2. Its SMART discovery document advertises OpenID Connect scopes only (openid, profile); as a read-oriented terminology service it does not expose SMART clinical resource scopes. The national record systems (My Health Record, HI Service, e-prescribing) use NASH PKI mutual TLS rather than OAuth scopes.
overview: 'Australian Digital Health Agency publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Australian Digital Health Agency API on a user''s behalf.


  Tokens are issued from https://api.healthterminologies.gov.au/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australian Digital Health Agency
provider_slug: australian-digital-health-agency
schemes:
- flows:
  - authorizationUrl: https://api.healthterminologies.gov.au/oauth2/login
    flow: authorizationCode
    tokenUrl: https://api.healthterminologies.gov.au/oauth2/token
  name: SMART-on-FHIR-OAuth2
  source: well-known/australian-digital-health-agency-smart-configuration.json
scope_count: 2
scope_names:
- openid
- profile
scopes:
- description: OpenID Connect authentication for the terminology server.
  flows:
  - authorizationCode
  scope: openid
- description: Access to basic OpenID Connect profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: australian-digital-health-agency-scopes
source_filename: australian-digital-health-agency-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: well-known/australian-digital-health-agency-smart-configuration.json\ndocs: https://api.healthterminologies.gov.au/integration/R4/fhir/.well-known/smart-configuration\nnote: >-\n  The NCTS FHIR terminology server authenticates with SMART-on-FHIR OAuth2. Its\n  SMART discovery document advertises OpenID Connect scopes only (openid, profile);\n  as a read-oriented terminology service it does not expose SMART clinical resource\n  scopes. The national record systems (My Health Record, HI Service, e-prescribing)\n  use NASH PKI mutual TLS rather than OAuth scopes.\nschemes:\n  - name: SMART-on-FHIR-OAuth2\n    source: well-known/australian-digital-health-agency-smart-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.healthterminologies.gov.au/oauth2/login\n        tokenUrl: https://api.healthterminologies.gov.au/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID\
  \ Connect authentication for the terminology server.\n    flows: [authorizationCode]\n    sources: [well-known/australian-digital-health-agency-smart-configuration.json]\n  - scope: profile\n    description: Access to basic OpenID Connect profile claims.\n    flows: [authorizationCode]\n    sources: [well-known/australian-digital-health-agency-smart-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-digital-health-agency/refs/heads/main/scopes/australian-digital-health-agency-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Healthcare
- Australia
- National Health System
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Electronic Health Record
- e-Prescribing
- Terminology
- Government
token_urls:
- https://api.healthterminologies.gov.au/oauth2/token
---
