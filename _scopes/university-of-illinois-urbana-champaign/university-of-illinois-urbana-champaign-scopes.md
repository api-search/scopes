---
api_specs:
- filename: university-of-illinois-urbana-champaign-services-api-openapi.yml
  format: yaml
  label: Rokwire Core Building Block API
  slug: rokwire-core-building-block
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-services-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-client-api-openapi.yml
  format: yaml
  label: Rokwire Gateway Building Block API
  slug: rokwire-gateway-building-block
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-client-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: University Of Illinois Urbana Champaign Scopes
name_suffix: OAuth Scopes
note: UIUC publishes NO enumerated scope list. The Core building block's OIDC discovery document returns only issuer and jwks_uri — there is no scopes_supported array to read — so nothing here is a scope string the institution has advertised. What IS published, in the Core OpenAPI that UIUC authors, is the scope GRAMMAR and the objects that carry scopes; that grammar and the worked examples in the spec are recorded below. Individual scope strings are per-deployment, minted when a service registers, and are NOT enumerable from outside. Do not read this file as a catalog of grantable scopes.
overview: 'University of Illinois Urbana-Champaign uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Illinois Urbana-Champaign
provider_slug: university-of-illinois-urbana-champaign
schemes:
- bearerFormat: JWT
  discovery: https://api.rokwire.illinois.edu/core/.well-known/openid-configuration
  discovery_completeness: Minimal — issuer and jwks_uri only. No authorization_endpoint, token_endpoint or scopes_supported.
  issuer: https://api.rokwire.illinois.edu/core
  jwks_uri: https://api.rokwire.illinois.edu/core/tps/auth-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/university-of-illinois-urbana-champaign-rokwire-core.yaml
  - openapi/_original/university-of-illinois-urbana-champaign-rokwire-gateway.yaml
  type: http
scope_count: 0
scope_names: []
scopes: []
slug: university-of-illinois-urbana-champaign-scopes
source_filename: university-of-illinois-urbana-champaign-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: >-\n  openapi/_original/university-of-illinois-urbana-champaign-rokwire-core.yaml,\n  openapi/_original/university-of-illinois-urbana-champaign-rokwire-gateway.yaml,\n  probed https://api.rokwire.illinois.edu/core/.well-known/openid-configuration\nnote: >-\n  UIUC publishes NO enumerated scope list. The Core building block's OIDC discovery document\n  returns only issuer and jwks_uri — there is no scopes_supported array to read — so nothing here\n  is a scope string the institution has advertised. What IS published, in the Core OpenAPI that\n  UIUC authors, is the scope GRAMMAR and the objects that carry scopes; that grammar and the\n  worked examples in the spec are recorded below. Individual scope strings are per-deployment,\n  minted when a service registers, and are NOT enumerable from outside. Do not read this file as a\n  catalog of grantable scopes.\noperator: institution\nschemes:\n- name: bearerAuth\n  type: http\n\
  \  scheme: bearer\n  bearerFormat: JWT\n  issuer: https://api.rokwire.illinois.edu/core\n  jwks_uri: https://api.rokwire.illinois.edu/core/tps/auth-keys\n  discovery: https://api.rokwire.illinois.edu/core/.well-known/openid-configuration\n  discovery_completeness: >-\n    Minimal — issuer and jwks_uri only. No authorization_endpoint, token_endpoint or\n    scopes_supported.\n  sources:\n  - openapi/_original/university-of-illinois-urbana-champaign-rokwire-core.yaml\n  - openapi/_original/university-of-illinois-urbana-champaign-rokwire-gateway.yaml\ngrammar:\n  pattern: '<service_id>:<resource>[.<sub-resource>]:<operation>'\n  examples_in_spec:\n  - core:resource.value:get\n  - core:resource.value2.get\n  detail: >-\n    A scope names the owning service (service_id), the resource path within it, and the operation.\n    Scopes are attached to three objects in the Core data model — AppOrgRole.scopes[],\n    ServiceAccount.scopes[] and ServiceReg.scopes[] — and are granted alongside, not instead\
  \ of,\n    the named Permission objects.\ncarriers:\n- object: ServiceScope\n  where: components.schemas.ServiceScope\n  fields:\n    scope: the scope string itself\n    required: whether the registering service demands it rather than requests it\n    explanation: the human-readable justification shown to the user at consent time\n  detail: >-\n    ServiceScope is the consent-facing unit. A service registration declares the scopes it needs,\n    marks each required or optional, and supplies the explanation a person sees before approving.\n- object: ServiceReg.scopes[]\n  where: components.schemas.ServiceReg\n  detail: >-\n    The full service registration record — service_id, host, first_party, pub_key and the\n    ServiceScope[] the service asks for. This is where a scope enters the system.\n- object: ServiceAccount.scopes[]\n  where: components.schemas.ServiceAccount\n  detail: >-\n    A machine identity scoped to an app_id/org_id pair, carrying both permissions[] and scopes[].\n   \
  \ Third-party service accounts are distinguished from first-party by ServiceAccount.first_party.\n- object: AppOrgRole.scopes[]\n  where: components.schemas.AppOrgRole\n  detail: >-\n    A role within one application/organization, carrying permissions[] (Permission objects with\n    assigners[]) and scopes[]. Roles are granted to accounts through\n    POST /admin/application/accounts/{id}/roles.\nconsent_surface:\n  detail: >-\n    POST /services/auth/authorize-service returns either an access_token with approved_scopes[]\n    or, when the service is not yet authorized, the service_reg record including its\n    ScopeService[] — so the calling client can render the consent screen. This is a real,\n    machine-readable consent handshake and is the strongest agent-facing property in the estate.\nadministration:\n  paths:\n  - /admin/application/permissions\n  - /admin/application/roles\n  - /admin/application/roles/{id}/permissions\n  - /admin/application/accounts/{id}/permissions\n  - /admin/application/accounts/{id}/roles\n\
  \  - /system/permissions\n  detail: >-\n    Permissions and roles are administered through the Core Admin and System APIs. Every one of\n    these paths is bearer-gated; an unauthenticated call returns 401 with the Rokwire error\n    envelope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/scopes/university-of-illinois-urbana-champaign-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Illinois
- Big Ten
- Land-Grant University
- Course Catalog
- Research Data
- Research Repository
- Open Data
- Identity Federation
- OAI-PMH
- Library
- Research Computing
- Open-Source
token_urls: []
---
