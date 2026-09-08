---
authorization_urls: []
description: 'OAuth 2.0 scopes accepted by the Clearstream API Platform token server at /authmanager/oauth2/access_token. Clearstream requires a two-part scope string: the literal `allow` scope on every request, plus at least one API-specific scope naming the resource being called. The scopes below were disclosed by the platform itself in 403 responses to unauthenticated probes — this is not a derived or inferred list, but it is also not exhaustive: the full catalogue of scopes a given consumer may request is returned by the token endpoint in the 400 body when an invalid scope is requested, and that requires credentials to see.'
docs:
- https://www.clearstream.com/caas/v1/media/2934048/data/3fa3fec668d8dd198e9bed4df879b26b/api-developer-guide.pdf
- https://www.clearstream.com/clearstream-en/res-library/connectivity/clearstream-api-services-2916788
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clearstream Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Clearstream publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clearstream API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clearstream
provider_slug: clearstream
schemes: []
scope_count: 4
scope_names:
- allow
- ocapi-playground-v1
- scim2-ext-v1
- cmax-api
scopes:
- description: Required on every token request. Present in every observed required_scopes.mandatory field; on its own it grants nothing.
  flows: []
  scope: allow
- description: Grants the free-of-charge synthetic Playground API used for connectivity testing and initial onboarding (endpoints /playground/v1/info and /playground/v1/echo).
  flows: []
  scope: ocapi-playground-v1
- description: Grants the SCIM 2.0 User Management API for provisioning, maintaining and monitoring Xact Web Portal users. The developer guide notes that most calls additionally require the Xact SCIM Admin or SCIM Read-Only role on the consumer.
  flows: []
  scope: scim2-ext-v1
- description: Grants the CmaX collateral management API surface. Discovered by probe; Clearstream's public pages describe CmaX as the triparty collateral platform but do not yet document this REST surface outside the gated Digital Business Platform catalogue.
  flows: []
  scope: cmax-api
slug: clearstream-scopes
source_filename: clearstream-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Clearstream\nproviderId: clearstream\ngenerated: '2026-09-05'\nmodified: '2026-09-05'\nmethod: probed\nsource: >-\n  Live unauthenticated GETs against the Clearstream API Platform pre-production host\n  https://api-t2s-test.clearstream.com on 2026-09-05. Each protected prefix answers 403 with a\n  JSON body that names the exact OAuth scopes it requires. Scope semantics cross-read from the\n  Clearstream API Developer Guide (August 2025).\ndocs:\n  - https://www.clearstream.com/caas/v1/media/2934048/data/3fa3fec668d8dd198e9bed4df879b26b/api-developer-guide.pdf\n  - https://www.clearstream.com/clearstream-en/res-library/connectivity/clearstream-api-services-2916788\ndescription: >-\n  OAuth 2.0 scopes accepted by the Clearstream API Platform token server at\n  /authmanager/oauth2/access_token. Clearstream requires a two-part scope string: the literal\n  `allow` scope on every request, plus at least\
  \ one API-specific scope naming the resource being\n  called. The scopes below were disclosed by the platform itself in 403 responses to\n  unauthenticated probes — this is not a derived or inferred list, but it is also not exhaustive:\n  the full catalogue of scopes a given consumer may request is returned by the token endpoint in\n  the 400 body when an invalid scope is requested, and that requires credentials to see.\nscope_string_format: '<mandatory scope> <one or more API scopes>, space separated'\nscopes:\n  - scope: allow\n    kind: mandatory\n    description: >-\n      Required on every token request. Present in every observed required_scopes.mandatory\n      field; on its own it grants nothing.\n    evidence: https://api-t2s-test.clearstream.com/playground/v1/info\n    evidence_status: 403\n  - scope: ocapi-playground-v1\n    kind: api\n    api: Clearstream API Playground\n    path_prefix: /playground\n    description: >-\n      Grants the free-of-charge synthetic Playground API\
  \ used for connectivity testing and\n      initial onboarding (endpoints /playground/v1/info and /playground/v1/echo).\n    evidence: https://api-t2s-test.clearstream.com/playground/v1/info\n    evidence_status: 403\n  - scope: scim2-ext-v1\n    kind: api\n    api: Xact Web Portal User Management (SCIM 2.0)\n    path_prefix: /scim2\n    description: >-\n      Grants the SCIM 2.0 User Management API for provisioning, maintaining and monitoring Xact\n      Web Portal users. The developer guide notes that most calls additionally require the Xact\n      SCIM Admin or SCIM Read-Only role on the consumer.\n    evidence: https://api-t2s-test.clearstream.com/scim2\n    evidence_status: 403\n  - scope: cmax-api\n    kind: api\n    api: CmaX triparty collateral management\n    path_prefix: /cmax\n    description: >-\n      Grants the CmaX collateral management API surface. Discovered by probe; Clearstream's\n      public pages describe CmaX as the triparty collateral platform but do not yet document\n\
  \      this REST surface outside the gated Digital Business Platform catalogue.\n    evidence: https://api-t2s-test.clearstream.com/cmax/v1\n    evidence_status: 403\ncompleteness:\n  exhaustive: false\n  note: >-\n    Only prefixes that could be named from Clearstream's own published material were probed;\n    a 200 HTML landing page is the platform's catch-all for an unknown path, so absence of a\n    403 is not proof a surface does not exist. The authoritative list lives in the Deutsche\n    Börse Digital Business Platform API catalogue, which requires registration\n    (https://developer.deutsche-boerse.com/console/api/v2/apis returned 401 on 2026-09-05).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearstream/refs/heads/main/scopes/clearstream-scopes.yml
summary_line: 4 scopes
tags:
- API Platform
- Capital Markets
- Collateral Management
- Custody
- Financial-Services
- ISO 15022
- ISO 20022
- Mutual TLS
- OAuth 2.0
- Post-Trade
- Post-Trade Infrastructure
- SCIM
- Securities
- Settlement
- Swift
token_urls: []
---
