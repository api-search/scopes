---
authorization_urls: []
description: ''
docs: https://docs-vcc.atlassian.net/wiki/spaces/VCCA
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Newvoicemedia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NewVoiceMedia publishes 10 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the NewVoiceMedia API on a user''s behalf.


  Tokens are issued from https://{region}.cc.vonage.com/Auth/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NewVoiceMedia
provider_slug: newvoicemedia
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{region}.cc.vonage.com/Auth/connect/token
  name: OAuth2ClientCredentials
scope_count: 10
scope_names:
- agents-availability:read
- users:read
- users:write
- interactions:write
- interaction-content:read
- interaction-content:delete
- stats
- globalpci
- admin:read
- admin:write
scopes:
- description: Read access to the Agent Availability API (query agents by skills and presence).
  flows:
  - clientCredentials
  scope: agents-availability:read
- description: Read VCC user details, settings, and presences (User Admin / Agents API).
  flows:
  - clientCredentials
  scope: users:read
- description: Update VCC user details, settings, and presences.
  flows:
  - clientCredentials
  scope: users:write
- description: Create and update active interactions (Interactions / Interaction Control API).
  flows:
  - clientCredentials
  scope: interactions:write
- description: Read and download interaction content (recordings, transcripts) and schedule exports.
  flows:
  - clientCredentials
  scope: interaction-content:read
- description: Delete interaction content such as recordings and transcripts.
  flows:
  - clientCredentials
  scope: interaction-content:delete
- description: Access the Insights Stats API for VCC activity metrics.
  flows:
  - clientCredentials
  scope: stats
- description: Access the Payment API for PCI-compliant secure payment sessions.
  flows:
  - clientCredentials
  scope: globalpci
- description: Read VCC administration settings.
  flows:
  - clientCredentials
  scope: admin:read
- description: Update VCC administration settings.
  flows:
  - clientCredentials
  scope: admin:write
slug: newvoicemedia-scopes
source_filename: newvoicemedia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs-vcc.atlassian.net/wiki/spaces/VCCA/pages/3567190030/How+to+authenticate+with+a+Vonage+Contact+Center+(VCC)+API\ndocs: https://docs-vcc.atlassian.net/wiki/spaces/VCCA\nnotes: >-\n  VCC OAuth 2.0 scopes follow an object:action convention and are requested at\n  token time via the client-credentials flow. This list is captured verbatim\n  from the VCC authentication documentation; individual API reference pages may\n  document additional per-endpoint scopes.\nschemes:\n  - name: OAuth2ClientCredentials\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://{region}.cc.vonage.com/Auth/connect/token\nscopes:\n  - scope: agents-availability:read\n    description: Read access to the Agent Availability API (query agents by skills and presence).\n    flows: [clientCredentials]\n  - scope: users:read\n    description: Read VCC user details, settings, and presences (User Admin / Agents API).\n    flows: [clientCredentials]\n\
  \  - scope: users:write\n    description: Update VCC user details, settings, and presences.\n    flows: [clientCredentials]\n  - scope: interactions:write\n    description: Create and update active interactions (Interactions / Interaction Control API).\n    flows: [clientCredentials]\n  - scope: interaction-content:read\n    description: Read and download interaction content (recordings, transcripts) and schedule exports.\n    flows: [clientCredentials]\n  - scope: interaction-content:delete\n    description: Delete interaction content such as recordings and transcripts.\n    flows: [clientCredentials]\n  - scope: stats\n    description: Access the Insights Stats API for VCC activity metrics.\n    flows: [clientCredentials]\n  - scope: globalpci\n    description: Access the Payment API for PCI-compliant secure payment sessions.\n    flows: [clientCredentials]\n  - scope: admin:read\n    description: Read VCC administration settings.\n    flows: [clientCredentials]\n  - scope: admin:write\n\
  \    description: Update VCC administration settings.\n    flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newvoicemedia/refs/heads/main/scopes/newvoicemedia-scopes.yml
summary_line: 10 scopes · clientCredentials
tags:
- Company
- Cloud
- Contact Center
- CCaaS
- Communications
- Customer Experience
- Telephony
- Analytics
token_urls:
- https://{region}.cc.vonage.com/Auth/connect/token
---
