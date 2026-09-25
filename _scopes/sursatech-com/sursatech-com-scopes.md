---
authorization_urls: []
description: ''
docs: https://api.sursatech.com/auth.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Sursatech Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SursaTech publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SursaTech API on a user''s behalf.


  Tokens are issued from https://api.sursatech.com/api/a2a/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SursaTech
provider_slug: sursatech-com
schemes:
- bearerFormat: opaque
  flows:
  - client_authentication: none (anonymous registration; token_endpoint_auth_methods_supported ["none"])
    flow: clientCredentials
    registrationUrl: https://api.sursatech.com/api/a2a/register
    tokenUrl: https://api.sursatech.com/api/a2a/token
  issuer: https://api.sursatech.com
  name: bearerAuth
  scheme: bearer
  source: a2a/sursatech-com-agent-card.json
  type: http
scope_count: 4
scope_names:
- a2a
- company.read
- requirements.write
- booking.write
scopes:
- description: The A2A agent scope. The scope every anonymous self-registration token receives (auth.md); the token endpoint's observed response carries scope "a2a".
  flows:
  - clientCredentials
  scope: a2a
- description: Read company knowledge (profile, services, portfolio, process, pricing). Listed in scopes_supported; the provider publishes no per-scope description, so this reading is inferred from the scope name and the read skills on the agent card.
  flows:
  - clientCredentials
  scope: company.read
- description: Persist a structured project requirement (the capture_lead_requirement skill). Listed in scopes_supported; no per-scope description is published — inferred from the name.
  flows:
  - clientCredentials
  scope: requirements.write
- description: Consultation booking, payment checkout, confirmation and cancel/reschedule (the four guarded booking skills). Listed in scopes_supported; no per-scope description is published — inferred from the name.
  flows:
  - clientCredentials
  scope: booking.write
slug: sursatech-com-scopes
source_filename: sursatech-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://api.sursatech.com/.well-known/oauth-authorization-server (scopes_supported), https://api.sursatech.com/.well-known/oauth-protected-resource (scopes_supported), https://api.sursatech.com/auth.md (\"Credential Use\"), and the observed token response on 2026-09-19.\ndocs: https://api.sursatech.com/auth.md\nopenapi_note: No OpenAPI is served, so derive-oauth-scopes.py found nothing to derive; every scope below is the provider's own published list.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: opaque\n  source: a2a/sursatech-com-agent-card.json\n  issuer: https://api.sursatech.com\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.sursatech.com/api/a2a/token\n    registrationUrl: https://api.sursatech.com/api/a2a/register\n    client_authentication: none (anonymous registration; token_endpoint_auth_methods_supported [\"none\"])\nscope_count: 4\nscopes:\n- scope: a2a\n  description:\
  \ The A2A agent scope. The scope every anonymous self-registration token receives (auth.md); the token endpoint's observed response carries scope \"a2a\".\n  granted_to: anonymous self-registered agents\n  flows: [clientCredentials]\n  sources:\n  - https://api.sursatech.com/.well-known/oauth-authorization-server\n  - https://api.sursatech.com/auth.md\n- scope: company.read\n  description: Read company knowledge (profile, services, portfolio, process, pricing). Listed in scopes_supported; the provider publishes no per-scope description, so this reading is inferred from the scope name and the read skills on the agent card.\n  description_published: false\n  flows: [clientCredentials]\n  sources:\n  - https://api.sursatech.com/.well-known/oauth-authorization-server\n- scope: requirements.write\n  description: Persist a structured project requirement (the capture_lead_requirement skill). Listed in scopes_supported; no per-scope description is published — inferred from the name.\n  description_published:\
  \ false\n  flows: [clientCredentials]\n  sources:\n  - https://api.sursatech.com/.well-known/oauth-authorization-server\n- scope: booking.write\n  description: Consultation booking, payment checkout, confirmation and cancel/reschedule (the four guarded booking skills). Listed in scopes_supported; no per-scope description is published — inferred from the name.\n  description_published: false\n  flows: [clientCredentials]\n  sources:\n  - https://api.sursatech.com/.well-known/oauth-authorization-server\nnotes:\n- The provider publishes the scope NAMES but no scope reference page: auth.md lists them in one line and says only that self-registration tokens receive the A2A agent scope. Which skills require which of the other three scopes, and how a partner obtains them (\"minted out-of-band for known partners\"), is not documented.\n- No scope is requested in the observed anonymous token exchange; the default is a2a.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sursatech-com/refs/heads/main/scopes/sursatech-com-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- AI Agents
- A2A
- AI Consulting
- Product Engineering
- Software Development
- RAG
- QA Automation
- Nepal
- Agent-Native
- Company
token_urls:
- https://api.sursatech.com/api/a2a/token
---
