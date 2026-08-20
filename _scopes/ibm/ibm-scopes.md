---
api_specs:
- filename: ibm-api-keys-api-openapi.yml
  format: yaml
  label: IBM API Keys API
  slug: ibm-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-api-keys-api-openapi.yml
- filename: ibm-claim-rules-api-openapi.yml
  format: yaml
  label: IBM Claim Rules API
  slug: ibm-claim-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-claim-rules-api-openapi.yml
- filename: ibm-policies-api-openapi.yml
  format: yaml
  label: IBM Policies API
  slug: ibm-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-policies-api-openapi.yml
- filename: ibm-roles-api-openapi.yml
  format: yaml
  label: IBM Roles API
  slug: ibm-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-roles-api-openapi.yml
- filename: ibm-service-ids-api-openapi.yml
  format: yaml
  label: IBM Service IDs API
  slug: ibm-service-ids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-service-ids-api-openapi.yml
- filename: ibm-tokens-api-openapi.yml
  format: yaml
  label: IBM Tokens API
  slug: ibm-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-tokens-api-openapi.yml
- filename: ibm-trusted-profiles-api-openapi.yml
  format: yaml
  label: IBM Trusted Profiles API
  slug: ibm-trusted-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/openapi/ibm-trusted-profiles-api-openapi.yml
authorization_urls: []
description: ''
docs: https://cloud.ibm.com/docs/account?topic=account-iamoverview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ibm Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'IBM publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the IBM API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IBM
provider_slug: ibm
schemes:
- authorization_endpoint: https://identity-3.us-east.iam.cloud.ibm.com/identity/authorize
  grant_types:
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ibm:params:oauth:grant-type:apikey
  - urn:ibm:params:oauth:grant-type:delegated-refresh-token
  - urn:ibm:params:oauth:grant-type:iam-authz
  issuer: https://iam.cloud.ibm.com/identity
  name: IBM Cloud IAM (OpenID Connect)
  token_endpoint: https://identity-3.us-east.iam.cloud.ibm.com/identity/token
scope_count: 7
scope_names:
- openid
- email
- profile
- ibm
- roles
- containers-kubernetes
- containers-openshift
scopes:
- description: Request an OpenID Connect ID token.
  flows: []
  scope: openid
- description: Include the user's email in identity claims.
  flows: []
  scope: email
- description: Include the user's profile in identity claims.
  flows: []
  scope: profile
- description: IBM Cloud platform identity scope.
  flows: []
  scope: ibm
- description: Include IAM role information in the token.
  flows: []
  scope: roles
- description: Scope for IBM Cloud Kubernetes Service access tokens.
  flows: []
  scope: containers-kubernetes
- description: Scope for IBM Cloud OpenShift access tokens.
  flows: []
  scope: containers-openshift
slug: ibm-scopes
source_filename: ibm-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://iam.cloud.ibm.com/identity/.well-known/openid-configuration\ndocs: https://cloud.ibm.com/docs/account?topic=account-iamoverview\nnotes: >-\n  The IBM Cloud IAM identity endpoint is an OAuth 2.0 / OpenID Connect authorization\n  server. The IAM management OpenAPI (openapi/ibm-cloud-iam.yml) itself uses http\n  bearer JWT, but the tokens are minted by this OAuth server, whose live OIDC\n  discovery document advertises the scopes and grant types below. Access to IBM\n  Cloud resources is governed by IAM access policies (roles + resource attributes),\n  not fine-grained OAuth scopes — these OIDC scopes control identity/session claims.\nschemes:\n  - name: IBM Cloud IAM (OpenID Connect)\n    issuer: https://iam.cloud.ibm.com/identity\n    authorization_endpoint: https://identity-3.us-east.iam.cloud.ibm.com/identity/authorize\n    token_endpoint: https://identity-3.us-east.iam.cloud.ibm.com/identity/token\n    grant_types:\n\
  \      - authorization_code\n      - refresh_token\n      - password\n      - implicit\n      - \"urn:ibm:params:oauth:grant-type:apikey\"\n      - \"urn:ibm:params:oauth:grant-type:delegated-refresh-token\"\n      - \"urn:ibm:params:oauth:grant-type:iam-authz\"\nscopes:\n  - scope: openid\n    description: Request an OpenID Connect ID token.\n  - scope: email\n    description: Include the user's email in identity claims.\n  - scope: profile\n    description: Include the user's profile in identity claims.\n  - scope: ibm\n    description: IBM Cloud platform identity scope.\n  - scope: roles\n    description: Include IAM role information in the token.\n  - scope: containers-kubernetes\n    description: Scope for IBM Cloud Kubernetes Service access tokens.\n  - scope: containers-openshift\n    description: Scope for IBM Cloud OpenShift access tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibm/refs/heads/main/scopes/ibm-scopes.yml
summary_line: 7 scopes
tags:
- API Management
- Artificial Intelligence
- Billing
- Cloud Computing
- Containers
- Data Governance
- Databases
- DevOps
- Enterprise
- Generative AI
- Hybrid Cloud
- Infrastructure
- Machine-Learning
- Networking
- Observability
- Security
- Serverless
- Storage
- Watson
- Watsonx
- Fortune 100
token_urls: []
---
