---
authorization_urls:
- https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- ciba
kind: oauth-scopes
layout: scope
method: searched
name: Traive Scopes
name_suffix: OAuth Scopes
note: 'Traive publishes no public developer API or scopes reference. These scopes are harvested verbatim from the scopes_supported claim of the public Keycloak OpenID Connect discovery document for realm traive-prod. No scope descriptions are published; "standard: true" marks OIDC/Keycloak built-in scopes, the remainder name Traive''s internal service estate.'
overview: 'Traive publishes 50 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and ciba flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Traive API on a user''s behalf.


  Tokens are issued from https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Traive
provider_slug: traive
schemes:
- flows:
  - authorizationUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth/device
    flow: deviceCode
  - flow: ciba
    grant: urn:openid:params:grant-type:ciba
  issuer: https://auth.traive-prod.com/realms/traive-prod
  name: traive-prod (Keycloak realm)
  source: well-known/traive-openid-configuration.json
  type: openIdConnect
scope_count: 50
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- roles
- web-origins
- acr
- basic
- service_account
- organization
- microprofile-jwt
- one-traive-api
- platform-graphql
- erp-integration-api
- dis-integration-api
- dis-integrator-service
- inbound-dis-integrator-service
- outbound-dis-integrator-service
- credit-core-service
- credit-assessment-service
- credit-snapshot-service
- credit-atheneum-backend-service
- farmers-core-service
- retailers-core-service
- user-core-service
- entity-core-service
- document-core-service
- document-processor-service
- financial-information-api-service
- attributes-api-service
- settings-api-service
- return-data-credit-limit-erp
- return-data-documents-erp
- return-data-client-erp
- atheneum-document-status
- atheneum-supervisor
- permission-groups-kafka-connector
- keycloak-policy-enforcer
- keycloak-extensions-api
- enchila-schema-registry
- enchila-schema-registry-ui
- marketplace
- fiagro-app
- mp-user
- appsmith
- geoserver
- databricks
- streamlit-internal
scopes:
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: email
- description: ''
  flows: []
  scope: address
- description: ''
  flows: []
  scope: phone
- description: ''
  flows: []
  scope: offline_access
- description: ''
  flows: []
  scope: roles
- description: ''
  flows: []
  scope: web-origins
- description: ''
  flows: []
  scope: acr
- description: ''
  flows: []
  scope: basic
- description: ''
  flows: []
  scope: service_account
- description: ''
  flows: []
  scope: organization
- description: ''
  flows: []
  scope: microprofile-jwt
- description: ''
  flows: []
  scope: one-traive-api
- description: ''
  flows: []
  scope: platform-graphql
- description: ''
  flows: []
  scope: erp-integration-api
- description: ''
  flows: []
  scope: dis-integration-api
- description: ''
  flows: []
  scope: dis-integrator-service
- description: ''
  flows: []
  scope: inbound-dis-integrator-service
- description: ''
  flows: []
  scope: outbound-dis-integrator-service
- description: ''
  flows: []
  scope: credit-core-service
- description: ''
  flows: []
  scope: credit-assessment-service
- description: ''
  flows: []
  scope: credit-snapshot-service
- description: ''
  flows: []
  scope: credit-atheneum-backend-service
- description: ''
  flows: []
  scope: farmers-core-service
- description: ''
  flows: []
  scope: retailers-core-service
- description: ''
  flows: []
  scope: user-core-service
- description: ''
  flows: []
  scope: entity-core-service
- description: ''
  flows: []
  scope: document-core-service
- description: ''
  flows: []
  scope: document-processor-service
- description: ''
  flows: []
  scope: financial-information-api-service
- description: ''
  flows: []
  scope: attributes-api-service
- description: ''
  flows: []
  scope: settings-api-service
- description: ''
  flows: []
  scope: return-data-credit-limit-erp
- description: ''
  flows: []
  scope: return-data-documents-erp
- description: ''
  flows: []
  scope: return-data-client-erp
- description: ''
  flows: []
  scope: atheneum-document-status
- description: ''
  flows: []
  scope: atheneum-supervisor
- description: ''
  flows: []
  scope: permission-groups-kafka-connector
- description: ''
  flows: []
  scope: keycloak-policy-enforcer
- description: ''
  flows: []
  scope: keycloak-extensions-api
- description: ''
  flows: []
  scope: enchila-schema-registry
- description: ''
  flows: []
  scope: enchila-schema-registry-ui
- description: ''
  flows: []
  scope: marketplace
- description: ''
  flows: []
  scope: fiagro-app
- description: ''
  flows: []
  scope: mp-user
- description: ''
  flows: []
  scope: appsmith
- description: ''
  flows: []
  scope: geoserver
- description: ''
  flows: []
  scope: databricks
- description: ''
  flows: []
  scope: streamlit-internal
slug: traive-scopes
source_filename: traive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://auth.traive-prod.com/realms/traive-prod/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Traive publishes no public developer API or scopes reference. These scopes are\n  harvested verbatim from the scopes_supported claim of the public Keycloak OpenID\n  Connect discovery document for realm traive-prod. No scope descriptions are\n  published; \"standard: true\" marks OIDC/Keycloak built-in scopes, the remainder\n  name Traive's internal service estate.\nschemes:\n- name: traive-prod (Keycloak realm)\n  type: openIdConnect\n  issuer: https://auth.traive-prod.com/realms/traive-prod\n  source: well-known/traive-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth\n    tokenUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/auth/device\n  - flow: ciba\n    grant: urn:openid:params:grant-type:ciba\nscopes:\n- scope: openid\n  standard: true\n- scope: profile\n  standard: true\n- scope: email\n  standard: true\n- scope: address\n  standard: true\n- scope: phone\n  standard: true\n- scope: offline_access\n  standard: true\n- scope: roles\n  standard: true\n- scope: web-origins\n  standard: true\n- scope: acr\n  standard: true\n- scope: basic\n  standard: true\n- scope: service_account\n  standard: true\n- scope: organization\n  standard: true\n- scope: microprofile-jwt\n  standard: true\n- scope: one-traive-api\n- scope: platform-graphql\n- scope: erp-integration-api\n- scope: dis-integration-api\n- scope: dis-integrator-service\n- scope: inbound-dis-integrator-service\n- scope: outbound-dis-integrator-service\n- scope: credit-core-service\n- scope: credit-assessment-service\n- scope: credit-snapshot-service\n\
  - scope: credit-atheneum-backend-service\n- scope: farmers-core-service\n- scope: retailers-core-service\n- scope: user-core-service\n- scope: entity-core-service\n- scope: document-core-service\n- scope: document-processor-service\n- scope: financial-information-api-service\n- scope: attributes-api-service\n- scope: settings-api-service\n- scope: return-data-credit-limit-erp\n- scope: return-data-documents-erp\n- scope: return-data-client-erp\n- scope: atheneum-document-status\n- scope: atheneum-supervisor\n- scope: permission-groups-kafka-connector\n- scope: keycloak-policy-enforcer\n- scope: keycloak-extensions-api\n- scope: enchila-schema-registry\n- scope: enchila-schema-registry-ui\n- scope: marketplace\n- scope: fiagro-app\n- scope: mp-user\n- scope: appsmith\n- scope: geoserver\n- scope: databricks\n- scope: streamlit-internal\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traive/refs/heads/main/scopes/traive-scopes.yml
summary_line: 50 scopes · authorizationCode/clientCredentials/deviceCode/ciba
tags:
- Company
- Agriculture
- Fintech
- Credit
- Risk Analysis
- Lending
- AgTech
- Brazil
token_urls:
- https://auth.traive-prod.com/realms/traive-prod/protocol/openid-connect/token
---
