---
api_specs:
- filename: cubist-cubesigner-openapi-original.json
  format: json
  label: CubeSigner API
  slug: cubist-cubesigner
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubist/refs/heads/main/openapi/cubist-cubesigner-openapi-original.json
authorization_urls: []
description: ''
docs: https://cubist.dev/product-suite
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cubist Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cubist publishes 135 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cubist API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cubist
provider_slug: cubist
schemes:
- header: Authorization
  name: SignerAuth
  source: openapi/cubist-cubesigner-openapi-original.json
  type: session-token
- header: Authorization
  name: Oidc
  source: openapi/cubist-cubesigner-openapi-original.json
  type: oidc-exchange
scope_count: 135
scope_names:
- export:user:complete
- export:user:init
- manage:authMigration:identity:add
- manage:authMigration:identity:remove
- manage:authMigration:user:update
- manage:contact:create
- manage:contact:delete
- manage:contact:get
- manage:contact:list
- manage:contact:lookup:address
- manage:contact:update:addresses
- manage:contact:update:editPolicy
- manage:contact:update:metadata
- manage:contact:update:name
- manage:contact:update:owner
- manage:email:delete
- manage:email:get
- manage:email:update
- manage:export:org:get
- manage:export:user:delete
- manage:export:user:list
- manage:identity:add
- manage:identity:list
- manage:identity:remove
- manage:identity:verify
- manage:key:attest
- manage:key:create
- manage:key:delete
- manage:key:get
- manage:key:history:tx:list
- manage:key:import
- manage:key:list
- manage:key:list_roles
- manage:key:update:editPolicy
- manage:key:update:enabled
- manage:key:update:metadata
- manage:key:update:owner
- manage:key:update:policy
- manage:mfa:list
- manage:mfa:register:email
- manage:mfa:register:fido
- manage:mfa:register:totp
- manage:mfa:unregister:fido
- manage:mfa:unregister:totp
- manage:mfa:verify:totp
- manage:mfa:vote:cs
- manage:mfa:vote:email
- manage:mfa:vote:fido
- manage:mfa:vote:totp
- manage:mmi:delete
- manage:mmi:get
- manage:mmi:list
- manage:mmi:reject
- manage:org:addUser
- manage:org:audit:query
- manage:org:create
- manage:org:deleteUser
- manage:org:get
- manage:org:invitation:cancel
- manage:org:invitation:list
- manage:org:inviteUser
- manage:org:metrics:query
- manage:org:resetMfa
- manage:org:update:*
- manage:org:updateMembership
- manage:org:user:get
- manage:org:user:list
- manage:policy:bucket:get
- manage:policy:bucket:update:acl
- manage:policy:bucket:update:metadata
- manage:policy:buckets:list
- manage:policy:create
- manage:policy:createImportKey
- manage:policy:delete
- manage:policy:get
- manage:policy:invoke
- manage:policy:list
- manage:policy:logs:get
- manage:policy:secrets:get
- manage:policy:secrets:update
- manage:policy:secrets:update:editPolicy
- manage:policy:secrets:update:values
- manage:policy:update
- manage:policy:update:editPolicy
- manage:policy:update:name
- manage:policy:update:owner
- manage:policy:update:rule
- manage:policy:wasm:upload
- manage:role:attest
- manage:role:create
- manage:role:delete
- manage:role:get
- manage:role:get:keys
- manage:role:get:users
- manage:role:history:tx:list
- manage:role:list
- manage:role:update:editPolicy
- manage:role:update:enable
- manage:role:update:key:add
- manage:role:update:key:remove
- manage:role:update:policy
- manage:role:update:user:add
- manage:role:update:user:remove
- manage:session:create
- manage:session:get
- manage:session:list
- manage:session:revoke
- mmi:*
- rpc:*
- sign:ava
- sign:babylon:covenant
- sign:babylon:eots:nonces
- sign:babylon:eots:sign
- sign:babylon:registration
- sign:babylon:staking
- sign:blob
- sign:btc:message:legacy
- sign:btc:message:segwit
- sign:btc:psbt:legacy
- sign:btc:psbt:segwit
- sign:btc:psbt:taproot
- sign:btc:segwit
- sign:btc:taproot
- sign:diffieHellman
- sign:eth2:stake
- sign:eth2:unstake
- sign:eth2:validate
- sign:evm:eip191
- sign:evm:eip712
- sign:evm:eip7702
- sign:evm:tx
- sign:mmi
- sign:solana
- sign:sui
- sign:tendermint
scopes:
- description: Grants user complete access
  flows: []
  scope: export:user:complete
- description: Grants user init access
  flows: []
  scope: export:user:init
- description: Grants authMigration identity add access
  flows: []
  scope: manage:authMigration:identity:add
- description: Grants authMigration identity remove access
  flows: []
  scope: manage:authMigration:identity:remove
- description: Grants authMigration user update access
  flows: []
  scope: manage:authMigration:user:update
- description: Grants contact create access
  flows: []
  scope: manage:contact:create
- description: Grants contact delete access
  flows: []
  scope: manage:contact:delete
- description: Grants contact get access
  flows: []
  scope: manage:contact:get
- description: Grants contact list access
  flows: []
  scope: manage:contact:list
- description: Grants contact lookup address access
  flows: []
  scope: manage:contact:lookup:address
- description: Grants contact update addresses access
  flows: []
  scope: manage:contact:update:addresses
- description: Grants contact update editPolicy access
  flows: []
  scope: manage:contact:update:editPolicy
- description: Grants contact update metadata access
  flows: []
  scope: manage:contact:update:metadata
- description: Grants contact update name access
  flows: []
  scope: manage:contact:update:name
- description: Grants contact update owner access
  flows: []
  scope: manage:contact:update:owner
- description: Grants email delete access
  flows: []
  scope: manage:email:delete
- description: Grants email get access
  flows: []
  scope: manage:email:get
- description: Grants email update access
  flows: []
  scope: manage:email:update
- description: Grants export org get access
  flows: []
  scope: manage:export:org:get
- description: Grants export user delete access
  flows: []
  scope: manage:export:user:delete
- description: Grants export user list access
  flows: []
  scope: manage:export:user:list
- description: Grants identity add access
  flows: []
  scope: manage:identity:add
- description: Grants identity list access
  flows: []
  scope: manage:identity:list
- description: Grants identity remove access
  flows: []
  scope: manage:identity:remove
- description: Grants identity verify access
  flows: []
  scope: manage:identity:verify
- description: Grants key attest access
  flows: []
  scope: manage:key:attest
- description: Grants key create access
  flows: []
  scope: manage:key:create
- description: Grants key delete access
  flows: []
  scope: manage:key:delete
- description: Grants key get access
  flows: []
  scope: manage:key:get
- description: Grants key history tx list access
  flows: []
  scope: manage:key:history:tx:list
- description: Grants key import access
  flows: []
  scope: manage:key:import
- description: Grants key list access
  flows: []
  scope: manage:key:list
- description: Grants key list_roles access
  flows: []
  scope: manage:key:list_roles
- description: Grants key update editPolicy access
  flows: []
  scope: manage:key:update:editPolicy
- description: Grants key update enabled access
  flows: []
  scope: manage:key:update:enabled
- description: Grants key update metadata access
  flows: []
  scope: manage:key:update:metadata
- description: Grants key update owner access
  flows: []
  scope: manage:key:update:owner
- description: Grants key update policy access
  flows: []
  scope: manage:key:update:policy
- description: Grants mfa list access
  flows: []
  scope: manage:mfa:list
- description: Grants mfa register email access
  flows: []
  scope: manage:mfa:register:email
- description: Grants mfa register fido access
  flows: []
  scope: manage:mfa:register:fido
- description: Grants mfa register totp access
  flows: []
  scope: manage:mfa:register:totp
- description: Grants mfa unregister fido access
  flows: []
  scope: manage:mfa:unregister:fido
- description: Grants mfa unregister totp access
  flows: []
  scope: manage:mfa:unregister:totp
- description: Grants mfa verify totp access
  flows: []
  scope: manage:mfa:verify:totp
- description: Grants mfa vote cs access
  flows: []
  scope: manage:mfa:vote:cs
- description: Grants mfa vote email access
  flows: []
  scope: manage:mfa:vote:email
- description: Grants mfa vote fido access
  flows: []
  scope: manage:mfa:vote:fido
- description: Grants mfa vote totp access
  flows: []
  scope: manage:mfa:vote:totp
- description: Grants mmi delete access
  flows: []
  scope: manage:mmi:delete
- description: Grants mmi get access
  flows: []
  scope: manage:mmi:get
- description: Grants mmi list access
  flows: []
  scope: manage:mmi:list
- description: Grants mmi reject access
  flows: []
  scope: manage:mmi:reject
- description: Grants org addUser access
  flows: []
  scope: manage:org:addUser
- description: Grants org audit query access
  flows: []
  scope: manage:org:audit:query
- description: Grants org create access
  flows: []
  scope: manage:org:create
- description: Grants org deleteUser access
  flows: []
  scope: manage:org:deleteUser
- description: Grants org get access
  flows: []
  scope: manage:org:get
- description: Grants org invitation cancel access
  flows: []
  scope: manage:org:invitation:cancel
- description: Grants org invitation list access
  flows: []
  scope: manage:org:invitation:list
- description: Grants org inviteUser access
  flows: []
  scope: manage:org:inviteUser
- description: Grants org metrics query access
  flows: []
  scope: manage:org:metrics:query
- description: Grants org resetMfa access
  flows: []
  scope: manage:org:resetMfa
- description: Grants org update * access
  flows: []
  scope: manage:org:update:*
- description: Grants org updateMembership access
  flows: []
  scope: manage:org:updateMembership
- description: Grants org user get access
  flows: []
  scope: manage:org:user:get
- description: Grants org user list access
  flows: []
  scope: manage:org:user:list
- description: Grants policy bucket get access
  flows: []
  scope: manage:policy:bucket:get
- description: Grants policy bucket update acl access
  flows: []
  scope: manage:policy:bucket:update:acl
- description: Grants policy bucket update metadata access
  flows: []
  scope: manage:policy:bucket:update:metadata
- description: Grants policy buckets list access
  flows: []
  scope: manage:policy:buckets:list
- description: Grants policy create access
  flows: []
  scope: manage:policy:create
- description: Grants policy createImportKey access
  flows: []
  scope: manage:policy:createImportKey
- description: Grants policy delete access
  flows: []
  scope: manage:policy:delete
- description: Grants policy get access
  flows: []
  scope: manage:policy:get
- description: Grants policy invoke access
  flows: []
  scope: manage:policy:invoke
- description: Grants policy list access
  flows: []
  scope: manage:policy:list
- description: Grants policy logs get access
  flows: []
  scope: manage:policy:logs:get
- description: Grants policy secrets get access
  flows: []
  scope: manage:policy:secrets:get
- description: Grants policy secrets update access
  flows: []
  scope: manage:policy:secrets:update
- description: Grants policy secrets update editPolicy access
  flows: []
  scope: manage:policy:secrets:update:editPolicy
- description: Grants policy secrets update values access
  flows: []
  scope: manage:policy:secrets:update:values
- description: Grants policy update access
  flows: []
  scope: manage:policy:update
- description: Grants policy update editPolicy access
  flows: []
  scope: manage:policy:update:editPolicy
- description: Grants policy update name access
  flows: []
  scope: manage:policy:update:name
- description: Grants policy update owner access
  flows: []
  scope: manage:policy:update:owner
- description: Grants policy update rule access
  flows: []
  scope: manage:policy:update:rule
- description: Grants policy wasm upload access
  flows: []
  scope: manage:policy:wasm:upload
- description: Grants role attest access
  flows: []
  scope: manage:role:attest
- description: Grants role create access
  flows: []
  scope: manage:role:create
- description: Grants role delete access
  flows: []
  scope: manage:role:delete
- description: Grants role get access
  flows: []
  scope: manage:role:get
- description: Grants role get keys access
  flows: []
  scope: manage:role:get:keys
- description: Grants role get users access
  flows: []
  scope: manage:role:get:users
- description: Grants role history tx list access
  flows: []
  scope: manage:role:history:tx:list
- description: Grants role list access
  flows: []
  scope: manage:role:list
- description: Grants role update editPolicy access
  flows: []
  scope: manage:role:update:editPolicy
- description: Grants role update enable access
  flows: []
  scope: manage:role:update:enable
- description: Grants role update key add access
  flows: []
  scope: manage:role:update:key:add
- description: Grants role update key remove access
  flows: []
  scope: manage:role:update:key:remove
- description: Grants role update policy access
  flows: []
  scope: manage:role:update:policy
- description: Grants role update user add access
  flows: []
  scope: manage:role:update:user:add
- description: Grants role update user remove access
  flows: []
  scope: manage:role:update:user:remove
- description: Grants session create access
  flows: []
  scope: manage:session:create
- description: Grants session get access
  flows: []
  scope: manage:session:get
- description: Grants session list access
  flows: []
  scope: manage:session:list
- description: Grants session revoke access
  flows: []
  scope: manage:session:revoke
- description: Grants * access
  flows: []
  scope: mmi:*
- description: Grants * access
  flows: []
  scope: rpc:*
- description: Grants ava access
  flows: []
  scope: sign:ava
- description: Grants babylon covenant access
  flows: []
  scope: sign:babylon:covenant
- description: Grants babylon eots nonces access
  flows: []
  scope: sign:babylon:eots:nonces
- description: Grants babylon eots sign access
  flows: []
  scope: sign:babylon:eots:sign
- description: Grants babylon registration access
  flows: []
  scope: sign:babylon:registration
- description: Grants babylon staking access
  flows: []
  scope: sign:babylon:staking
- description: Grants blob access
  flows: []
  scope: sign:blob
- description: Grants btc message legacy access
  flows: []
  scope: sign:btc:message:legacy
- description: Grants btc message segwit access
  flows: []
  scope: sign:btc:message:segwit
- description: Grants btc psbt legacy access
  flows: []
  scope: sign:btc:psbt:legacy
- description: Grants btc psbt segwit access
  flows: []
  scope: sign:btc:psbt:segwit
- description: Grants btc psbt taproot access
  flows: []
  scope: sign:btc:psbt:taproot
- description: Grants btc segwit access
  flows: []
  scope: sign:btc:segwit
- description: Grants btc taproot access
  flows: []
  scope: sign:btc:taproot
- description: Grants diffieHellman access
  flows: []
  scope: sign:diffieHellman
- description: Grants eth2 stake access
  flows: []
  scope: sign:eth2:stake
- description: Grants eth2 unstake access
  flows: []
  scope: sign:eth2:unstake
- description: Grants eth2 validate access
  flows: []
  scope: sign:eth2:validate
- description: Grants evm eip191 access
  flows: []
  scope: sign:evm:eip191
- description: Grants evm eip712 access
  flows: []
  scope: sign:evm:eip712
- description: Grants evm eip7702 access
  flows: []
  scope: sign:evm:eip7702
- description: Grants evm tx access
  flows: []
  scope: sign:evm:tx
- description: Grants mmi access
  flows: []
  scope: sign:mmi
- description: Grants solana access
  flows: []
  scope: sign:solana
- description: Grants sui access
  flows: []
  scope: sign:sui
- description: Grants tendermint access
  flows: []
  scope: sign:tendermint
slug: cubist-scopes
source_filename: cubist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cubist-cubesigner-openapi-original.json\ndocs: https://cubist.dev/product-suite\nmodel: CubeSigner session-token scopes. OIDC tokens are exchanged for signer session tokens; each session\n  (and each Role access token) is minted with a scope set drawn from this list. Scopes follow a manage:<domain>:<action>\n  / sign:<chain> / export:user:<phase> grammar. Role scopes gate what a session may do (least-privilege\n  signing).\nschemes:\n- name: SignerAuth\n  type: session-token\n  header: Authorization\n  source: openapi/cubist-cubesigner-openapi-original.json\n- name: Oidc\n  type: oidc-exchange\n  header: Authorization\n  source: openapi/cubist-cubesigner-openapi-original.json\nscope_count: 135\nscopes:\n- scope: export:user:complete\n  description: Grants user complete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: export:user:init\n  description: Grants user init access\n  sources:\n\
  \  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:authMigration:identity:add\n  description: Grants authMigration identity add access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:authMigration:identity:remove\n  description: Grants authMigration identity remove access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:authMigration:user:update\n  description: Grants authMigration user update access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:create\n  description: Grants contact create access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:delete\n  description: Grants contact delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:get\n  description: Grants contact get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:list\n\
  \  description: Grants contact list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:lookup:address\n  description: Grants contact lookup address access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:update:addresses\n  description: Grants contact update addresses access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:update:editPolicy\n  description: Grants contact update editPolicy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:update:metadata\n  description: Grants contact update metadata access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:update:name\n  description: Grants contact update name access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:contact:update:owner\n  description: Grants contact update owner access\n  sources:\n\
  \  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:email:delete\n  description: Grants email delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:email:get\n  description: Grants email get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:email:update\n  description: Grants email update access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:export:org:get\n  description: Grants export org get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:export:user:delete\n  description: Grants export user delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:export:user:list\n  description: Grants export user list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:identity:add\n  description: Grants identity add access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n\
  - scope: manage:identity:list\n  description: Grants identity list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:identity:remove\n  description: Grants identity remove access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:identity:verify\n  description: Grants identity verify access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:attest\n  description: Grants key attest access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:create\n  description: Grants key create access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:delete\n  description: Grants key delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:get\n  description: Grants key get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:history:tx:list\n  description:\
  \ Grants key history tx list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:import\n  description: Grants key import access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:list\n  description: Grants key list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:list_roles\n  description: Grants key list_roles access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:update:editPolicy\n  description: Grants key update editPolicy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:update:enabled\n  description: Grants key update enabled access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:update:metadata\n  description: Grants key update metadata access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:update:owner\n\
  \  description: Grants key update owner access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:key:update:policy\n  description: Grants key update policy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:list\n  description: Grants mfa list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:register:email\n  description: Grants mfa register email access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:register:fido\n  description: Grants mfa register fido access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:register:totp\n  description: Grants mfa register totp access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:unregister:fido\n  description: Grants mfa unregister fido access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:unregister:totp\n\
  \  description: Grants mfa unregister totp access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:verify:totp\n  description: Grants mfa verify totp access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:vote:cs\n  description: Grants mfa vote cs access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:vote:email\n  description: Grants mfa vote email access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:vote:fido\n  description: Grants mfa vote fido access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mfa:vote:totp\n  description: Grants mfa vote totp access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mmi:delete\n  description: Grants mmi delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mmi:get\n  description: Grants mmi\
  \ get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mmi:list\n  description: Grants mmi list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:mmi:reject\n  description: Grants mmi reject access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:addUser\n  description: Grants org addUser access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:audit:query\n  description: Grants org audit query access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:create\n  description: Grants org create access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:deleteUser\n  description: Grants org deleteUser access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:get\n  description: Grants org get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n\
  - scope: manage:org:invitation:cancel\n  description: Grants org invitation cancel access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:invitation:list\n  description: Grants org invitation list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:inviteUser\n  description: Grants org inviteUser access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:metrics:query\n  description: Grants org metrics query access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:resetMfa\n  description: Grants org resetMfa access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:update:*\n  description: Grants org update * access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:updateMembership\n  description: Grants org updateMembership access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n\
  - scope: manage:org:user:get\n  description: Grants org user get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:org:user:list\n  description: Grants org user list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:bucket:get\n  description: Grants policy bucket get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:bucket:update:acl\n  description: Grants policy bucket update acl access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:bucket:update:metadata\n  description: Grants policy bucket update metadata access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:buckets:list\n  description: Grants policy buckets list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:create\n  description: Grants policy create access\n  sources:\n\
  \  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:createImportKey\n  description: Grants policy createImportKey access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:delete\n  description: Grants policy delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:get\n  description: Grants policy get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:invoke\n  description: Grants policy invoke access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:list\n  description: Grants policy list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:logs:get\n  description: Grants policy logs get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:secrets:get\n  description: Grants policy secrets get access\n  sources:\n\
  \  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:secrets:update\n  description: Grants policy secrets update access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:secrets:update:editPolicy\n  description: Grants policy secrets update editPolicy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:secrets:update:values\n  description: Grants policy secrets update values access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:update\n  description: Grants policy update access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:update:editPolicy\n  description: Grants policy update editPolicy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:update:name\n  description: Grants policy update name access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n\
  - scope: manage:policy:update:owner\n  description: Grants policy update owner access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:update:rule\n  description: Grants policy update rule access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:policy:wasm:upload\n  description: Grants policy wasm upload access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:attest\n  description: Grants role attest access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:create\n  description: Grants role create access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:delete\n  description: Grants role delete access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:get\n  description: Grants role get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:get:keys\n\
  \  description: Grants role get keys access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:get:users\n  description: Grants role get users access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:history:tx:list\n  description: Grants role history tx list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:list\n  description: Grants role list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:update:editPolicy\n  description: Grants role update editPolicy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:update:enable\n  description: Grants role update enable access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:update:key:add\n  description: Grants role update key add access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n-\
  \ scope: manage:role:update:key:remove\n  description: Grants role update key remove access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:update:policy\n  description: Grants role update policy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:update:user:add\n  description: Grants role update user add access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:role:update:user:remove\n  description: Grants role update user remove access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:session:create\n  description: Grants session create access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:session:get\n  description: Grants session get access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: manage:session:list\n  description: Grants session list access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n\
  - scope: manage:session:revoke\n  description: Grants session revoke access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: mmi:*\n  description: Grants * access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: rpc:*\n  description: Grants * access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:ava\n  description: Grants ava access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:babylon:covenant\n  description: Grants babylon covenant access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:babylon:eots:nonces\n  description: Grants babylon eots nonces access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:babylon:eots:sign\n  description: Grants babylon eots sign access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:babylon:registration\n  description: Grants babylon registration\
  \ access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:babylon:staking\n  description: Grants babylon staking access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:blob\n  description: Grants blob access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:message:legacy\n  description: Grants btc message legacy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:message:segwit\n  description: Grants btc message segwit access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:psbt:legacy\n  description: Grants btc psbt legacy access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:psbt:segwit\n  description: Grants btc psbt segwit access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:psbt:taproot\n  description: Grants btc psbt taproot access\n  sources:\n\
  \  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:segwit\n  description: Grants btc segwit access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:btc:taproot\n  description: Grants btc taproot access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:diffieHellman\n  description: Grants diffieHellman access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:eth2:stake\n  description: Grants eth2 stake access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:eth2:unstake\n  description: Grants eth2 unstake access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:eth2:validate\n  description: Grants eth2 validate access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:evm:eip191\n  description: Grants evm eip191 access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope:\
  \ sign:evm:eip712\n  description: Grants evm eip712 access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:evm:eip7702\n  description: Grants evm eip7702 access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:evm:tx\n  description: Grants evm tx access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:mmi\n  description: Grants mmi access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:solana\n  description: Grants solana access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:sui\n  description: Grants sui access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n- scope: sign:tendermint\n  description: Grants tendermint access\n  sources:\n  - openapi/cubist-cubesigner-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubist/refs/heads/main/scopes/cubist-scopes.yml
summary_line: 135 scopes
tags:
- Company
- Developer Tools
- Key Management
- Wallets
- Digital Signatures
- Security
- Blockchain
- Web3
- Custody
token_urls: []
---
