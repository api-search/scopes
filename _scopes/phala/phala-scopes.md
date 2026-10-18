---
api_specs:
- filename: phala-apps-api-openapi.yml
  format: yaml
  label: Phala Network Apps API
  slug: phala-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-api-openapi.yml
- filename: phala-apps-kms-info-api-openapi.yml
  format: yaml
  label: Phala Network Apps Kms Info API
  slug: phala-apps-kms-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-kms-info-api-openapi.yml
- filename: phala-apps-pending-updates-api-openapi.yml
  format: yaml
  label: Phala Network Apps Pending Updates API
  slug: phala-apps-pending-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-apps-pending-updates-api-openapi.yml
- filename: phala-attestations-api-openapi.yml
  format: yaml
  label: Phala Network Attestations API
  slug: phala-attestations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-attestations-api-openapi.yml
- filename: phala-cvms-api-openapi.yml
  format: yaml
  label: Phala Network CVMs API
  slug: phala-cvms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-api-openapi.yml
- filename: phala-cvms-network-config-api-openapi.yml
  format: yaml
  label: Phala Network Cvms Network Config API
  slug: phala-cvms-network-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-cvms-network-config-api-openapi.yml
- filename: phala-instance-types-api-openapi.yml
  format: yaml
  label: Phala Network Instance Types API
  slug: phala-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-instance-types-api-openapi.yml
- filename: phala-kms-api-openapi.yml
  format: yaml
  label: Phala Network KMS API
  slug: phala-kms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-kms-api-openapi.yml
- filename: phala-ssh-keys-api-openapi.yml
  format: yaml
  label: Phala Network SSH Keys API
  slug: phala-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-ssh-keys-api-openapi.yml
- filename: phala-webhooks-api-openapi.yml
  format: yaml
  label: Phala Network Webhooks API
  slug: phala-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/openapi/phala-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Phala Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Phala Network uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Phala Network
provider_slug: phala
schemes:
- flows:
  - flow: authorizationCode
    tokenUrl: token
  name: OAuth2AuthorizationCodeBearer
  source: openapi/phala-cloud-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: phala-scopes
source_filename: phala-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/phala-cloud-api-openapi.yml\nschemes:\n- name: OAuth2AuthorizationCodeBearer\n  source: openapi/phala-cloud-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    tokenUrl: token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phala/refs/heads/main/scopes/phala-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Confidential Computing
- Trusted Execution Environments
- Inference
- Cloud Infrastructure
- Attestation
- LLM Router
token_bound: false
token_urls:
- token
---
