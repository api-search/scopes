---
authorization_urls:
- https://login.salesforce.com/services/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pardot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Salesforce Marketing Cloud Account Engagement (Pardot) publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Salesforce Marketing Cloud Account Engagement (Pardot) API on a user''s behalf.


  Tokens are issued from https://login.salesforce.com/services/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Salesforce Marketing Cloud Account Engagement (Pardot)
provider_slug: pardot
schemes:
- description: 'Authenticate via Salesforce OAuth2 and pass the resulting access

    token as `Authorization: Bearer {token}`. The `Pardot-Business-Unit-Id`

    header is also required on every request.'
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: BearerAuth
  source: openapi/pardot-openapi.yml
scope_count: 1
scope_names:
- pardot_api
scopes:
- description: Access the Pardot/Account Engagement API
  flows:
  - authorizationCode
  scope: pardot_api
slug: pardot-scopes
source_filename: pardot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pardot-openapi.yml\nschemes:\n- name: BearerAuth\n  source: openapi/pardot-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n  description: |-\n    Authenticate via Salesforce OAuth2 and pass the resulting access\n    token as `Authorization: Bearer {token}`. The `Pardot-Business-Unit-Id`\n    header is also required on every request.\nscopes:\n- scope: pardot_api\n  description: Access the Pardot/Account Engagement API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pardot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pardot/refs/heads/main/scopes/pardot-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Marketing Automation
- B2B Marketing
- Lead Generation
- Email Marketing
- Salesforce
- Account Engagement
token_urls:
- https://login.salesforce.com/services/oauth2/token
---
