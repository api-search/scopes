---
authorization_urls: []
description: ''
docs: https://app.collimer.com/docs
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Collimer Scopes
name_suffix: OAuth Scopes
note: Scopes read from the advertised RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata; per-operation scope from x-mcp-required-scope in the v0 OpenAPI. The v1 OAuth2 scheme declares an empty scopes map; docs state both v1 scan routes require scans:write.
overview: 'Collimer publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Collimer API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Collimer
provider_slug: collimer-com
schemes: []
scope_count: 13
scope_names:
- brands:read
- brands:write
- articles:read
- articles:write
- articles:publish
- recommendations:read
- recommendations:write
- drafts:score
- scans:write
- audits:read
- audits:write
- identity:read
- offline_access
scopes:
- description: ''
  flows: []
  scope: brands:read
- description: ''
  flows: []
  scope: brands:write
- description: ''
  flows: []
  scope: articles:read
- description: ''
  flows: []
  scope: articles:write
- description: ''
  flows: []
  scope: articles:publish
- description: ''
  flows: []
  scope: recommendations:read
- description: ''
  flows: []
  scope: recommendations:write
- description: ''
  flows: []
  scope: drafts:score
- description: ''
  flows: []
  scope: scans:write
- description: ''
  flows: []
  scope: audits:read
- description: ''
  flows: []
  scope: audits:write
- description: ''
  flows: []
  scope: identity:read
- description: ''
  flows: []
  scope: offline_access
slug: collimer-com-scopes
source_filename: collimer-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://app.collimer.com/.well-known/oauth-authorization-server\ndocs: https://app.collimer.com/docs\nnote: Scopes read from the advertised RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata; per-operation scope from x-mcp-required-scope in the v0 OpenAPI. The v1 OAuth2 scheme\n  declares an empty scopes map; docs state both v1 scan routes require scans:write.\nscopes:\n- name: brands:read\n  operations:\n  - getBrand\n  - getBrandContext\n  - getClientRead\n  - listBrands\n  - resolveBrand\n- name: brands:write\n  operations:\n  - createBrand\n  - deleteBrand\n  - updateBrand\n  - updateBrandContext\n- name: articles:read\n  operations:\n  - exportArticle\n  - getArticle\n  - getAuditArtifact\n  - getRecap\n  - getRubric\n  - getWritingJobResult\n  - listChanges\n  - listFeedback\n  - listImpact\n  - listTemplates\n  - listWork\n  - verifyPublished\n- name: articles:write\n  operations:\n  - abandonPass\n\
  \  - advanceArticle\n  - applyCodeFix\n  - checkClaims\n  - checkCodeBlocks\n  - createFeedback\n  - createIdea\n  - deleteArticle\n  - discardFeedback\n  - editArticle\n  - findStatCandidates\n  - generateArticle\n  - importArticle\n  - insertStatCandidate\n  - restartArticle\n  - restoreArticle\n  - rewriteArticle\n  - suggestVisuals\n  - updateArticle\n- name: articles:publish\n  operations: []\n- name: recommendations:read\n  operations:\n  - getFinding\n  - getRecap\n  - getRecommendation\n  - getRecommendationVerification\n  - listFindings\n  - listRunRecommendations\n- name: recommendations:write\n  operations:\n  - updateFinding\n  - updateRecommendation\n  - verifyRecommendation\n  - verifyRunRecommendations\n- name: drafts:score\n  operations:\n  - scoreDraft\n- name: scans:write\n  operations:\n  - createScan\n  - getScanStatus\n- name: audits:read\n  operations:\n  - getAudit\n  - getAuditArtifact\n  - getRun\n  - listRuns\n- name: audits:write\n  operations:\n  - retryAudit\n\
  \  - startAudit\n- name: identity:read\n  operations: []\n- name: offline_access\n  operations: []\n"
source_yaml_url: https://artifacts.apis.io/collimer-com/scopes/collimer-com-scopes.yml
summary_line: 13 scopes
tags:
- Company
- AI Visibility
- Generative Engine Optimization
- SEO
- Marketing
- Analytics
- AI Search
token_bound: false
token_urls: []
---
