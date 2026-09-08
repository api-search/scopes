---
api_specs:
- filename: university-of-waikato-uowidp-openapi.yml
  format: yaml
  label: University of Waikato Identity Provider (uowidp)
  slug: uowidp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waikato/refs/heads/main/openapi/university-of-waikato-uowidp-openapi.yml
authorization_urls: []
description: The complete authorization scope surface the University of Waikato publishes. The institution's own OpenID Connect provider declares three scopes in scopes_supported, and nothing else on the estate publishes a scope vocabulary — the DSpace REST API and OAI-PMH interface are anonymous reads, the One-Time Secret API is HTTP Basic with no scoping, and LTI 1.3 tool launches carry 1EdTech message claims rather than named OAuth scopes. Scopes here are transcribed from the provider's own discovery document; none is inferred.
docs: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: University Of Waikato Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Waikato publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Waikato API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Waikato
provider_slug: university-of-waikato
schemes:
- authorizationUrl: https://api.svc.waikato.ac.nz/uowidp/v1/auth
  issuer: https://api.svc.waikato.ac.nz/uowidp/v1
  name: uowidp
  notes: No incremental or resource-specific scopes are advertised. Access to a university system is decided by the client registration ITS issues, not by scope selection at the authorization endpoint.
  operator: institution
  tokenUrl: https://api.svc.waikato.ac.nz/uowidp/v1/token
  type: openIdConnect
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: Required for OpenID Connect; requests an id_token identifying the university account.
  flows: []
  scope: openid
- description: Requests profile claims. The provider advertises claims_supported [iss, aud, nbf, exp, iat, nonce, Username, name, ver, oid, sub]; `Username` and `name` are the profile-bearing claims.
  flows: []
  scope: profile
- description: Requests the university email address claim.
  flows: []
  scope: email
slug: university-of-waikato-scopes
source_filename: university-of-waikato-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration\ndocs: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration\ndescription: >-\n  The complete authorization scope surface the University of Waikato publishes. The institution's\n  own OpenID Connect provider declares three scopes in scopes_supported, and nothing else on the\n  estate publishes a scope vocabulary — the DSpace REST API and OAI-PMH interface are anonymous\n  reads, the One-Time Secret API is HTTP Basic with no scoping, and LTI 1.3 tool launches carry\n  1EdTech message claims rather than named OAuth scopes. Scopes here are transcribed from the\n  provider's own discovery document; none is inferred.\nschemes:\n- name: uowidp\n  type: openIdConnect\n  operator: institution\n  issuer: https://api.svc.waikato.ac.nz/uowidp/v1\n  authorizationUrl: https://api.svc.waikato.ac.nz/uowidp/v1/auth\n  tokenUrl: https://api.svc.waikato.ac.nz/uowidp/v1/token\n\
  \  notes: >-\n    No incremental or resource-specific scopes are advertised. Access to a university system is\n    decided by the client registration ITS issues, not by scope selection at the authorization\n    endpoint.\nscopes:\n- scope: openid\n  scheme: uowidp\n  description: Required for OpenID Connect; requests an id_token identifying the university account.\n- scope: profile\n  scheme: uowidp\n  description: >-\n    Requests profile claims. The provider advertises claims_supported [iss, aud, nbf, exp, iat,\n    nonce, Username, name, ver, oid, sub]; `Username` and `name` are the profile-bearing claims.\n- scope: email\n  scheme: uowidp\n  description: Requests the university email address claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waikato/refs/heads/main/scopes/university-of-waikato-scopes.yml
summary_line: 3 scopes
tags:
- Education
- Higher Education
- University
- New Zealand
- Research
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- SAML
- OpenID Connect
- Learning Management
- Machine Learning
token_urls: []
---
