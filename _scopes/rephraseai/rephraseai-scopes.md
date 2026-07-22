---
authorization_urls: []
description: ''
docs: https://studio-rephrase-api.readme.io/reference/documentation
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rephraseai Scopes
name_suffix: OAuth Scopes
note: Only one OAuth2 scope is documented in the legacy Rephrase Studio API reference. The provider (acquired by Adobe, Nov 2023) publishes no dedicated scopes/permissions reference page.
overview: 'Rephrase.ai publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rephrase.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rephrase.ai
provider_slug: rephraseai
schemes:
- flow: refreshToken
  name: RephraseStudioOAuth2
  tokenUrl: https://auth.rephrase.ai/oauth/token
scope_count: 1
scope_names:
- all:diy
scopes:
- description: Default do-it-yourself (self-serve) access scope granted to Rephrase Studio API tokens; covers actor/voice listing and video create/export/get operations.
  flows:
  - refreshToken
  scope: all:diy
slug: rephraseai-scopes
source_filename: rephraseai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://studio-rephrase-api.readme.io/reference/get-access-token\ndocs: https://studio-rephrase-api.readme.io/reference/documentation\nnote: >-\n  Only one OAuth2 scope is documented in the legacy Rephrase Studio API\n  reference. The provider (acquired by Adobe, Nov 2023) publishes no dedicated\n  scopes/permissions reference page.\nschemes:\n  - name: RephraseStudioOAuth2\n    flow: refreshToken\n    tokenUrl: https://auth.rephrase.ai/oauth/token\nscopes:\n  - scope: all:diy\n    description: >-\n      Default do-it-yourself (self-serve) access scope granted to Rephrase\n      Studio API tokens; covers actor/voice listing and video create/export/get\n      operations.\n    flows: [refreshToken]\n    sources: [https://studio-rephrase-api.readme.io/reference/get-access-token]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rephraseai/refs/heads/main/scopes/rephraseai-scopes.yml
summary_line: 1 scope
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video
- Text to Video
- Avatars
- Media
- Content Creation
token_urls: []
---
