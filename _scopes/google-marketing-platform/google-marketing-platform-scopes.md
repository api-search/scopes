---
api_specs:
- filename: google-marketing-platform-v1alpha-api-openapi.yml
  format: yaml
  label: Google Marketing Platform Admin V1alpha API
  slug: google-marketing-platform-v1alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/openapi/google-marketing-platform-v1alpha-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: https://developers.google.com/marketing-platform/devguides/api/admin/v1/quickstart
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Marketing Platform Scopes
name_suffix: OAuth Scopes
note: Scope descriptions are the provider's own, read verbatim from the live Discovery Document (revision 20260813) auth.oauth2.scopes block. The per-method scope requirements come from the first-party service config published with the protos, which is more precise than the Discovery Document — Discovery lists both scopes as acceptable on read methods, while the service config pins the three write methods to the update scope alone. Upgraded from the derived pass, which had only spec-inferred descriptions.
overview: 'Google Marketing Platform Admin publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Marketing Platform Admin API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  note: accounts.google.com/.well-known/openid-configuration (saved to well-known/) advertises the v2 authorization endpoint https://accounts.google.com/o/oauth2/v2/auth and the same token endpoint.
  source: openapi/google-marketing-platform-v1alpha-api-openapi.yml
  type: oauth2
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/marketingplatformadmin.analytics.read
- https://www.googleapis.com/auth/marketingplatformadmin.analytics.update
scopes:
- description: View your Google Analytics product account data in GMP home
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.read
- description: Manage your Google Analytics product account data in GMP home
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.update
slug: google-marketing-platform-scopes
source_filename: google-marketing-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://marketingplatformadmin.googleapis.com/$discovery/rest?version=v1alpha\ndocs: https://developers.google.com/marketing-platform/devguides/api/admin/v1/quickstart\nalso_source:\n  - grpc/google-marketing-platform-service-config.yaml\n  - openapi/google-marketing-platform-v1alpha-api-openapi.yml\nnote: >-\n  Scope descriptions are the provider's own, read verbatim from the live\n  Discovery Document (revision 20260813) auth.oauth2.scopes block. The\n  per-method scope requirements come from the first-party service config\n  published with the protos, which is more precise than the Discovery Document\n  — Discovery lists both scopes as acceptable on read methods, while the\n  service config pins the three write methods to the update scope alone.\n  Upgraded from the derived pass, which had only spec-inferred descriptions.\nschemes:\n  - name: oauth2\n    type: oauth2\n    source: openapi/google-marketing-platform-v1alpha-api-openapi.yml\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://accounts.google.com/o/oauth2/auth\n        tokenUrl: https://oauth2.googleapis.com/token\n    note: >-\n      accounts.google.com/.well-known/openid-configuration (saved to\n      well-known/) advertises the v2 authorization endpoint\n      https://accounts.google.com/o/oauth2/v2/auth and the same token endpoint.\nscope_count: 2\nscopes:\n  - scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.read\n    description: View your Google Analytics product account data in GMP home\n    description_source: Discovery Document auth.oauth2.scopes (verbatim)\n    access: read\n    flows: [authorizationCode]\n    sources:\n      - openapi/google-marketing-platform-v1alpha-discovery.json\n      - openapi/google-marketing-platform-v1alpha-api-openapi.yml\n    grants:\n      - marketingplatformadmin.organizations.list\n      - marketingplatformadmin.organizations.get\n      - marketingplatformadmin.organizations.findSalesPartnerManagedClients\n\
  \      - marketingplatformadmin.organizations.reportPropertyUsage\n      - marketingplatformadmin.organizations.analyticsAccountLinks.list\n  - scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n    description: Manage your Google Analytics product account data in GMP home\n    description_source: Discovery Document auth.oauth2.scopes (verbatim)\n    access: write\n    flows: [authorizationCode]\n    sources:\n      - openapi/google-marketing-platform-v1alpha-discovery.json\n      - openapi/google-marketing-platform-v1alpha-api-openapi.yml\n    grants:\n      - marketingplatformadmin.organizations.analyticsAccountLinks.create\n      - marketingplatformadmin.organizations.analyticsAccountLinks.delete\n      - marketingplatformadmin.organizations.analyticsAccountLinks.setPropertyServiceLevel\n    note: >-\n      Also accepted on every read method, so a token holding only this scope\n      can do everything. There is no read-only-plus-one-write intermediate.\n\
  adjacent_scopes:\n  - scope: https://www.googleapis.com/auth/cloud-platform\n    required: false\n    note: >-\n      The quickstart's gcloud ADC command requests cloud-platform alongside the\n      analytics.read scope. It is needed for the Cloud project / quota-project\n      plumbing around the call, not by the API's own authentication rules —\n      the service config's canonical_scopes list does not include it.\n    source: https://developers.google.com/marketing-platform/devguides/api/admin/v1/quickstart\ncaveats:\n  - >-\n    A Cloud quota project is required on the credential and is not set by\n    default. Holding the right scope is necessary but not sufficient.\n  - >-\n    Scope failures and quota failures both surface as HTTP 403. Distinguish\n    them by error.errors[].reason — rateLimitExceeded is quota, anything else\n    is authorization.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/scopes/google-marketing-platform-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
token_urls:
- https://oauth2.googleapis.com/token
---
