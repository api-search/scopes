---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Logto Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Logto publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Logto API on a user''s behalf.


  Tokens are issued from /oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Logto
provider_slug: logto
schemes:
- description: "Logto Management API is a comprehensive set of REST APIs that gives you the full control over Logto to suit your product needs and tech stack. To see the full guide on Management API interactions, visit [Interact with Management API](https://docs.logto.io/docs/recipes/interact-with-management-api/).\n\n### Get started\n\nThe API follows the same authentication principles as other API resources in Logto, with some slight differences. To use Logto Management API:\n\n1. A machine-to-machine (M2M) application needs to be created.\n2. A machine-to-machine (M2M) role with Management API permission `all` needs to be assigned to the application.\n\nOnce you have them set up, you can use the `client_credentials` grant type to fetch an access token and use it to authenticate your requests to the Logto Management API.\n\n### Fetch an access token\n\nTo fetch an access token, you need to make a `POST` request to the `/oidc/token` endpoint of your Logto tenant.\n\nFor Logto Cloud users,\
    \ the base URL is your Logto endpoint, i.e. `https://[tenant-id].logto.app`. The tenant ID can be found in the following places:\n\n- The first path segment of the URL when you are signed in to Logto Cloud. For example, if the URL is `https://cloud.logto.io/foo/get-started`, the tenant ID is `foo`.\n- In the \"Settings\" tab of Logto Cloud.\n\nThe request should follow the OAuth 2.0 [client credentials](https://datatracker.ietf.org/doc/html/rfc6749#section-4.4) grant type. Here is a non-normative example of how to fetch an access token:\n\n```bash\ncurl --location \\\n  --request POST 'https://[tenant-id].logto.app/oidc/token' \\\n  --header 'Content-Type: application/x-www-form-urlencoded' \\\n  --data-urlencode 'grant_type=client_credentials' \\\n  --data-urlencode 'client_id=[app-id]' \\\n  --data-urlencode 'client_secret=[app-secret]' \\\n  --data-urlencode 'resource=https://[tenant-id].logto.app/api' \\\n  --data-urlencode 'scope=all'\n```\n\nReplace `[tenant-id]`, `[app-id]`, and\
    \ `[app-secret]` with your Logto tenant ID, application ID, and application secret, respectively.\n\nThe response will be like:\n\n```json\n{\n  \"access_token\": \"eyJhbG...2g\", // Use this value for accessing the Logto Management API\n  \"expires_in\": 3600, // Token expiration in seconds\n  \"token_type\": \"Bearer\", // Token type for your request when using the access token\n  \"scope\": \"all\" // Scope `all` for Logto Management API\n}\n```\n\n### Use the access token\n\nOnce you have the access token, you can use it to authenticate your requests to the Logto Management API. The access token should be included in the `Authorization` header of your requests with the `Bearer` authentication scheme.\n\nHere is an example of how to list the first page of users in your Logto tenant:\n\n```bash\ncurl --location \\\n  --request GET 'https://[tenant-id].logto.app/api/users' \\\n  --header 'Authorization: Bearer eyJhbG...2g'\n```\n\nReplace `[tenant-id]` with your Logto tenant ID and\
    \ `eyJhbG...2g` with the access token you fetched earlier."
  flows:
  - flow: clientCredentials
    tokenUrl: /oidc/token
  name: OAuth2
  source: openapi/logto-openapi-original.yml
scope_count: 1
scope_names:
- all
scopes:
- description: All scopes
  flows:
  - clientCredentials
  scope: all
slug: logto-scopes
source_filename: logto-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/logto-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/logto-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oidc/token\n  description: |-\n    Logto Management API is a comprehensive set of REST APIs that gives you the full control over Logto to suit your product needs and tech stack. To see the full guide on Management API interactions, visit [Interact with Management API](https://docs.logto.io/docs/recipes/interact-with-management-api/).\n\n    ### Get started\n\n    The API follows the same authentication principles as other API resources in Logto, with some slight differences. To use Logto Management API:\n\n    1. A machine-to-machine (M2M) application needs to be created.\n    2. A machine-to-machine (M2M) role with Management API permission `all` needs to be assigned to the application.\n\n    Once you have them set up, you can use the `client_credentials` grant type\
  \ to fetch an access token and use it to authenticate your requests to the Logto Management API.\n\n    ### Fetch an access token\n\n    To fetch an access token, you need to make a `POST` request to the `/oidc/token` endpoint of your Logto tenant.\n\n    For Logto Cloud users, the base URL is your Logto endpoint, i.e. `https://[tenant-id].logto.app`. The tenant ID can be found in the following places:\n\n    - The first path segment of the URL when you are signed in to Logto Cloud. For example, if the URL is `https://cloud.logto.io/foo/get-started`, the tenant ID is `foo`.\n    - In the \"Settings\" tab of Logto Cloud.\n\n    The request should follow the OAuth 2.0 [client credentials](https://datatracker.ietf.org/doc/html/rfc6749#section-4.4) grant type. Here is a non-normative example of how to fetch an access token:\n\n    ```bash\n    curl --location \\\n      --request POST 'https://[tenant-id].logto.app/oidc/token' \\\n      --header 'Content-Type: application/x-www-form-urlencoded'\
  \ \\\n      --data-urlencode 'grant_type=client_credentials' \\\n      --data-urlencode 'client_id=[app-id]' \\\n      --data-urlencode 'client_secret=[app-secret]' \\\n      --data-urlencode 'resource=https://[tenant-id].logto.app/api' \\\n      --data-urlencode 'scope=all'\n    ```\n\n    Replace `[tenant-id]`, `[app-id]`, and `[app-secret]` with your Logto tenant ID, application ID, and application secret, respectively.\n\n    The response will be like:\n\n    ```json\n    {\n      \"access_token\": \"eyJhbG...2g\", // Use this value for accessing the Logto Management API\n      \"expires_in\": 3600, // Token expiration in seconds\n      \"token_type\": \"Bearer\", // Token type for your request when using the access token\n      \"scope\": \"all\" // Scope `all` for Logto Management API\n    }\n    ```\n\n    ### Use the access token\n\n    Once you have the access token, you can use it to authenticate your requests to the Logto Management API. The access token should be included in\
  \ the `Authorization` header of your requests with the `Bearer` authentication scheme.\n\n    Here is an example of how to list the first page of users in your Logto tenant:\n\n    ```bash\n    curl --location \\\n      --request GET 'https://[tenant-id].logto.app/api/users' \\\n      --header 'Authorization: Bearer eyJhbG...2g'\n    ```\n\n    Replace `[tenant-id]` with your Logto tenant ID and `eyJhbG...2g` with the access token you fetched earlier.\nscopes:\n- scope: all\n  description: All scopes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/logto-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logto/refs/heads/main/scopes/logto-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Authentication
- Authorization
- Identity
- OIDC
- OAuth
- SAML
- Open Source
token_urls:
- /oidc/token
---
