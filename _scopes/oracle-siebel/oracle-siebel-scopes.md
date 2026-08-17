---
api_specs:
- filename: oracle-siebel-event-pubsub-asyncapi.yml
  format: yaml
  label: Oracle Siebel Event Pub/Sub API
  slug: oracle-siebel-event-pubsub-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/asyncapi/oracle-siebel-event-pubsub-asyncapi.yml
- filename: oracle-siebel-accounts-api-openapi.yml
  format: yaml
  label: Oracle Siebel Accounts API
  slug: oracle-siebel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-accounts-api-openapi.yml
- filename: oracle-siebel-activities-api-openapi.yml
  format: yaml
  label: Oracle Siebel Activities API
  slug: oracle-siebel-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-activities-api-openapi.yml
- filename: oracle-siebel-business-services-api-openapi.yml
  format: yaml
  label: Oracle Siebel Business Services API
  slug: oracle-siebel-business-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-business-services-api-openapi.yml
- filename: oracle-siebel-contacts-api-openapi.yml
  format: yaml
  label: Oracle Siebel Contacts API
  slug: oracle-siebel-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-contacts-api-openapi.yml
- filename: oracle-siebel-metadata-api-openapi.yml
  format: yaml
  label: Oracle Siebel Metadata API
  slug: oracle-siebel-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-metadata-api-openapi.yml
- filename: oracle-siebel-opportunities-api-openapi.yml
  format: yaml
  label: Oracle Siebel Opportunities API
  slug: oracle-siebel-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-opportunities-api-openapi.yml
- filename: oracle-siebel-orders-api-openapi.yml
  format: yaml
  label: Oracle Siebel Orders API
  slug: oracle-siebel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-orders-api-openapi.yml
- filename: oracle-siebel-products-api-openapi.yml
  format: yaml
  label: Oracle Siebel Products API
  slug: oracle-siebel-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-products-api-openapi.yml
- filename: oracle-siebel-repository-api-openapi.yml
  format: yaml
  label: Oracle Siebel Repository API
  slug: oracle-siebel-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-repository-api-openapi.yml
- filename: oracle-siebel-service-requests-api-openapi.yml
  format: yaml
  label: Oracle Siebel Service Requests API
  slug: oracle-siebel-service-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-service-requests-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.oracle.com/cd/G30562_01/books/Secur/c-Using-OAuth-with-REST-Inbound-Web-Services.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Oracle Siebel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Oracle Siebel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Oracle Siebel
provider_slug: oracle-siebel
schemes:
- declared_in:
  - openapi/oracle-siebel-accounts-api-openapi.yml
  - openapi/oracle-siebel-activities-api-openapi.yml
  - openapi/oracle-siebel-business-services-api-openapi.yml
  - openapi/oracle-siebel-contacts-api-openapi.yml
  - openapi/oracle-siebel-metadata-api-openapi.yml
  - openapi/oracle-siebel-opportunities-api-openapi.yml
  - openapi/oracle-siebel-orders-api-openapi.yml
  - openapi/oracle-siebel-products-api-openapi.yml
  - openapi/oracle-siebel-repository-api-openapi.yml
  - openapi/oracle-siebel-service-requests-api-openapi.yml
  declared_scopes: 0
  name: oauth2
  note: 'Every one of the ten specs declares an oauth2 scheme with an EMPTY scopes map. That is consistent with the documentation: there is no Siebel scope vocabulary to declare. The authorizationUrl and tokenUrl carried in those schemes are placeholders — Siebel exposes no such endpoints. See authentication/oracle-siebel-authentication.yml (spec_discrepancy).'
scope_count: 0
scope_names: []
scopes: []
slug: oracle-siebel-scopes
source_filename: oracle-siebel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.oracle.com/cd/G30562_01/books/Secur/c-Using-OAuth-with-REST-Inbound-Web-Services.html\n  and https://docs.oracle.com/cd/F26413_26/books/Secur/index.html, read against\n  the oauth2 securitySchemes declared in openapi/*.yml\ndocs: https://docs.oracle.com/cd/G30562_01/books/Secur/c-Using-OAuth-with-REST-Inbound-Web-Services.html\nprovider: Oracle Siebel\nproviderId: oracle-siebel\nscope_count: 0\nscopes: []\nsummary: >-\n  Oracle publishes NO OAuth scope registry for Siebel, and the absence is\n  structural rather than an omission. Siebel is a resource server that never\n  issues tokens: scope names are minted by whatever external OAuth provider the\n  customer configures (Oracle Access Manager, IDCS/IAM, or a third party). All\n  Oracle states is the matching rule — \"if the token scope is used while\n  retrieving the token, then the token scope must match the executed operation.\"\n  There is consequently\
  \ nothing for this artifact to enumerate, and enumerating\n  plausible scope strings would fabricate a contract that does not exist.\nfinding: no-published-scope-registry\nauthorization_model:\n  primary: siebel-responsibilities-positions-and-view-mode\n  description: >-\n    Real authorization in Siebel is data-level, not scope-level. The\n    authenticated user's responsibilities, position and organization determine\n    which records are visible, refined per request by the ViewMode query\n    parameter. Two callers presenting tokens with identical scopes can legally\n    see completely different data.\n  scope_role: >-\n    Where scopes exist at all, they are a coarse gate in front of Siebel, not a\n    permission model inside it.\nschemes:\n  - name: oauth2\n    declared_in:\n      - openapi/oracle-siebel-accounts-api-openapi.yml\n      - openapi/oracle-siebel-activities-api-openapi.yml\n      - openapi/oracle-siebel-business-services-api-openapi.yml\n      - openapi/oracle-siebel-contacts-api-openapi.yml\n\
  \      - openapi/oracle-siebel-metadata-api-openapi.yml\n      - openapi/oracle-siebel-opportunities-api-openapi.yml\n      - openapi/oracle-siebel-orders-api-openapi.yml\n      - openapi/oracle-siebel-products-api-openapi.yml\n      - openapi/oracle-siebel-repository-api-openapi.yml\n      - openapi/oracle-siebel-service-requests-api-openapi.yml\n    declared_scopes: 0\n    note: >-\n      Every one of the ten specs declares an oauth2 scheme with an EMPTY scopes\n      map. That is consistent with the documentation: there is no Siebel scope\n      vocabulary to declare. The authorizationUrl and tokenUrl carried in those\n      schemes are placeholders — Siebel exposes no such endpoints. See\n      authentication/oracle-siebel-authentication.yml (spec_discrepancy).\nmcp_scope_note: >-\n  The Siebel AI Connectors MCP runtime does have a scope hook —\n  security.jwt.required-scope in application.yaml — but the value is chosen by\n  the deploying customer, so it too is deployment-specific\
  \ rather than published.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/scopes/oracle-siebel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- CRM
- Customer Management
- Enterprise Software
- Marketing Automation
- Oracle
- Sales Automation
- Service Automation
token_urls: []
---
