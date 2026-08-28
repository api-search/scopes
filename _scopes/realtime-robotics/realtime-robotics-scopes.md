---
authorization_urls: []
description: Realtime Robotics declares no oauth2 securitySchemes anywhere - it publishes no OpenAPI at all - so this scope list is read directly from the OpenID Connect discovery document its identity service publishes at clerk.rtr.ai. These are the scopes the Resolver Cloud identity layer advertises; they are identity and organisation scopes, not resource scopes over a Resolver API, and no scope-to-endpoint mapping is published because the Resolver REST API itself is documented as not yet publicly available.
docs: https://resolver.rtr.ai/docs/user_guide/resolver/log_in/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Realtime Robotics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Realtime Robotics uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Realtime Robotics
provider_slug: realtime-robotics
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: realtime-robotics-scopes
source_filename: realtime-robotics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://clerk.rtr.ai/.well-known/openid-configuration\ndocs: https://resolver.rtr.ai/docs/user_guide/resolver/log_in/\nname: Realtime Robotics OAuth scopes\ndescription: >-\n  Realtime Robotics declares no oauth2 securitySchemes anywhere - it publishes no\n  OpenAPI at all - so this scope list is read directly from the OpenID Connect\n  discovery document its identity service publishes at clerk.rtr.ai. These are the\n  scopes the Resolver Cloud identity layer advertises; they are identity and\n  organisation scopes, not resource scopes over a Resolver API, and no scope-to-endpoint\n  mapping is published because the Resolver REST API itself is documented as not yet\n  publicly available.\nissuer: https://clerk.rtr.ai\napplies_to: realtime-robotics:resolver-cloud\nscopes:\n- name: openid\n  description: OpenID Connect - request an ID token for the authenticated subject.\n- name: profile\n  description: Profile claims (name, given_name,\
  \ family_name, preferred_username, picture).\n- name: email\n  description: Email address and email_verified claim.\n- name: offline_access\n  description: Issue a refresh token so the client can renew access without re-prompting.\n- name: user:org:read\n  description: Read the organisation membership of the authenticated user (org_id claim).\n- name: public_metadata\n  description: Read the user's public metadata.\n- name: private_metadata\n  description: Read the user's private metadata.\nclaims_supported:\n- sub\n- iss\n- aud\n- exp\n- iat\n- email\n- email_verified\n- name\n- given_name\n- family_name\n- preferred_username\n- picture\n- org_id\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://clerk.rtr.ai/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtime-robotics/refs/heads/main/scopes/realtime-robotics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Robotics
- Motion Planning
- Industrial Automation
- Manufacturing
- Simulation
- Collision Avoidance
- Robot Programming
- Machine Vision
- Digital Twin
token_urls: []
---
