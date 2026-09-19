---
api_specs:
- filename: iab-tech-lab-opendirect-1-5-1-swagger.yaml
  format: yaml
  label: OpenDirect API
  slug: opendirect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml
- filename: iab-tech-lab-agentic-advertising-api-openapi.yaml
  format: yaml
  label: IAB Agentic Advertising API
  slug: agentic-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-agentic-advertising-api-openapi.yaml
- filename: iab-tech-lab-seller-agent-openapi.json
  format: json
  label: Seller Agent API
  slug: seller-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-seller-agent-openapi.json
- filename: iab-tech-lab-buyer-agent-openapi.json
  format: json
  label: Buyer Agent API
  slug: buyer-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/openapi/iab-tech-lab-buyer-agent-openapi.json
authorization_urls:
- https://opendirect.example.com/connect/authorize
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Iab Tech Lab Scopes
name_suffix: OAuth Scopes
note: 'The OpenDirect 1.5.1 securityDefinitions is explicitly illustrative (''Example of one of OAuth 2.0 authorization flow''): the one scope, https://opendirect.example.com/scope/example, is a placeholder. OpenDirect leaves the OAuth authorization server and scopes to each implementing seller, so no real scope catalog exists to search for; the seller-agent reference implementation uses static API keys with buyer/operator roles instead (authentication/).'
overview: 'IAB Tech Lab publishes 1 OAuth 2.0 scope via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the IAB Tech Lab API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: IAB Tech Lab
provider_slug: iab-tech-lab
schemes:
- description: Example of one of OAuth 2.0 authorization flow that can be used according to specification.
  flows:
  - authorizationUrl: https://opendirect.example.com/connect/authorize
    flow: implicit
  name: OauthSecurity
  source: openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml
scope_count: 1
scope_names:
- https://opendirect.example.com/scope/example
scopes:
- description: Example scope
  flows:
  - implicit
  scope: https://opendirect.example.com/scope/example
slug: iab-tech-lab-scopes
source_filename: iab-tech-lab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: derived\nsource: openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml\nschemes:\n- name: OauthSecurity\n  source: openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://opendirect.example.com/connect/authorize\n  description: Example of one of OAuth 2.0 authorization flow that can be used according to specification.\nscopes:\n- scope: https://opendirect.example.com/scope/example\n  description: Example scope\n  flows:\n  - implicit\n  sources:\n  - openapi/iab-tech-lab-opendirect-1-5-1-swagger.yaml\nnote: 'The OpenDirect 1.5.1 securityDefinitions is explicitly illustrative (''Example of one of OAuth 2.0 authorization\n  flow''): the one scope, https://opendirect.example.com/scope/example, is a placeholder. OpenDirect leaves the\n  OAuth authorization server and scopes to each implementing seller, so no real scope catalog exists to search for;\n  the seller-agent reference implementation\
  \ uses static API keys with buyer/operator roles instead (authentication/).'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iab-tech-lab/refs/heads/main/scopes/iab-tech-lab-scopes.yml
summary_line: 1 scope · implicit
tags:
- Company
- Advertising
- AdTech
- Standards
- Programmatic
- Real-Time Bidding
- Consent
- Privacy
- Video Ads
- Agentic Advertising
- Non-Profit
token_urls: []
---
