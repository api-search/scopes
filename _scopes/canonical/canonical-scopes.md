---
api_specs:
- filename: canonical-snapd-rest-api-openapi.yml
  format: yaml
  label: snapd REST API
  slug: snapd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snapd-rest-api-openapi.yml
- filename: canonical-landscape-debarchive-api-openapi.yml
  format: yaml
  label: Landscape API
  slug: landscape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-landscape-debarchive-api-openapi.yml
- filename: canonical-assertions-api-openapi.yml
  format: yaml
  label: Canonical Assertions API
  slug: canonical-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-assertions-api-openapi.yml
- filename: canonical-search-api-openapi.yml
  format: yaml
  label: Canonical Search API
  slug: canonical-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-search-api-openapi.yml
- filename: canonical-snaps-api-openapi.yml
  format: yaml
  label: Canonical Snaps API
  slug: canonical-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snaps-api-openapi.yml
- filename: canonical-lxd-rest-api-openapi.yml
  format: yaml
  label: LXD REST API
  slug: lxd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-lxd-rest-api-openapi.yml
- filename: canonical-ubuntu-security-api-openapi.json
  format: json
  label: Ubuntu Security API
  slug: ubuntu-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-ubuntu-security-api-openapi.json
- filename: canonical-pebble-api-openapi.yml
  format: yaml
  label: Pebble API
  slug: pebble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-pebble-api-openapi.yml
- filename: canonical-testflinger-api-openapi.json
  format: json
  label: Testflinger API
  slug: testflinger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-testflinger-api-openapi.json
- filename: canonical-hardware-api-openapi.json
  format: json
  label: Ubuntu Hardware API (hwapi)
  slug: hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-hardware-api-openapi.json
- filename: canonical-identity-platform-api-openapi.yml
  format: yaml
  label: Canonical Identity Platform API
  slug: identity-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-identity-platform-api-openapi.yml
- filename: canonical-test-observer-api-openapi.json
  format: json
  label: Test Observer API
  slug: test-observer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-test-observer-api-openapi.json
- filename: canonical-anbox-cloud-ams-api-openapi.json
  format: json
  label: Anbox Cloud AMS API
  slug: anbox-cloud-ams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-cloud-ams-api-openapi.json
- filename: canonical-anbox-stream-gateway-api-openapi.json
  format: json
  label: Anbox Stream Gateway API
  slug: anbox-stream-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-stream-gateway-api-openapi.json
- filename: canonical-cos-registration-server-api-openapi.yml
  format: yaml
  label: COS Registration Server API
  slug: cos-registration-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-cos-registration-server-api-openapi.yml
- filename: canonical-microceph-api-openapi.yml
  format: yaml
  label: MicroCeph REST API
  slug: microceph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-microceph-api-openapi.yml
authorization_urls:
- https://example.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Canonical Scopes
name_suffix: OAuth Scopes
note: The only OAuth2 surface in the Canonical portfolio is the Identity Platform API, which is software a customer deploys rather than a Canonical-hosted service; its spec declares the standard OIDC scopes against https://example.com placeholder endpoints. The Snap Store and Charmhub use macaroons and Launchpad uses OAuth 1.0a — neither has a scope reference to search for. No scopes documentation page exists to upgrade this file with; method stays derived.
overview: 'Canonical publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canonical API on a user''s behalf.


  Tokens are issued from https://example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canonical
provider_slug: canonical
schemes:
- flows:
  - authorizationUrl: https://example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/oauth/token
  name: OAuth2
  source: openapi/canonical-identity-platform-api-openapi.yml
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: email
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: profile
slug: canonical-scopes
source_filename: canonical-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/canonical-identity-platform-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/canonical-identity-platform-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/oauth/authorize\n    tokenUrl: https://example.com/oauth/token\nscopes:\n- scope: email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canonical-identity-platform-api-openapi.yml\n- scope: openid\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canonical-identity-platform-api-openapi.yml\n- scope: profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canonical-identity-platform-api-openapi.yml\nnote: The only OAuth2 surface in the Canonical portfolio is the Identity Platform API, which is software\n  a customer deploys rather than a Canonical-hosted service; its spec declares the standard OIDC scopes\n  against https://example.com placeholder endpoints. The Snap Store and Charmhub\
  \ use macaroons and Launchpad\n  uses OAuth 1.0a — neither has a scope reference to search for. No scopes documentation page exists to\n  upgrade this file with; method stays derived.\ndocs: null\nsearched:\n  date: '2026-09-05'\n  result: no OAuth scope reference page published by Canonical for any product\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/scopes/canonical-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Cloud
- Linux
- Open-Source
- Ubuntu
- Containers
- Bare Metal
- Charms
- Identity
token_urls:
- https://example.com/oauth/token
---
