---
api_specs:
- filename: notarize-cost-centers-api-openapi.yml
  format: yaml
  label: Notarize Cost Centers API
  slug: notarize-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-cost-centers-api-openapi.yml
- filename: notarize-documents-api-openapi.yml
  format: yaml
  label: Notarize Documents API
  slug: notarize-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-documents-api-openapi.yml
- filename: notarize-eligibilities-api-openapi.yml
  format: yaml
  label: Notarize Eligibilities API
  slug: notarize-eligibilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-eligibilities-api-openapi.yml
- filename: notarize-enote-api-openapi.yml
  format: yaml
  label: Notarize E Note API
  slug: notarize-enote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-enote-api-openapi.yml
- filename: notarize-integrations-api-openapi.yml
  format: yaml
  label: Notarize Integrations API
  slug: notarize-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-integrations-api-openapi.yml
- filename: notarize-notaries-api-openapi.yml
  format: yaml
  label: Notarize Notaries API
  slug: notarize-notaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-notaries-api-openapi.yml
- filename: notarize-notarization-records-api-openapi.yml
  format: yaml
  label: Notarize Notarization Records API
  slug: notarize-notarization-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-notarization-records-api-openapi.yml
- filename: notarize-oauth-2-0-api-openapi.yml
  format: yaml
  label: Notarize OAuth 2.0 API
  slug: notarize-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-oauth-2-0-api-openapi.yml
- filename: notarize-oid4vp-api-openapi.yml
  format: yaml
  label: Notarize OID4VP API
  slug: notarize-oid4vp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-oid4vp-api-openapi.yml
- filename: notarize-organizations-api-openapi.yml
  format: yaml
  label: Notarize Organizations API
  slug: notarize-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-organizations-api-openapi.yml
- filename: notarize-referrals-api-openapi.yml
  format: yaml
  label: Notarize Referrals API
  slug: notarize-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-referrals-api-openapi.yml
- filename: notarize-scim-api-openapi.yml
  format: yaml
  label: Notarize SCIM API
  slug: notarize-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-scim-api-openapi.yml
- filename: notarize-security-events-api-openapi.yml
  format: yaml
  label: Notarize Security Events API
  slug: notarize-security-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-security-events-api-openapi.yml
- filename: notarize-templates-api-openapi.yml
  format: yaml
  label: Notarize Templates API
  slug: notarize-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-templates-api-openapi.yml
- filename: notarize-title-agencies-api-openapi.yml
  format: yaml
  label: Notarize Title Agencies API
  slug: notarize-title-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-title-agencies-api-openapi.yml
- filename: notarize-transactions-api-openapi.yml
  format: yaml
  label: Notarize Transactions API
  slug: notarize-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-transactions-api-openapi.yml
- filename: notarize-webhooks-api-openapi.yml
  format: yaml
  label: Notarize Webhooks API
  slug: notarize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/openapi/notarize-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://dev.proof.com/docs/oauth-client-credentials
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Notarize Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Notarize publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Notarize API on a user''s behalf.


  Tokens are issued from https://api.proof.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Notarize
provider_slug: notarize
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.proof.com/oauth/v2/token
  name: OAuth2
  source: https://dev.proof.com/docs/oauth-client-credentials
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Proof API resources.
  flows:
  - clientCredentials
  scope: read
- description: Write access to create and modify Proof API resources.
  flows:
  - clientCredentials
  scope: write
slug: notarize-scopes
source_filename: notarize-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://dev.proof.com/docs/oauth-client-credentials\ndocs: https://dev.proof.com/docs/oauth-client-credentials\nnotes: >-\n  Proof's OAuth 2.0 client_credentials grant issues tokens with a coarse\n  read/write scope pair (seen in the token and token/info responses:\n  \"scope\":\"read write\"). Proof does not publish a fine-grained per-resource\n  scope catalog; access is primarily differentiated by API-key access level\n  (Full Access vs Client Only) rather than OAuth scopes.\nschemes:\n  - name: OAuth2\n    source: https://dev.proof.com/docs/oauth-client-credentials\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.proof.com/oauth/v2/token\nscopes:\n  - scope: read\n    description: Read access to Proof API resources.\n    flows: [clientCredentials]\n    sources: [https://dev.proof.com/docs/oauth-client-credentials]\n  - scope: write\n    description: Write access to create and modify Proof API resources.\n\
  \    flows: [clientCredentials]\n    sources: [https://dev.proof.com/docs/oauth-client-credentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notarize/refs/heads/main/scopes/notarize-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Company
- PropTech
- Notarization
- Remote Online Notarization
- Identity Verification
- E-Signature
- Digital Credentials
- Real Estate
- Mortgage
- Legal Tech
token_bound: false
token_urls:
- https://api.proof.com/oauth/v2/token
---
