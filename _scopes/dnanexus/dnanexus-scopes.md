---
authorization_urls:
- https://oidc.dnanexus.com/authorize
description: ''
docs: https://documentation.dnanexus.com/developer/api/oidc-clients
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Dnanexus Scopes
name_suffix: OAuth Scopes
note: The DNAnexus Platform API itself (api.dnanexus.com) is bearer-token authenticated and has NO OAuth scope surface - a token carries the full permissions of the user or job it was issued for, and access is instead constrained by project/org permission levels (VIEW / UPLOAD / CONTRIBUTE / ADMINISTER). The scopes below belong to the DNAnexus OpenID Connect provider, which third-party web apps use to sign users in.
overview: 'DNAnexus publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DNAnexus API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DNAnexus
provider_slug: dnanexus
schemes:
- flows:
  - authorizationUrl: https://oidc.dnanexus.com/authorize
    flow: authorizationCode
    pkce: S256
    response_types:
    - code
  issuer: https://oidc.dnanexus.com
  name: DNAnexusOIDC
  source: https://oidc.dnanexus.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- name
- email
- user_id
scopes:
- description: Required OpenID Connect scope; requests an ID token for the signed-in DNAnexus user.
  flows:
  - authorizationCode
  scope: openid
- description: Releases the DNAnexus user's display name as the `name` claim.
  flows:
  - authorizationCode
  scope: name
- description: Releases the DNAnexus user's email address as the `email` claim.
  flows:
  - authorizationCode
  scope: email
- description: Releases the DNAnexus platform user handle (user-xxxx) as the `user_id` claim.
  flows:
  - authorizationCode
  scope: user_id
slug: dnanexus-scopes
source_filename: dnanexus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://oidc.dnanexus.com/.well-known/openid-configuration\ndocs: https://documentation.dnanexus.com/developer/api/oidc-clients\nnote: >-\n  The DNAnexus Platform API itself (api.dnanexus.com) is bearer-token authenticated\n  and has NO OAuth scope surface - a token carries the full permissions of the user\n  or job it was issued for, and access is instead constrained by project/org\n  permission levels (VIEW / UPLOAD / CONTRIBUTE / ADMINISTER). The scopes below\n  belong to the DNAnexus OpenID Connect provider, which third-party web apps use to\n  sign users in.\nschemes:\n- name: DNAnexusOIDC\n  issuer: https://oidc.dnanexus.com\n  source: https://oidc.dnanexus.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oidc.dnanexus.com/authorize\n    pkce: S256\n    response_types: [code]\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope; requests an ID\
  \ token for the signed-in\n    DNAnexus user.\n  flows: [authorizationCode]\n  claims: [sub, sid, auth_time, iss]\n  sources: [https://oidc.dnanexus.com/.well-known/openid-configuration]\n- scope: name\n  description: Releases the DNAnexus user's display name as the `name` claim.\n  flows: [authorizationCode]\n  claims: [name]\n  sources: [https://oidc.dnanexus.com/.well-known/openid-configuration]\n- scope: email\n  description: Releases the DNAnexus user's email address as the `email` claim.\n  flows: [authorizationCode]\n  claims: [email]\n  sources: [https://oidc.dnanexus.com/.well-known/openid-configuration]\n- scope: user_id\n  description: Releases the DNAnexus platform user handle (user-xxxx) as the `user_id`\n    claim.\n  flows: [authorizationCode]\n  claims: [user_id]\n  sources: [https://oidc.dnanexus.com/.well-known/openid-configuration]\njob_identity_provider:\n  issuer: https://job-oidc.dnanexus.com\n  source: https://job-oidc.dnanexus.com/.well-known/openid-configuration\n\
  \  scopes: [openid]\n  note: >-\n    Job identity tokens support only the `openid` scope; the audience is set by the\n    caller and the claim set (job_id, project_id, app_name, bill_to, region, ...)\n    is what a relying cloud provider writes its trust policy against.\nplatform_permission_model:\n  docs: https://documentation.dnanexus.com/developer/api/data-containers/project-permissions-and-sharing\n  levels: [VIEW, UPLOAD, CONTRIBUTE, ADMINISTER]\n  note: >-\n    Project permission levels, not OAuth scopes, are the authorization surface for\n    the Platform API.\nx-evidence:\n  fetched: '2026-08-04'\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dnanexus/refs/heads/main/scopes/dnanexus-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Genomics
- Bioinformatics
- Life Sciences
- Healthcare
- Cloud Computing
- Data Platform
- Scientific Computing
- Precision Medicine
- Clinical Research
token_urls: []
---
