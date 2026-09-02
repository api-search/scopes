---
api_specs:
- filename: shanghai-jiao-tong-university-open-api-openapi.yml
  format: yaml
  label: SJTU Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shanghai-jiao-tong-university/refs/heads/main/openapi/shanghai-jiao-tong-university-open-api-openapi.yml
- filename: shanghai-jiao-tong-university-data-resources-openapi.yml
  format: yaml
  label: SJTU Data Resources API
  slug: data-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shanghai-jiao-tong-university/refs/heads/main/openapi/shanghai-jiao-tong-university-data-resources-openapi.yml
authorization_urls:
- https://jaccount.sjtu.edu.cn/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: searched
name: Shanghai Jiao Tong University Scopes
name_suffix: OAuth Scopes
note: 'The complete OAuth 2.0 authorization-scope registry SJTU publishes for its own jAccount authorization server. The scope strings, the bit values and the supported grants are the university''s, read verbatim from the 授权范围列表 table on its developer portal; the English descriptions are ours, translated from the Chinese in the same table. Two things are worth reading off this list. First, it is a bitmask registry — every scope has a value of the form 1<<n and the portal documents that a caller may request multiple scopes either as a space-separated string or as the SUM of the values (scope=basic essential is equivalent to scope=3). That is an unusual, pre-OAuth-2.1 design and it is stated openly. Second, the gaps in the bit sequence (there is no 1<<4, 1<<13..16, 1<<18..19, 1<<21..22, 1<<24, 1<<28, 1<<31..33) are retired or internal scopes; only the 39 published here are documented. Note the mismatch with discovery: the OIDC metadata at https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration
  advertises scopes_supported as [openid, basic] only. An agent reading discovery alone sees 2 scopes; the documentation publishes 39.'
overview: 'Shanghai Jiao Tong University publishes 40 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shanghai Jiao Tong University API on a user''s behalf.


  Tokens are issued from https://jaccount.sjtu.edu.cn/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shanghai Jiao Tong University
provider_slug: shanghai-jiao-tong-university
schemes:
- combination: Space-separated scope names, or the arithmetic sum of the bit values.
  flows:
  - authorizationUrl: https://jaccount.sjtu.edu.cn/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token
  - flow: password
    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token
  issuer: https://jaccount.sjtu.edu.cn/oauth2/
  name: jAccountOAuth2
  source: https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration
scope_count: 40
scope_names:
- openid
- basic
- essential
- profile
- unicode
- tasks
- messages
- notifications
- privacy
- introspect
- read_apps
- write_apps
- exchange_data
- signature
- manage_card
- send_app_notification
- send_notification
- read_mails
- send_mail
- storage
- modify_notification
- lessons
- classes
- exams
- scores
- students_list
- card_info
- card_transactions
- write_card_info
- income
- create_jaccount
- edit_jaccount
- net_service_info
- connect_wechat
- connect_shmec
- print
- connect_finance
- student_affairs
- bus
- calendar
scopes:
- description: Standard OpenID Connect scope — requests an ID token for the signed-in user. Advertised in the discovery document but absent from the portal's 授权范围列表 table.
  flows:
  - authorizationCode
  scope: openid
- description: Read the user's identifier (system id and jAccount name) and real name.
  flows:
  - authorizationCode
  - clientCredentials
  scope: basic
- description: Read basic identifier and name plus the bound identity (identity id, identity type, and owning department/school).
  flows:
  - authorizationCode
  - clientCredentials
  scope: essential
- description: Read fuller user detail — basic identifier, name, account information, mobile number, usual email address.
  flows:
  - authorizationCode
  - clientCredentials
  scope: profile
- description: Activate, retrieve or validate the Siyuan code (思源码).
  flows:
  - authorizationCode
  - clientCredentials
  scope: unicode
- description: Read actionable/pending/in-progress/completed task lists; read or aggregate manageable workflows, instances and tasks.
  flows:
  - authorizationCode
  - clientCredentials
  scope: tasks
- description: Read the user's messages.
  flows:
  - clientCredentials
  scope: messages
- description: Read the user's system notifications.
  flows:
  - authorizationCode
  scope: notifications
- description: Read the user's detailed information, including personal ID-document details and date of birth.
  flows:
  - authorizationCode
  scope: privacy
- description: Introspect an OAuth token. API-development use only.
  flows:
  - clientCredentials
  scope: introspect
- description: Read application registration information.
  flows:
  - clientCredentials
  scope: read_apps
- description: Create and modify application registration information.
  flows:
  - clientCredentials
  scope: write_apps
- description: Data exchange — the scope the Data Resources APIs on graphql.sjtu.edu.cn require.
  flows:
  - clientCredentials
  scope: exchange_data
- description: Obtain a digital signature.
  flows:
  - authorizationCode
  - clientCredentials
  scope: signature
- description: Campus-card management, such as account opening.
  flows:
  - authorizationCode
  scope: manage_card
- description: Send a Jiao-Wo-Ban (交我办) app notification to a user.
  flows:
  - clientCredentials
  scope: send_app_notification
- description: Send a notification to a user.
  flows:
  - password
  scope: send_notification
- description: Read the user's mail.
  flows:
  - authorizationCode
  scope: read_mails
- description: Send mail on the user's behalf, or change a message's read state.
  flows:
  - authorizationCode
  - password
  scope: send_mail
- description: Full control of the application's own unstructured storage.
  flows:
  - clientCredentials
  - password
  scope: storage
- description: Modify the state of the application's own notifications.
  flows:
  - authorizationCode
  scope: modify_notification
- description: Read the user's lesson information.
  flows:
  - authorizationCode
  scope: lessons
- description: Read the user's timetable (including courses).
  flows:
  - authorizationCode
  scope: classes
- description: Read the user's examination information.
  flows:
  - authorizationCode
  scope: exams
- description: Read the user's examination results.
  flows:
  - authorizationCode
  scope: scores
- description: Read the enrolled-student roster for a class (teacher).
  flows:
  - authorizationCode
  scope: students_list
- description: Read the user's campus-card information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: card_info
- description: Read the user's campus-card transaction records.
  flows:
  - authorizationCode
  scope: card_transactions
- description: Campus-card write operations — change the query password, report a card lost, top up from a bound bank card.
  flows:
  - authorizationCode
  scope: write_card_info
- description: Query the user's income information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: income
- description: Create a jAccount account.
  flows:
  - clientCredentials
  scope: create_jaccount
- description: Modify a jAccount account.
  flows:
  - authorizationCode
  scope: edit_jaccount
- description: Read all personal network-service information for a specified user.
  flows:
  - authorizationCode
  scope: net_service_info
- description: Bind a jAccount to a WeChat account.
  flows:
  - authorizationCode
  scope: connect_wechat
- description: Bind a jAccount to a Shanghai Municipal Education Commission account.
  flows:
  - authorizationCode
  scope: connect_shmec
- description: Self-service printing.
  flows:
  - authorizationCode
  - clientCredentials
  scope: print
- description: Integrate with the finance appointment system.
  flows:
  - clientCredentials
  scope: connect_finance
- description: Retrieve student-affairs information.
  flows:
  - clientCredentials
  scope: student_affairs
- description: Read campus-bus and inter-campus shuttle timetables and real-time information.
  flows:
  - clientCredentials
  scope: bus
- description: Synchronise calendar information.
  flows:
  - authorizationCode
  - clientCredentials
  scope: calendar
slug: shanghai-jiao-tong-university-scopes
source_filename: shanghai-jiao-tong-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://developer.sjtu.edu.cn/auth/oauth.html#授权范围\nx-operator: institution\nnote: 'The complete OAuth 2.0 authorization-scope registry SJTU publishes for its own jAccount authorization\n  server. The scope strings, the bit values and the supported grants are the university''s, read verbatim\n  from the 授权范围列表 table on its developer portal; the English descriptions are ours, translated from\n  the Chinese in the same table.\n\n\n  Two things are worth reading off this list. First, it is a bitmask registry — every scope has a value\n  of the form 1<<n and the portal documents that a caller may request multiple scopes either as a space-separated\n  string or as the SUM of the values (scope=basic essential is equivalent to scope=3). That is an unusual,\n  pre-OAuth-2.1 design and it is stated openly. Second, the gaps in the bit sequence (there is no 1<<4,\n  1<<13..16, 1<<18..19, 1<<21..22, 1<<24, 1<<28, 1<<31..33) are retired\
  \ or internal scopes; only the\n  39 published here are documented.\n\n\n  Note the mismatch with discovery: the OIDC metadata at https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration\n  advertises scopes_supported as [openid, basic] only. An agent reading discovery alone sees 2 scopes;\n  the documentation publishes 39.'\nschemes:\n- name: jAccountOAuth2\n  source: https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration\n  issuer: https://jaccount.sjtu.edu.cn/oauth2/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://jaccount.sjtu.edu.cn/oauth2/authorize\n    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token\n  - flow: password\n    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token\n  combination: Space-separated scope names, or the arithmetic sum of the bit values.\nscopes:\n- scope: openid\n  value: null\n  description: Standard OpenID Connect scope\
  \ — requests an ID token for the signed-in user. Advertised\n    in the discovery document but absent from the portal's 授权范围列表 table.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/shanghai-jiao-tong-university-openid-configuration.json\n- scope: basic\n  value: 1<<0\n  description: Read the user's identifier (system id and jAccount name) and real name.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: essential\n  value: 1<<1\n  description: Read basic identifier and name plus the bound identity (identity id, identity type, and\n    owning department/school).\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: profile\n  value: 1<<2\n  description: Read fuller user detail — basic identifier, name, account information, mobile number,\n    usual email address.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n\
  \  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: unicode\n  value: 1<<3\n  description: Activate, retrieve or validate the Siyuan code (思源码).\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: tasks\n  value: 1<<5\n  description: Read actionable/pending/in-progress/completed task lists; read or aggregate manageable\n    workflows, instances and tasks.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: messages\n  value: 1<<6\n  description: Read the user's messages.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: notifications\n  value: 1<<7\n  description: Read the user's system notifications.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: privacy\n  value: 1<<8\n  description: Read the user's detailed information,\
  \ including personal ID-document details and date\n    of birth.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: introspect\n  value: 1<<9\n  description: Introspect an OAuth token. API-development use only.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: read_apps\n  value: 1<<10\n  description: Read application registration information.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: write_apps\n  value: 1<<11\n  description: Create and modify application registration information.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: exchange_data\n  value: 1<<12\n  description: Data exchange — the scope the Data Resources APIs on graphql.sjtu.edu.cn require.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope:\
  \ signature\n  value: 1<<17\n  description: Obtain a digital signature.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: manage_card\n  value: 1<<20\n  description: Campus-card management, such as account opening.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: send_app_notification\n  value: 1<<23\n  description: Send a Jiao-Wo-Ban (交我办) app notification to a user.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: send_notification\n  value: 1<<25\n  description: Send a notification to a user.\n  flows:\n  - password\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: read_mails\n  value: 1<<26\n  description: Read the user's mail.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: send_mail\n  value: 1<<27\n  description:\
  \ Send mail on the user's behalf, or change a message's read state.\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: storage\n  value: 1<<29\n  description: Full control of the application's own unstructured storage.\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: modify_notification\n  value: 1<<30\n  description: Modify the state of the application's own notifications.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: lessons\n  value: 1<<34\n  description: Read the user's lesson information.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: classes\n  value: 1<<35\n  description: Read the user's timetable (including courses).\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: exams\n\
  \  value: 1<<36\n  description: Read the user's examination information.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: scores\n  value: 1<<37\n  description: Read the user's examination results.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: students_list\n  value: 1<<38\n  description: Read the enrolled-student roster for a class (teacher).\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: card_info\n  value: 1<<39\n  description: Read the user's campus-card information.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: card_transactions\n  value: 1<<40\n  description: Read the user's campus-card transaction records.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: write_card_info\n\
  \  value: 1<<41\n  description: Campus-card write operations — change the query password, report a card lost, top up\n    from a bound bank card.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: income\n  value: 1<<42\n  description: Query the user's income information.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: create_jaccount\n  value: 1<<43\n  description: Create a jAccount account.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: edit_jaccount\n  value: 1<<44\n  description: Modify a jAccount account.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: net_service_info\n  value: 1<<45\n  description: Read all personal network-service information for a specified user.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n\
  - scope: connect_wechat\n  value: 1<<46\n  description: Bind a jAccount to a WeChat account.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: connect_shmec\n  value: 1<<47\n  description: Bind a jAccount to a Shanghai Municipal Education Commission account.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: print\n  value: 1<<48\n  description: Self-service printing.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: connect_finance\n  value: 1<<49\n  description: Integrate with the finance appointment system.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: student_affairs\n  value: 1<<50\n  description: Retrieve student-affairs information.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope:\
  \ bus\n  value: 1<<51\n  description: Read campus-bus and inter-campus shuttle timetables and real-time information.\n  flows:\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n- scope: calendar\n  value: 1<<52\n  description: Synchronise calendar information.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.sjtu.edu.cn/auth/oauth.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shanghai-jiao-tong-university/refs/heads/main/scopes/shanghai-jiao-tong-university-scopes.yml
summary_line: 40 scopes · authorizationCode/clientCredentials/password
tags:
- University
- Higher Education
- Education
- Research
- China
- C9 League
- Identity Federation
- Course Catalog
- Research Computing
- Campus Life
- Authentication
- OpenID Connect
- SAML
- Shibboleth
- Payments
token_urls:
- https://jaccount.sjtu.edu.cn/oauth2/token
---
