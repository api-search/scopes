---
authorization_urls: []
description: ''
docs: https://docs.raidxai.com/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Raid Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Raid AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Raid AI
provider_slug: raid-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: raid-ai-scopes
source_filename: raid-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.raidxai.com/docs/authentication\ndocs: https://docs.raidxai.com/docs/authentication\nnotes: >-\n  Two distinct scope surfaces. (1) API-key scopes gate which detection\n  endpoints a dashboard-issued bearer token may call; documented on the\n  Authentication page. (2) OAuth2/OIDC scopes advertised by the OpenIddict\n  authorization server (from the openid-configuration discovery document) —\n  platform/dashboard and bot identity, not the detection API-key surface.\napi_key_scopes:\n  - scope: image\n    endpoints: /api/app/image-forensics/*\n    description: Analyze images for AI generation, deepfakes, and tampering.\n  - scope: audio\n    endpoints: /api/app/voice-analysis/*\n    description: Analyze audio for AI-generated / cloned voices, with optional transcription.\n  - scope: fact-check\n    endpoints: /api/app/fact-checking/*\n    description: Submit and poll asynchronous fact-checking jobs.\n  - scope: document\n\
  \    endpoints: /api/app/document (documentForensicsAnalyze)\n    description: Analyze a PDF document for tampering, consistency, and anomalies.\n  - scope: document-image\n    endpoints: documentDeepfakeDetect\n    description: Detect tampering / AI editing in a single document-page image.\noauth2_scopes:\n  source: https://api.raidxai.com/.well-known/openid-configuration\n  scopes:\n    - scope: openid\n      description: OpenID Connect authentication.\n    - scope: email\n      description: Access the user's email claim.\n    - scope: profile\n      description: Access the user's profile claims.\n    - scope: roles\n      description: Access the user's role claims.\n    - scope: offline_access\n      description: Issue refresh tokens for long-lived access.\n    - scope: Raid\n      description: Access to the Raid platform resource server.\n    - scope: xbot.admin\n      description: Administrative access to the X (Twitter) bot integration.\n    - scope: whatsappbot.admin\n      description:\
  \ Administrative access to the WhatsApp bot integration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raid-ai/refs/heads/main/scopes/raid-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Deepfake Detection
- AI Content Detection
- Media Forensics
- Voice / Audio Detection
- Image Forensics
- Document Forensics
- Fact-Checking
- Trust & Safety
- Security
token_urls: []
---
