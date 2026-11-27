---
authorization_urls: []
description: ''
docs: https://cocuyo.ai/llms.txt
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cocuyo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cocuyo publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cocuyo API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cocuyo
provider_slug: cocuyo-ai
schemes: []
scope_count: 2
scope_names:
- cocuyo:leer
- cocuyo:crear
scopes:
- description: Read-only. Balance and daily-limit checks, model discovery, quotes (quoting does not generate or charge) and listing the connection's creations. Tools cocuyo_saldo, cocuyo_modelos, cocuyo_cotizar, cocuyo_creaciones.
  flows: []
  scope: cocuyo:leer
- description: Creation permission. Generating with confirmed credits (cocuyo_generar) and checking/continuing an existing confirmed job (cocuyo_estado, treated as a write). Respects the per-connection daily credit limit.
  flows: []
  scope: cocuyo:crear
slug: cocuyo-ai-scopes
source_filename: cocuyo-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cocuyo.ai/.well-known/oauth-authorization-server\ndocs: https://cocuyo.ai/llms.txt\nscopes:\n- name: cocuyo:leer\n  description: Read-only. Balance and daily-limit checks, model discovery, quotes (quoting does not generate or charge) and listing the connection's creations. Tools cocuyo_saldo, cocuyo_modelos, cocuyo_cotizar, cocuyo_creaciones.\n- name: cocuyo:crear\n  description: Creation permission. Generating with confirmed credits (cocuyo_generar) and checking/continuing an existing confirmed job (cocuyo_estado, treated as a write). Respects the per-connection daily credit limit.\n"
source_yaml_url: https://artifacts.apis.io/cocuyo-ai/scopes/cocuyo-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Text-to-Speech
- MCP
- Creative Tools
token_bound: false
token_urls: []
---
