---
api_specs:
- filename: tradingview-account-api-openapi.yml
  format: yaml
  label: TradingView Account API
  slug: tradingview-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-account-api-openapi.yml
- filename: tradingview-authorization-api-openapi.yml
  format: yaml
  label: TradingView Authorization API
  slug: tradingview-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-authorization-api-openapi.yml
- filename: tradingview-broker-configuration-api-openapi.yml
  format: yaml
  label: TradingView Broker Configuration API
  slug: tradingview-broker-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-broker-configuration-api-openapi.yml
- filename: tradingview-data-integration-api-openapi.yml
  format: yaml
  label: TradingView Data Integration API
  slug: tradingview-data-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-integration-api-openapi.yml
- filename: tradingview-data-permissions-api-openapi.yml
  format: yaml
  label: TradingView Data Permissions API
  slug: tradingview-data-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-data-permissions-api-openapi.yml
- filename: tradingview-market-data-api-openapi.yml
  format: yaml
  label: TradingView Market Data API
  slug: tradingview-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-market-data-api-openapi.yml
- filename: tradingview-trading-api-openapi.yml
  format: yaml
  label: TradingView Trading API
  slug: tradingview-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradingview/openapi/tradingview-trading-api-openapi.yml
authorization_urls:
- https://your-rest-implementation.com/api/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tradingview Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TradingView publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the TradingView API on a user''s behalf.


  Tokens are issued from https://your-rest-implementation.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TradingView
provider_slug: tradingview
schemes:
- description: 'TradingView supports OAuth 2 Authorization Code flow (standard) and OAuth 2 Authorization Code flow with PKCE, as described in [RFC 6749](https://tools.ietf.org/html/rfc6749) and [RFC 7636](https://tools.ietf.org/html/rfc7636), respectively.

    After performing authorization, the access token is sent with every request in the `Authorization` header.


    **Code Flow:**


    For OAuth 2 Code Flow the broker provides TradingView with the following OAuth 2 application parameters:


    Application parameter | Description | Example value

    ----------------------|-------------|----------------------------------------

    client id             | A unique client identifier | sQeww4FgtythHTUrhrfMo9rRTq |

    client secret         | A client secret | 45dd67oi56ds678st6788dffdyu |

    authorization URI     | An authorization endpoint URI |https://your-rest-implementation.com/oauth/authorize |

    token URI             | A token endpoint URI | https://your-rest-implementation.com/oauth/token |

    logout URI (optional) | A logout URI | https://your-rest-implementation.com/oauth/logout |

    scope                 | A scope of the access request as a list of space-delimited, case-sensitive strings | read trade profile |


    TradingView provides the broker with two redirect URIs, one for the staging environment and the other for the production environment.


    TradingView also provides a `redirect_uri` URI if the broker supports user logout with a redirect.


    **Note**: The `redirect_uri` parameter should be verified by the broker''s OAuth service, and should be whitelisted on the broker''s side.


    **PKCE:**


    TradingView supports OAuth 2 Authorization Code Flow with PKCE as an extension of the standard Code Flow.


    In the Authorization Code flow with PKCE, TradingView binds the authorization request and the token request using a one-time secret (`code_verifier`).

    The following parameters are added:

    - Authorization Request: `code_challenge`, `code_challenge_method`

    - Token Request: `code_verifier`


    When PKCE is not used, PKCE-only parameters must be omitted.


    *Authorization Request*


    TradingView sends the Authorization Request according to [OAuth 2 specification, 4.1.1](https://tools.ietf.org/html/rfc6749#section-4.1.1)

    and [Proof Key for Code Exchange by OAuth Public Clients, 4.3](https://datatracker.ietf.org/doc/html/rfc7636#section-4.3).

    The following parameters will be in the query part of the authorization URI:


    OAuth2 parameter | Description

    -----------------|------------

    response_type    | Response type. The value will be set to `code` |

    client_id        | A client identifier string provided by the broker |

    redirect_uri     | [Redirection Endpoint](https://tools.ietf.org/html/rfc6749#section-3.1.2) |

    scope            | A scope of the access request if it is provided by the broker |

    code_challenge   | (PKCE only) PKCE code challenge derived from `code_verifier` |

    code_challenge_method | (PKCE only) PKCE challenge method. TradingView uses `S256` |

    state            | [A literal string](https://tools.ietf.org/html/rfc6749#section-4.1.1) that the broker should return back to TradingView without changes in the authorization response


    **Note**: The `redirect_uri` parameter should be verified by the broker''s OAuth service, and should be whitelisted on the broker''s service.


    TradingView could send the `lang` parameter additionally if it is required by the broker, with the following possible values:

    `ar`, `br`, `de`, `en`, `es`, `fr`, `he` ,`hu`, `id`, `in`, `it`, `ja`, `kr`, `ms`, `pl`, `ru`, `th`, `tr`, `uk`, `vi`, `zh`.


    If all the parameters of the authorization request are valid and access is granted, the broker issues an authorization code and redirects to the redirect URI

    with the following parameters added to the request URI component:


    OAuth2 parameter | Description

    -----------------|------------

    code  | The authorization code. It must expire shortly after its release to prevent the risk of leakage |

    state | The exact value which was sent in the authorization request |


    *Access Token Request*


    TradingView makes an Access Token Request by sending the following parameters using the `application/x-www-form-urlencoded` format:


    OAuth2 parameter | Description

    -----------------|------------

    grant_type       | The grant type. The value will be set to `authorization_code` |

    client_id        | A client identifier string provided by the broker |

    client_secret    | A client secret string provided by the broker |

    code             | The authorization code received from the broker |

    redirect_uri     | The same redirect URI used in the Authorization Request |

    code_verifier    | (PKCE only) PKCE code verifier used to validate `code_challenge` |


    After successful verification of the authorization code broker issues an access token,

    a refresh token and responds to the access token request as follows:


    OAuth2 parameter         | Description

    -------------------------|------------

    access_token             | The access token which will be used in every request to the API |

    refresh_token            | Token used to obtain new access tokens |

    token_type               | Token type. Should be set to `bearer` |

    expires_in               | The life time of the access token in seconds |

    refresh_token_expires_in | The life time of the refresh token in seconds |


    The `expires_in` and `refresh_token_expires_in` parameters are optional, but are recommended to provide

    a more secure environment for integration users.


    *Refresh Request*


    To refresh the access token TradingView makes a Refresh Request to the token endpoint using the `application/x-www-form-urlencoded` format with the following parameters:


    OAuth2 parameter | Description

    -----------------|------------

    grant_type       | The grant type. The value will be set to `refresh_token` |

    refresh_token    | The refresh token issued by the broker |

    client_secret    | The client secret value provided by the broker |


    If all parameters are valid, the broker issues a new access token and, if necessary,

    a new refresh token and responds to the request as described in the *Access token request* section above.


    *Logout Request*


    To log the user out of the integration, TradingView makes a Logout Request to the logout endpoint with the following query string parameters:


    OAuth2 parameter | Description | Example

    -----------------|-------------|----------

    client_id        | A client identifier string provided by the broker |

    redirect_uri     | The url where the user should be redirected to after logging out | https://www.tradingview.com/trading/logout-redirect/'
  flows:
  - authorizationUrl: https://your-rest-implementation.com/api/authorize
    flow: authorizationCode
    tokenUrl: https://your-rest-implementation.com/api/oauth/token
  name: OAuth2Bearer
  source: openapi/tradingview-broker-rest-api-openapi.yml
- description: "This authentication flow is used for server-to-server requests where authentication needs to be done without human intervention.\nIt can be used with the [/history](#operation/getHistory), [/symbol_info](#operation/getSymbolInfo), [/streaming](#operation/streaming)\nand [/groups](#operation/getGroups) endpoints.\n\nJSON Web Token (JWT) is used to securely transmit information between broker and TradingView.\nMore information about JWT can be found [here](https://jwt.io/introduction/).\n\n### Application and OAuth2 parameters\n\nThe broker provides the following application and OAuth2 parameters to TradingView:\n\nApplication parameter | Description | Example value\n-----------------|-------------|---------------\nAppUrl | A URL uniquely representing broker's application | https://your-rest-implementation.com\nUserId | A user identifier for which the access token will be issued | testuser1\n\nOAuth2 parameter | Description | Example value\n-----------------|-------------|---------------\n\
    client_id | A unique client Identifier | FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5 |\nclient_secret | Secret code | adfegywrtyw |\ntoken_url | An url to which the access token request will be sent | https://your-rest-implementation.com/authorize/token\ngrant_type | Indicates the type of grant being presented in exchange for an access token  | urn:your-broker:oauth:grant-type:personal-jwt\n\n### X.509 Certificate\nThe broker provides a valid X.509 certificate to TradingView for signing JWT.\n\n\n### JSON Web Token\nJWT for the access token request is created with the following headers and claims:\n\nHeader | Description | Standard | Sample Value\n-------|-----------|------------|---------------\nx5t | Thumbprint of provided X.509 certificate used for signing JWT | [RFC 7515](https://tools.ietf.org/html/rfc7515#section-4.1.7) | 935093f1690900asdfd98626dfw35fa22b41d9dfd\nalg | Algorithm used to sign JWT. RS256 is only supported at the moment | [RFC 1518](https://tools.ietf.org/html/rfc7518#page-6)\
    \ | RS256\n\nClaim | Description | Sample Value\n------|-------------|-------------\niss | Issuer - Value should be client_id | FGGH7-TRVC3-ECDD2-CDHRG3\nsub | UserId - Value should be the UserId for which token is needed | testuser1\nexp | Expiry - Value should be a Unix time stamp indicating expiry of the token | 1549465914\naud | Audience - Value should be the token_url | https://your-rest-implementation.com/authorize/token\nspurl | AppUrl - The AppUrl of your application | https://your-rest-implementation.com\n\n### Requesting the access token\nTradingView sends a POST request to the `token_url` to obtain an access token.\nThe `client_id` and `client_secret` are included as parameters in the request body.\nThe JWT is sent in a parameter named `assertion`.\n\n#### Example Access Token request\n\n    POST /token HTTP/1.1\n    Host: sim.logonvalidation.net\n    Content-Type: application/x-www-form-urlencoded\n\n    grant_type=urn%3Ayour-broker%3Aoauth%3Agrant-type%3Apersonal-jwt\n \
    \   &assertion=eyJhbGciOiJFUzI1NiIsImtpZCI6IjE2In0.eyJpc3Mi[...omitted for brevity...]\n    &client_id=1234-5678-9101\n    &client_secret=abcdefghijklmn\n\nThe response to this request should contain an `access_token`. A `refresh_token` is optional and can be omitted:\n\n#### Example Access Token response\n    {\n      \"access_token\" : \"eyJhbfGujudUf.eyJvYWEiOiIw[omitted for brevity]\",\n      \"expires_in\": 1200,\n      \"token_type\": \"Bearer\",\n      \"refresh_token\": \"86fy7fa3d2-5e13-4736-86031-9ehiyiufrow0b\",\n      \"refresh_token_expires_in\": 2400\n    }"
  flows:
  - flow: clientCredentials
    tokenUrl: https://your-rest-implementation.com/api/authorize/token
  name: ServerOAuth2Bearer
  source: openapi/tradingview-broker-rest-api-openapi.yml
- description: "This authentication flow is used for server-to-server requests where\nauthentication needs to be done without human intervention.  It can be\nused with the [/history](#operation/getHistory),\n[/symbol_info](#operation/getSymbolInfo),\n[/streaming](#operation/streaming) and [/groups](#operation/getGroups)\nendpoints.\n\nJSON Web Token (JWT) is used to securely transmit information between\nbroker and TradingView.  More information about JWT can be found\n[here](https://jwt.io/introduction/).\n\nThis flow is described in Section 2.2 of\n[RFC 7523](https://datatracker.ietf.org/doc/html/rfc7523#section-2.2).\n\n### Application and OAuth2 parameters\n\nThe broker provides the following application and OAuth2 parameters to\nTradingView:\n\nApplication parameter | Description                                                 | Example value\n----------------------|-------------------------------------------------------------|---------------\nAudience              | A URL uniquely\
    \ representing broker's application            | https://your-rest-implementation.com\nUserId                | A user identifier for which the access token will be issued | testuser1\n\nOAuth2 parameter | Description                                           | Example value\n-----------------|-------------------------------------------------------|---------------\nclient_id        | A unique client identifier                            | FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5\ntoken_url        | A URL to which the access token request will be sent  | https://your-rest-implementation.com/authorize/token\n\n### X.509 Certificate\n\nThe broker provides a valid X.509 certificate and RSA private key to\nTradingView for signing JWT.\n\n### JSON Web Token\n\nJWT for the access token request is created with the following headers\nand claims:\n\nHeader | Description                                                       | Standard                                                  |Sample Value\n-------|-------------------------------------------------------------------|-----------------------------------------------------------|--------------\n\
    x5t    | Thumbprint of X.509 certificate used for signing JWT              | [RFC 7515](https://datatracker.ietf.org/doc/html/rfc7515) | 8e098221574da76cb97db539f69ae09d3c770ba9\nalg    | Algorithm used to sign JWT. RS256 is only supported at the moment | [RFC 7518](https://datatracker.ietf.org/doc/html/rfc7518) | RS256\n\nClaim | Description                                                               | Sample Value\n------|---------------------------------------------------------------------------|-------------\niss   | Issuer - Value should be client_id                                        | FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5\nsub   | UserId - Value should be the UserId for which token is needed             | testuser1\nexp   | Expiry - Value should be a Unix time stamp indicating expiry of the token | 1745166000\naud   | Audience - Value should be the token_url                                  | https://your-rest-implementation.com/authorize/token\njti   | JWT ID - An identifier\
    \ for the token, must be unique per request          | 7061d388-a4c0-4cd6-89f7-919567e38cfb\n\n### Requesting the access token\n\nTradingView sends a POST request to the `token_url` to obtain an access\ntoken.  The `client_id` and `audience` are included as parameters in the\nrequest body.  The JWT is sent in a parameter named `client_assertion`.\n\n#### Example Access Token request\n\n    POST /api/authorize/token HTTP/1.1\n    Host: your-rest-implementation.com\n    Content-Type: application/x-www-form-urlencoded\n\n    grant_type=client_credentials\n    &client_id=FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5\n    &client_assertion=eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOi[...omitted for brevity...]\n    &client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n    &audience=https://your-rest-implementation.com\n\nThe response to this request should contain an `access_token`.\n\n#### Example Access Token response\n\n    {\n      \"access_token\" : \"eyJhbfGujudUf.eyJvYWEiOiIw[...omitted\
    \ for brevity...]\",\n      \"token_type\": \"Bearer\",\n      \"expires_in\": 1200\n    }"
  flows:
  - flow: clientCredentials
    tokenUrl: https://your-rest-implementation.com/api/authorize/token
  name: ServerOAuth2JWT
  source: openapi/tradingview-broker-rest-api-openapi.yml
scope_count: 1
scope_names:
- general
scopes:
- description: permission to perform all requests
  flows:
  - authorizationCode
  - clientCredentials
  scope: general
slug: tradingview-scopes
source_filename: tradingview-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/tradingview-broker-rest-api-openapi.yml\nschemes:\n- name: OAuth2Bearer\n  source: openapi/tradingview-broker-rest-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-rest-implementation.com/api/authorize\n    tokenUrl: https://your-rest-implementation.com/api/oauth/token\n  description: |-\n    TradingView supports OAuth 2 Authorization Code flow (standard) and OAuth 2 Authorization Code flow with PKCE, as described in [RFC 6749](https://tools.ietf.org/html/rfc6749) and [RFC 7636](https://tools.ietf.org/html/rfc7636), respectively.\n    After performing authorization, the access token is sent with every request in the `Authorization` header.\n\n    **Code Flow:**\n\n    For OAuth 2 Code Flow the broker provides TradingView with the following OAuth 2 application parameters:\n\n    Application parameter | Description | Example value\n    ----------------------|-------------|----------------------------------------\n\
  \    client id             | A unique client identifier | sQeww4FgtythHTUrhrfMo9rRTq |\n    client secret         | A client secret | 45dd67oi56ds678st6788dffdyu |\n    authorization URI     | An authorization endpoint URI |https://your-rest-implementation.com/oauth/authorize |\n    token URI             | A token endpoint URI | https://your-rest-implementation.com/oauth/token |\n    logout URI (optional) | A logout URI | https://your-rest-implementation.com/oauth/logout |\n    scope                 | A scope of the access request as a list of space-delimited, case-sensitive strings | read trade profile |\n\n    TradingView provides the broker with two redirect URIs, one for the staging environment and the other for the production environment.\n\n    TradingView also provides a `redirect_uri` URI if the broker supports user logout with a redirect.\n\n    **Note**: The `redirect_uri` parameter should be verified by the broker's OAuth service, and should be whitelisted on the broker's side.\n\
  \n    **PKCE:**\n\n    TradingView supports OAuth 2 Authorization Code Flow with PKCE as an extension of the standard Code Flow.\n\n    In the Authorization Code flow with PKCE, TradingView binds the authorization request and the token request using a one-time secret (`code_verifier`).\n    The following parameters are added:\n    - Authorization Request: `code_challenge`, `code_challenge_method`\n    - Token Request: `code_verifier`\n\n    When PKCE is not used, PKCE-only parameters must be omitted.\n\n    *Authorization Request*\n\n    TradingView sends the Authorization Request according to [OAuth 2 specification, 4.1.1](https://tools.ietf.org/html/rfc6749#section-4.1.1)\n    and [Proof Key for Code Exchange by OAuth Public Clients, 4.3](https://datatracker.ietf.org/doc/html/rfc7636#section-4.3).\n    The following parameters will be in the query part of the authorization URI:\n\n    OAuth2 parameter | Description\n    -----------------|------------\n    response_type    | Response\
  \ type. The value will be set to `code` |\n    client_id        | A client identifier string provided by the broker |\n    redirect_uri     | [Redirection Endpoint](https://tools.ietf.org/html/rfc6749#section-3.1.2) |\n    scope            | A scope of the access request if it is provided by the broker |\n    code_challenge   | (PKCE only) PKCE code challenge derived from `code_verifier` |\n    code_challenge_method | (PKCE only) PKCE challenge method. TradingView uses `S256` |\n    state            | [A literal string](https://tools.ietf.org/html/rfc6749#section-4.1.1) that the broker should return back to TradingView without changes in the authorization response\n\n    **Note**: The `redirect_uri` parameter should be verified by the broker's OAuth service, and should be whitelisted on the broker's service.\n\n    TradingView could send the `lang` parameter additionally if it is required by the broker, with the following possible values:\n    `ar`, `br`, `de`, `en`, `es`, `fr`, `he` ,`hu`,\
  \ `id`, `in`, `it`, `ja`, `kr`, `ms`, `pl`, `ru`, `th`, `tr`, `uk`, `vi`, `zh`.\n\n    If all the parameters of the authorization request are valid and access is granted, the broker issues an authorization code and redirects to the redirect URI\n    with the following parameters added to the request URI component:\n\n    OAuth2 parameter | Description\n    -----------------|------------\n    code  | The authorization code. It must expire shortly after its release to prevent the risk of leakage |\n    state | The exact value which was sent in the authorization request |\n\n    *Access Token Request*\n\n    TradingView makes an Access Token Request by sending the following parameters using the `application/x-www-form-urlencoded` format:\n\n    OAuth2 parameter | Description\n    -----------------|------------\n    grant_type       | The grant type. The value will be set to `authorization_code` |\n    client_id        | A client identifier string provided by the broker |\n    client_secret\
  \    | A client secret string provided by the broker |\n    code             | The authorization code received from the broker |\n    redirect_uri     | The same redirect URI used in the Authorization Request |\n    code_verifier    | (PKCE only) PKCE code verifier used to validate `code_challenge` |\n\n    After successful verification of the authorization code broker issues an access token,\n    a refresh token and responds to the access token request as follows:\n\n    OAuth2 parameter         | Description\n    -------------------------|------------\n    access_token             | The access token which will be used in every request to the API |\n    refresh_token            | Token used to obtain new access tokens |\n    token_type               | Token type. Should be set to `bearer` |\n    expires_in               | The life time of the access token in seconds |\n    refresh_token_expires_in | The life time of the refresh token in seconds |\n\n    The `expires_in` and `refresh_token_expires_in`\
  \ parameters are optional, but are recommended to provide\n    a more secure environment for integration users.\n\n    *Refresh Request*\n\n    To refresh the access token TradingView makes a Refresh Request to the token endpoint using the `application/x-www-form-urlencoded` format with the following parameters:\n\n    OAuth2 parameter | Description\n    -----------------|------------\n    grant_type       | The grant type. The value will be set to `refresh_token` |\n    refresh_token    | The refresh token issued by the broker |\n    client_secret    | The client secret value provided by the broker |\n\n    If all parameters are valid, the broker issues a new access token and, if necessary,\n    a new refresh token and responds to the request as described in the *Access token request* section above.\n\n    *Logout Request*\n\n    To log the user out of the integration, TradingView makes a Logout Request to the logout endpoint with the following query string parameters:\n\n    OAuth2 parameter\
  \ | Description | Example\n    -----------------|-------------|----------\n    client_id        | A client identifier string provided by the broker |\n    redirect_uri     | The url where the user should be redirected to after logging out | https://www.tradingview.com/trading/logout-redirect/\n- name: ServerOAuth2Bearer\n  source: openapi/tradingview-broker-rest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-rest-implementation.com/api/authorize/token\n  description: |-\n    This authentication flow is used for server-to-server requests where authentication needs to be done without human intervention.\n    It can be used with the [/history](#operation/getHistory), [/symbol_info](#operation/getSymbolInfo), [/streaming](#operation/streaming)\n    and [/groups](#operation/getGroups) endpoints.\n\n    JSON Web Token (JWT) is used to securely transmit information between broker and TradingView.\n    More information about JWT can be found [here](https://jwt.io/introduction/).\n\
  \n    ### Application and OAuth2 parameters\n\n    The broker provides the following application and OAuth2 parameters to TradingView:\n\n    Application parameter | Description | Example value\n    -----------------|-------------|---------------\n    AppUrl | A URL uniquely representing broker's application | https://your-rest-implementation.com\n    UserId | A user identifier for which the access token will be issued | testuser1\n\n    OAuth2 parameter | Description | Example value\n    -----------------|-------------|---------------\n    client_id | A unique client Identifier | FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5 |\n    client_secret | Secret code | adfegywrtyw |\n    token_url | An url to which the access token request will be sent | https://your-rest-implementation.com/authorize/token\n    grant_type | Indicates the type of grant being presented in exchange for an access token  | urn:your-broker:oauth:grant-type:personal-jwt\n\n    ### X.509 Certificate\n    The broker provides a valid\
  \ X.509 certificate to TradingView for signing JWT.\n\n\n    ### JSON Web Token\n    JWT for the access token request is created with the following headers and claims:\n\n    Header | Description | Standard | Sample Value\n    -------|-----------|------------|---------------\n    x5t | Thumbprint of provided X.509 certificate used for signing JWT | [RFC 7515](https://tools.ietf.org/html/rfc7515#section-4.1.7) | 935093f1690900asdfd98626dfw35fa22b41d9dfd\n    alg | Algorithm used to sign JWT. RS256 is only supported at the moment | [RFC 1518](https://tools.ietf.org/html/rfc7518#page-6) | RS256\n\n    Claim | Description | Sample Value\n    ------|-------------|-------------\n    iss | Issuer - Value should be client_id | FGGH7-TRVC3-ECDD2-CDHRG3\n    sub | UserId - Value should be the UserId for which token is needed | testuser1\n    exp | Expiry - Value should be a Unix time stamp indicating expiry of the token | 1549465914\n    aud | Audience - Value should be the token_url | https://your-rest-implementation.com/authorize/token\n\
  \    spurl | AppUrl - The AppUrl of your application | https://your-rest-implementation.com\n\n    ### Requesting the access token\n    TradingView sends a POST request to the `token_url` to obtain an access token.\n    The `client_id` and `client_secret` are included as parameters in the request body.\n    The JWT is sent in a parameter named `assertion`.\n\n    #### Example Access Token request\n\n        POST /token HTTP/1.1\n        Host: sim.logonvalidation.net\n        Content-Type: application/x-www-form-urlencoded\n\n        grant_type=urn%3Ayour-broker%3Aoauth%3Agrant-type%3Apersonal-jwt\n        &assertion=eyJhbGciOiJFUzI1NiIsImtpZCI6IjE2In0.eyJpc3Mi[...omitted for brevity...]\n        &client_id=1234-5678-9101\n        &client_secret=abcdefghijklmn\n\n    The response to this request should contain an `access_token`. A `refresh_token` is optional and can be omitted:\n\n    #### Example Access Token response\n        {\n          \"access_token\" : \"eyJhbfGujudUf.eyJvYWEiOiIw[omitted\
  \ for brevity]\",\n          \"expires_in\": 1200,\n          \"token_type\": \"Bearer\",\n          \"refresh_token\": \"86fy7fa3d2-5e13-4736-86031-9ehiyiufrow0b\",\n          \"refresh_token_expires_in\": 2400\n        }\n- name: ServerOAuth2JWT\n  source: openapi/tradingview-broker-rest-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-rest-implementation.com/api/authorize/token\n  description: |-\n    This authentication flow is used for server-to-server requests where\n    authentication needs to be done without human intervention.  It can be\n    used with the [/history](#operation/getHistory),\n    [/symbol_info](#operation/getSymbolInfo),\n    [/streaming](#operation/streaming) and [/groups](#operation/getGroups)\n    endpoints.\n\n    JSON Web Token (JWT) is used to securely transmit information between\n    broker and TradingView.  More information about JWT can be found\n    [here](https://jwt.io/introduction/).\n\n    This flow is described\
  \ in Section 2.2 of\n    [RFC 7523](https://datatracker.ietf.org/doc/html/rfc7523#section-2.2).\n\n    ### Application and OAuth2 parameters\n\n    The broker provides the following application and OAuth2 parameters to\n    TradingView:\n\n    Application parameter | Description                                                 | Example value\n    ----------------------|-------------------------------------------------------------|---------------\n    Audience              | A URL uniquely representing broker's application            | https://your-rest-implementation.com\n    UserId                | A user identifier for which the access token will be issued | testuser1\n\n    OAuth2 parameter | Description                                           | Example value\n    -----------------|-------------------------------------------------------|---------------\n    client_id        | A unique client identifier                            | FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5\n    token_url   \
  \     | A URL to which the access token request will be sent  | https://your-rest-implementation.com/authorize/token\n\n    ### X.509 Certificate\n\n    The broker provides a valid X.509 certificate and RSA private key to\n    TradingView for signing JWT.\n\n    ### JSON Web Token\n\n    JWT for the access token request is created with the following headers\n    and claims:\n\n    Header | Description                                                       | Standard                                                  |Sample Value\n    -------|-------------------------------------------------------------------|-----------------------------------------------------------|--------------\n    x5t    | Thumbprint of X.509 certificate used for signing JWT              | [RFC 7515](https://datatracker.ietf.org/doc/html/rfc7515) | 8e098221574da76cb97db539f69ae09d3c770ba9\n    alg    | Algorithm used to sign JWT. RS256 is only supported at the moment | [RFC 7518](https://datatracker.ietf.org/doc/html/rfc7518)\
  \ | RS256\n\n    Claim | Description                                                               | Sample Value\n    ------|---------------------------------------------------------------------------|-------------\n    iss   | Issuer - Value should be client_id                                        | FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5\n    sub   | UserId - Value should be the UserId for which token is needed             | testuser1\n    exp   | Expiry - Value should be a Unix time stamp indicating expiry of the token | 1745166000\n    aud   | Audience - Value should be the token_url                                  | https://your-rest-implementation.com/authorize/token\n    jti   | JWT ID - An identifier for the token, must be unique per request          | 7061d388-a4c0-4cd6-89f7-919567e38cfb\n\n    ### Requesting the access token\n\n    TradingView sends a POST request to the `token_url` to obtain an access\n    token.  The `client_id` and `audience` are included as parameters in the\n\
  \    request body.  The JWT is sent in a parameter named `client_assertion`.\n\n    #### Example Access Token request\n\n        POST /api/authorize/token HTTP/1.1\n        Host: your-rest-implementation.com\n        Content-Type: application/x-www-form-urlencoded\n\n        grant_type=client_credentials\n        &client_id=FGGH7-TRVC3-ECDD2-CDHRG3-FYUDG5\n        &client_assertion=eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOi[...omitted for brevity...]\n        &client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n        &audience=https://your-rest-implementation.com\n\n    The response to this request should contain an `access_token`.\n\n    #### Example Access Token response\n\n        {\n          \"access_token\" : \"eyJhbfGujudUf.eyJvYWEiOiIw[...omitted for brevity...]\",\n          \"token_type\": \"Bearer\",\n          \"expires_in\": 1200\n        }\nscopes:\n- scope: general\n  description: permission to perform all requests\n  flows:\n  - authorizationCode\n\
  \  - clientCredentials\n  sources:\n  - openapi/tradingview-broker-rest-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/tradingview/scopes/tradingview-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Consumer
- Charts
- Charting Library
- Financial Data
- Market Data
- Widgets
- Trading
- Fintech
- Embeddable Components
token_bound: false
token_urls:
- https://your-rest-implementation.com/api/oauth/token
- https://your-rest-implementation.com/api/authorize/token
---
