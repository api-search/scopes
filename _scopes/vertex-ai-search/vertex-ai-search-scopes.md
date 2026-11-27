---
api_specs:
- filename: vertex-ai-search-projects-api-openapi.yml
  format: yaml
  label: Discovery Engine API (Vertex AI Search) - Projects
  slug: vertex-ai-search-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex-ai-search/openapi/vertex-ai-search-projects-api-openapi.yml
- filename: vertex-ai-search-billingaccounts-api-openapi.yml
  format: yaml
  label: Vertex AI Search Billing Accounts API
  slug: vertex-ai-search-billingaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex-ai-search/openapi/vertex-ai-search-billingaccounts-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Vertex AI Search Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vertex AI Search publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vertex AI Search API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vertex AI Search
provider_slug: vertex-ai-search
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/vertex-ai-search-billing-accounts-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/vertex-ai-search-projects-api-openapi.yml
scope_count: 5
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud_search.query
- https://www.googleapis.com/auth/discoveryengine.assist.readwrite
- https://www.googleapis.com/auth/discoveryengine.readwrite
- https://www.googleapis.com/auth/discoveryengine.serving.readwrite
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: Search your organization's data in the Cloud Search index
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud_search.query
- description: View your Agentspace chat history, including uploaded files and generated reports and visualizations, and interact with the Agentspace assistant on your behalf. Also view the artifacts you access through NotebookLM Enterprise.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/discoveryengine.assist.readwrite
- description: View, edit, create, and delete all your data associated with any Discovery Engine API product, such as Agentspace, Vertex AI Search, or NotebookLM Enterprise, including both end user data and administration or configuration data.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/discoveryengine.readwrite
- description: Interact with Discovery Engine API products, such as Agentspace, Vertex AI Search, or NotebookLM Enterprise, on your behalf. It will also allow the app to view all data that you have access to when you use or interact with a Discovery Engine API product.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/discoveryengine.serving.readwrite
slug: vertex-ai-search-scopes
source_filename: vertex-ai-search-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/vertex-ai-search-billing-accounts-api-openapi.yml, openapi/vertex-ai-search-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/vertex-ai-search-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n\
  - scope: https://www.googleapis.com/auth/cloud_search.query\n  description: Search your organization's data in the Cloud Search index\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/discoveryengine.assist.readwrite\n  description: View your Agentspace chat history, including uploaded files and generated reports\n    and visualizations, and interact with the Agentspace assistant on your behalf. Also view\n    the artifacts you access through NotebookLM Enterprise.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/discoveryengine.readwrite\n  description: View, edit, create, and delete all your data associated with any Discovery Engine\n    API product, such as Agentspace, Vertex AI\
  \ Search, or NotebookLM Enterprise, including both\n    end user data and administration or configuration data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/discoveryengine.serving.readwrite\n  description: Interact with Discovery Engine API products, such as Agentspace, Vertex AI Search,\n    or NotebookLM Enterprise, on your behalf. It will also allow the app to view all data that\n    you have access to when you use or interact with a Discovery Engine API product.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/vertex-ai-search/scopes/vertex-ai-search-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Search
- Enterprise
- Google Cloud
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
