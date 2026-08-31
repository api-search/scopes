---
api_specs:
- filename: universite-de-montreal-sadvr-openapi.yml
  format: yaml
  label: SADVR REST API (Vitrine-Recherche)
  slug: sadvr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/openapi/universite-de-montreal-sadvr-openapi.yml
authorization_urls: []
description: Authorization scopes across Université de Montréal's programmable surfaces. The institution publishes no OAuth 2.0 authorization server and therefore defines no OAuth scopes. What it does operate is a SAML attribute release policy through its Shibboleth IdP, which is the functional equivalent for the federated surfaces — and it is the only place where UdeM makes an access-control decision about a machine-readable identity.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Universite De Montreal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Université de Montréal uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Université de Montréal
provider_slug: universite-de-montreal
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: universite-de-montreal-scopes
source_filename: universite-de-montreal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nspecification: API Commons Scopes\nspecificationVersion: '0.1'\nprovider: Université de Montréal\nproviderId: universite-de-montreal\ngenerated: '2026-08-30'\nmethod: probed\nsource: live probes of Université de Montréal surfaces, 2026-08-30\ndescription: >-\n  Authorization scopes across Université de Montréal's programmable surfaces. The institution\n  publishes no OAuth 2.0 authorization server and therefore defines no OAuth scopes. What it does\n  operate is a SAML attribute release policy through its Shibboleth IdP, which is the functional\n  equivalent for the federated surfaces — and it is the only place where UdeM makes an\n  access-control decision about a machine-readable identity.\noauth2:\n  present: false\n  detail: >-\n    No authorization server, no token endpoint, no .well-known/oauth-authorization-server and no\n    .well-known/openid-configuration were found on any umontreal.ca host. No scope vocabulary\n    exists to record.\nscopes: []\nalternative_authorization:\n\
  - mechanism: SAML attribute release\n  x-operator: institution\n  surface: https://shibboleth.umontreal.ca/idp/shibboleth\n  detail: >-\n    The IdP declares an AttributeAuthorityDescriptor supporting SAML 1.1, meaning attribute\n    queries are answered out of band as well as in the assertion. The scope asserted for released\n    attributes is shibmd:Scope \"umontreal.ca\" — a service provider must reject any scoped\n    attribute value from this IdP that does not carry that domain. The attribute release policy\n    itself is not public; it is negotiated per service provider through the federation.\n  evidence:\n    url: https://shibboleth.umontreal.ca/idp/shibboleth\n    status: 200\n- mechanism: SADVR consent flags\n  x-operator: institution\n  surface: https://www.recherche.umontreal.ca/vitrine/rest/api/1.8/umontreal/info/individu\n  detail: >-\n    Not an authorization mechanism in the technical sense, but it is the only access constraint\n    the SADVR API expresses. Each full individual\
  \ record carries a `consentement` object naming\n    the UdeM showcases the person agreed to appear in (\"Vitrine de la recherche\", \"Répertoire des\n    experts à l'intention des médias\") with a `statutConsentement` flag, and an `affichageWeb`\n    block giving the URLs where that consent applies. Each affiliation also carries `exclusion`\n    and `exclusionTel` flags. The API returns the data regardless; honouring the flags is left\n    entirely to the consumer.\n  evidence:\n    url: https://www.recherche.umontreal.ca/vitrine/rest/api/1.8/umontreal/info/individu?idsadvr=in13593\n    status: 200\n- mechanism: Dataverse API token\n  x-operator: tenant\n  surface: https://borealisdata.ca/api\n  detail: >-\n    Borealis issues per-account Dataverse API tokens with permissions derived from the Dataverse\n    role model, not from a scope string. UdeM does not define or issue these.\nnotes: >-\n  Recording an empty `scopes` list is the honest measurement here. It is not a gap in the probe\
  \ —\n  it is the finding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/scopes/universite-de-montreal-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Canada
- Québec
- French Language
- U15
- Public Research University
- Research
- Research Data
- Research Expertise
- Identity Federation
- Institutional Repository
- Library
- Open Access
- OAI-PMH
- Shibboleth
- SAML
token_urls: []
---
