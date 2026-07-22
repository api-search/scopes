---
authorization_urls: []
description: ''
docs: https://developers.shakr.com/docs/api/authentication/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Shakr Media Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shakr Media publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shakr Media API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shakr Media
provider_slug: shakr-media
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  source: docs
  tokenHost: https://api.shakr.com
scope_count: 6
scope_names:
- template_style_version:read
- template_style_version:write
- mapping:read
- mapping:write
- render_session:read
- render_session:write
scopes:
- description: Read access to TemplateStyleVersion resources.
  flows: []
  scope: template_style_version:read
- description: Write access to TemplateStyleVersion resources.
  flows: []
  scope: template_style_version:write
- description: Read access to Mapping resources.
  flows: []
  scope: mapping:read
- description: Write access to Mapping resources.
  flows: []
  scope: mapping:write
- description: Read access to RenderSession resources.
  flows: []
  scope: render_session:read
- description: Write access to RenderSession resources.
  flows: []
  scope: render_session:write
slug: shakr-media-scopes
source_filename: shakr-media-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.shakr.com/api/retrieve-an-access-token/\ndocs: https://developers.shakr.com/docs/api/authentication/\nschemes:\n  - name: OAuth2ClientCredentials\n    flow: clientCredentials\n    tokenHost: https://api.shakr.com\n    source: docs\nconvention:\n  format: \"resource[:action][:target]\"\n  description: >-\n    The optional `scope` parameter on the token request restricts the actions a\n    token can perform. Scope strings are comma-separated and follow the\n    resource[:action][:target] convention. `action` is read or write; `target`\n    optionally narrows the scope to a single resource id (e.g.\n    template_style_version:write:Zx1A grants write on one TemplateStyleVersion).\n  example: \"template_style_version:write:Zx1A\"\nresources: [template_style_version, mapping, render_session]\nactions: [read, write]\nscopes:\n  - scope: \"template_style_version:read\"\n    description: Read access to TemplateStyleVersion\
  \ resources.\n  - scope: \"template_style_version:write\"\n    description: Write access to TemplateStyleVersion resources.\n  - scope: \"mapping:read\"\n    description: Read access to Mapping resources.\n  - scope: \"mapping:write\"\n    description: Write access to Mapping resources.\n  - scope: \"render_session:read\"\n    description: Read access to RenderSession resources.\n  - scope: \"render_session:write\"\n    description: Write access to RenderSession resources.\nnotes: >-\n  Scopes above are documented convention examples derived from the published\n  resource[:action][:target] grammar and the three API resources (Mapping,\n  RenderSession, TemplateStyleVersion). Shakr does not publish a fixed\n  enumerated scope list; tokens may also be minted un-scoped for full access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shakr-media/refs/heads/main/scopes/shakr-media-scopes.yml
summary_line: 6 scopes
tags:
- Company
- Video
- Video Creation
- Video Editing
- Video API
- Media
- SDK
- Automation
- Advertising
- White Label
token_urls: []
---
