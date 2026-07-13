---
api_specs:
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Studios API
  slug: shootproof-studios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Events & Galleries API
  slug: shootproof-events-galleries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Photos API
  slug: shootproof-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Clients API
  slug: shootproof-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Orders API
  slug: shootproof-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
- filename: shootproof-openapi.yml
  format: yaml
  label: ShootProof Contracts API
  slug: shootproof-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/openapi/shootproof-openapi.yml
authorization_urls:
- https://auth.shootproof.com/oauth2/authorization/new
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Shootproof Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ShootProof publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ShootProof API on a user''s behalf.


  Tokens are issued from https://auth.shootproof.com/oauth2/authorization/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ShootProof
provider_slug: shootproof
schemes:
- flows:
  - authorizationUrl: https://auth.shootproof.com/oauth2/authorization/new
    flow: authorizationCode
    tokenUrl: https://auth.shootproof.com/oauth2/authorization/token
  name: shootProofAuth
  source: openapi/shootproof-openapi.yml
scope_count: 5
scope_names:
- studio
- studio.brand.read-only
- studio.info.read-only
- studio.order.lab-shipment.read-write
- studio.order.read-write
scopes:
- description: read and write access to your Studio Panel data
  flows:
  - authorizationCode
  scope: studio
- description: read access to your Studio Panel Brand data
  flows:
  - authorizationCode
  scope: studio.brand.read-only
- description: read access to your Studio Panel account data
  flows:
  - authorizationCode
  scope: studio.info.read-only
- description: read and write access to your Studio Panel Order shipment data
  flows:
  - authorizationCode
  scope: studio.order.lab-shipment.read-write
- description: read and write access to your Studio Panel Order data
  flows:
  - authorizationCode
  scope: studio.order.read-write
slug: shootproof-scopes
source_filename: shootproof-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shootproof-openapi.yml\nschemes:\n- name: shootProofAuth\n  source: openapi/shootproof-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.shootproof.com/oauth2/authorization/new\n    tokenUrl: https://auth.shootproof.com/oauth2/authorization/token\nscopes:\n- scope: studio\n  description: read and write access to your Studio Panel data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shootproof-openapi.yml\n- scope: studio.brand.read-only\n  description: read access to your Studio Panel Brand data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shootproof-openapi.yml\n- scope: studio.info.read-only\n  description: read access to your Studio Panel account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shootproof-openapi.yml\n- scope: studio.order.lab-shipment.read-write\n  description: read and write access to your Studio Panel Order shipment data\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/shootproof-openapi.yml\n- scope: studio.order.read-write\n  description: read and write access to your Studio Panel Order data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/shootproof-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/scopes/shootproof-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Photography
- Client Galleries
- Proofing
- Digital Downloads
- Photo Studio Management
- E-Commerce
- SaaS
token_urls:
- https://auth.shootproof.com/oauth2/authorization/token
---
