---
authorization_urls: []
description: The complete set of OAuth 2.0 / OpenID Connect scopes advertised by the only authorization server OncoC4 serves publicly — the Umbraco CMS Delivery API member authorization server on oncoc4.com. Taken verbatim from `scopes_supported` in the discovery document. There is no developer API and no developer-facing permission model.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Oncoc4 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OncoC4 uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OncoC4
provider_slug: oncoc4
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: oncoc4-scopes
source_filename: oncoc4-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://oncoc4.com/.well-known/openid-configuration\nname: OncoC4 OAuth scopes\ndescription: >-\n  The complete set of OAuth 2.0 / OpenID Connect scopes advertised by the only\n  authorization server OncoC4 serves publicly — the Umbraco CMS Delivery API\n  member authorization server on oncoc4.com. Taken verbatim from\n  `scopes_supported` in the discovery document. There is no developer API and no\n  developer-facing permission model.\nissuer: https://oncoc4.com/\nauthorization_server: umbraco_delivery_member_oidc\ndocs: null\nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope requesting an ID token for the authenticated\n    Umbraco CMS member.\n  standard: true\n  source: openid-configuration scopes_supported\n- name: offline_access\n  description: >-\n    Standard OpenID Connect scope requesting a refresh token so the client can\n    renew the member session without re-authentication.\n  standard:\
  \ true\n  source: openid-configuration scopes_supported\ncounts:\n  total: 2\n  standard: 2\n  provider_specific: 0\nnotes:\n- No provider-specific or resource scopes are published. Both scopes are generic\n  OIDC scopes emitted by Umbraco's default configuration.\n- No scopes/permissions reference page exists on the OncoC4 site; a docs search\n  across oncoc4.com found no developer documentation of any kind.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://oncoc4.com/.well-known/openid-configuration\n  http_status: 200\n  file: well-known/oncoc4-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oncoc4/refs/heads/main/scopes/oncoc4-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Biotechnology
- Biopharmaceutical
- Life Sciences
- Oncology
- Immunotherapy
- Clinical Trials
- Healthcare
- Pharmaceuticals
token_urls: []
---
