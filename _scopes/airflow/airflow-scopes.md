---
api_specs:
- filename: airflow-openapi.yml
  format: yaml
  label: Apache Airflow API
  slug: airflow
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/openapi/airflow-openapi.yml
authorization_urls: []
description: ''
docs: https://airflow.apache.org/docs/apache-airflow/stable/security/api.html
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Airflow Scopes
name_suffix: OAuth Scopes
note: Apache Airflow does not publish OAuth scopes; the REST API authenticates with JWT tokens from POST /auth/token and authorization is handled by the configured auth manager's roles and permissions rather than OAuth scopes (see https://airflow.apache.org/docs/apache-airflow/stable/security/api.html).
overview: 'Apache Airflow uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Apache Airflow
provider_slug: airflow
schemes:
- description: To authenticate Airflow API requests, clients must include a JWT (JSON Web Token) in the Authorization header of each request. This token is used to verify the identity of the client and ensure that they have the appropriate permissions to access the requested resources. You can use the endpoint ``POST /auth/token`` in order to generate a JWT token. Upon successful authentication, the server will issue a JWT token that contains the necessary information (such as user identity and scope) to authenticate subsequent requests. To learn more about Airflow public API authentication, please read https://airflow.apache.org/docs/apache-airflow/stable/security/api.html.
  flows:
  - flow: password
    tokenUrl: /auth/token
  name: OAuth2PasswordBearer
  source: openapi/airflow-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: airflow-scopes
source_filename: airflow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airflow-openapi.yml\ndocs: https://airflow.apache.org/docs/apache-airflow/stable/security/api.html\nnote: Apache Airflow does not publish OAuth scopes; the REST API authenticates with\n  JWT tokens from POST /auth/token and authorization is handled by the configured\n  auth manager's roles and permissions rather than OAuth scopes (see\n  https://airflow.apache.org/docs/apache-airflow/stable/security/api.html).\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/airflow-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/token\n  description: To authenticate Airflow API requests, clients must include a JWT (JSON Web Token)\n    in the Authorization header of each request. This token is used to verify the identity of\n    the client and ensure that they have the appropriate permissions to access the requested\n    resources. You can use the endpoint ``POST /auth/token`` in order to generate a JWT token.\n\
  \    Upon successful authentication, the server will issue a JWT token that contains the necessary\n    information (such as user identity and scope) to authenticate subsequent requests. To learn\n    more about Airflow public API authentication, please read https://airflow.apache.org/docs/apache-airflow/stable/security/api.html.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/scopes/airflow-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
token_urls:
- /auth/token
---
