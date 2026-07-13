---
api_specs:
- filename: listrak-email-openapi.yml
  format: yaml
  label: Listrak Email REST API
  slug: email
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-email-openapi.yml
- filename: listrak-sms-openapi.yml
  format: yaml
  label: Listrak SMS REST API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-sms-openapi.yml
- filename: listrak-crosschannel-openapi.yml
  format: yaml
  label: Listrak Cross Channel REST API
  slug: crosschannel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-crosschannel-openapi.yml
- filename: listrak-data-openapi.yml
  format: yaml
  label: Listrak Data Import REST API
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-data-openapi.yml
- filename: listrak-twowaysms-openapi.yml
  format: yaml
  label: Listrak Two-Way SMS Conversation REST API
  slug: twowaysms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-twowaysms-openapi.yml
- filename: listrak-mobileclient-openapi.yml
  format: yaml
  label: Listrak Mobile App Push API
  slug: mobileclient
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-mobileclient-openapi.yml
- filename: listrak-privacy-openapi.yml
  format: yaml
  label: Listrak Privacy REST API
  slug: privacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/openapi/listrak-privacy-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Listrak Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Listrak publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Listrak API on a user''s behalf.


  Tokens are issued from https://auth.listrak.com/OAuth2/Token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Listrak
provider_slug: listrak
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.listrak.com/OAuth2/Token
  name: OAuth2
  source: openapi/listrak-data-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.listrak.com/OAuth2/Token
  name: OAuth2
  source: openapi/listrak-email-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.listrak.com/OAuth2/Token
  name: OAuth2
  source: openapi/listrak-privacy-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.listrak.com/OAuth2/Token
  name: OAuth2
  source: openapi/listrak-sms-openapi.yml
scope_count: 6
scope_names:
- Contact
- Event
- List
- Message
- Report
- Segmentation
scopes:
- description: Contact access
  flows:
  - clientCredentials
  scope: Contact
- description: Event access
  flows:
  - clientCredentials
  scope: Event
- description: List access
  flows:
  - clientCredentials
  scope: List
- description: Message access
  flows:
  - clientCredentials
  scope: Message
- description: Report access
  flows:
  - clientCredentials
  scope: Report
- description: Segmentation access
  flows:
  - clientCredentials
  scope: Segmentation
slug: listrak-scopes
source_filename: listrak-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/listrak-data-openapi.yml, openapi/listrak-email-openapi.yml, openapi/listrak-privacy-openapi.yml,\n  openapi/listrak-sms-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/listrak-data-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.listrak.com/OAuth2/Token\n- name: OAuth2\n  source: openapi/listrak-email-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.listrak.com/OAuth2/Token\n- name: OAuth2\n  source: openapi/listrak-privacy-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.listrak.com/OAuth2/Token\n- name: OAuth2\n  source: openapi/listrak-sms-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.listrak.com/OAuth2/Token\nscopes:\n- scope: Contact\n  description: Contact access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/listrak-email-openapi.yml\n- scope: Event\n  description: Event\
  \ access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/listrak-email-openapi.yml\n- scope: List\n  description: List access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/listrak-email-openapi.yml\n- scope: Message\n  description: Message access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/listrak-email-openapi.yml\n- scope: Report\n  description: Report access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/listrak-email-openapi.yml\n- scope: Segmentation\n  description: Segmentation access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/listrak-email-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listrak/refs/heads/main/scopes/listrak-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Email Marketing
- SMS Marketing
- Marketing Automation
- Cross-Channel
- Retail
- Push Notifications
- Data Import
- Privacy
token_urls:
- https://auth.listrak.com/OAuth2/Token
---
