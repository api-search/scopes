---
api_specs:
- filename: kyoto-oai-pmh-api-openapi.yml
  format: yaml
  label: KURENAI OAI-PMH API
  slug: kyoto-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-oai-pmh-api-openapi.yml
- filename: kyoto-rest-api-openapi.yml
  format: yaml
  label: KURENAI DSpace REST API
  slug: kyoto-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-rest-api-openapi.yml
- filename: kyoto-lms-api-openapi.yml
  format: yaml
  label: PandA Learning Support System API (Sakai Entity Broker + IMS LTI)
  slug: kyoto-lms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/openapi/kyoto-lms-api-openapi.yml
authorization_urls: []
description: Kyoto University publishes no OAuth 2.0 authorization server, no consent screen, no scope vocabulary and no developer registration for any surface it operates. This file records that absence explicitly rather than leaving the artifact missing, and records the two authorization vocabularies that do exist on its surfaces so neither is mistaken for a published scope model.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kyoto Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kyoto University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kyoto University
provider_slug: kyoto
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kyoto-scopes
source_filename: kyoto-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of every Kyoto University-operated surface in this profile, plus a read\n  of openapi/kyoto-lms-api-openapi.yml, openapi/kyoto-rest-api-openapi.yml and\n  openapi/kyoto-oai-pmh-api-openapi.yml.\nprovider: Kyoto University\nproviderId: kyoto\nstate: none_published\ndescription: >-\n  Kyoto University publishes no OAuth 2.0 authorization server, no consent screen, no scope\n  vocabulary and no developer registration for any surface it operates. This file records that\n  absence explicitly rather than leaving the artifact missing, and records the two authorization\n  vocabularies that do exist on its surfaces so neither is mistaken for a published scope model.\noauth2:\n  authorization_server: none_found\n  token_endpoint: none_found\n  scopes: []\n  detail: >-\n    No .well-known/oauth-authorization-server or .well-known/openid-configuration was found on any\n    Kyoto University-operated host. The\
  \ PandA LTI 1.3 handler exposes a token path\n    (/imsblis/lti13/token) but it answers 400 to a GET\n    ({\"error\":\"Unrecognized GET request parts=4 ...\"}), and LTI Advantage token issuance is a\n    platform-to-tool exchange for registered tools, not a public developer OAuth surface. No scopes\n    are advertised anywhere on it, so none are recorded.\nauthorization_vocabularies_observed:\n- name: Sakai tool functions\n  surface: https://panda.ecs.kyoto-u.ac.jp/direct/tool.json\n  operator: institution\n  machine_readable: true\n  detail: >-\n    The PandA tool registry publishes each tool's required permission in a `functions.require` field\n    (for example \"site.upd\" on the Site Group Manager Helper). This is Sakai's internal permission\n    vocabulary, readable by anyone, and it is the closest thing to a published authorization model on\n    any Kyoto surface. It is NOT an OAuth scope vocabulary and must not be scored as one: it governs\n    in-application permissions for authenticated\
  \ university accounts.\n  evidence:\n    url: https://panda.ecs.kyoto-u.ac.jp/direct/tool.json\n    status: 200\n- name: SAML attribute release\n  surface: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth\n  operator: institution\n  machine_readable: true\n  detail: >-\n    Authorization to Kyoto University services is expressed as SAML attribute release from the IIMC\n    Shibboleth IdP to federation service providers, governed by GakuNin policy and, per the IIMC,\n    by committee approval for each new service-provider connection. Attribute release is the real\n    access-control vocabulary in a university federation, but it is negotiated per relying party\n    rather than published as a self-service scope list.\n  evidence:\n    url: https://authidp1.iimc.kyoto-u.ac.jp/idp/shibboleth\n    status: 200\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyoto/refs/heads/main/scopes/kyoto-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Japan
- National University
- Research Repository
- Research Data
- Identity Federation
- Learning Management
- Open Access
- Research Computing
- Scholarly
token_urls: []
---
