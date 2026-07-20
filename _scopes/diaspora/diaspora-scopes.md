---
api_specs:
- filename: diaspora-api-openapi.yml
  format: yaml
  label: diaspora* API
  slug: diaspora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-api-openapi.yml
authorization_urls: []
description: diaspora* implements access scopes as defined by OAuth 2.0 (RFC 6749 §3.3), which OpenID Connect Core 1.0 builds on. A client requests a set of scopes when it requests an access token; the granted set may differ from the requested set. Every API endpoint requires at least one granted scope — a request carrying a token without the endpoint's scope returns 403 with no content. For some resources (posts, photos) the required scope depends on the visibility of the data (public vs private), and for others (streams) the granted scope set determines which data the response contains.
docs: https://diaspora.github.io/api-documentation/scopes.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Diaspora Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Diaspora uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Diaspora
provider_slug: diaspora
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: diaspora-scopes
source_filename: diaspora-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://diaspora.github.io/api-documentation/scopes.html — the official diaspora* \"Access scopes\"\n  reference. Cross-checked against the live scopes_supported list returned by\n  https://diaspora.social/.well-known/openid-configuration (HTTP 200) and against the per-operation\n  \"Required API scope\" annotations captured in openapi/diaspora-api-openapi.yml.\ndocs: https://diaspora.github.io/api-documentation/scopes.html\ndescription: >-\n  diaspora* implements access scopes as defined by OAuth 2.0 (RFC 6749 §3.3), which OpenID Connect\n  Core 1.0 builds on. A client requests a set of scopes when it requests an access token; the\n  granted set may differ from the requested set. Every API endpoint requires at least one granted\n  scope — a request carrying a token without the endpoint's scope returns 403 with no content.\n  For some resources (posts, photos) the required scope depends on the visibility of the data\n\
  \  (public vs private), and for others (streams) the granted scope set determines which data the\n  response contains.\n\nstandard: OAuth 2.0 / OpenID Connect Core 1.0\nscope_count: 16\nmandatory_scopes:\n- openid\nalways_granted_scopes:\n- public:read\n\nnotes:\n- >-\n  The openid scope is mandatory. If it is missing, API authentication fails outright.\n- >-\n  public:read is a special case: it is granted to every authorized client even when not explicitly\n  requested, because it only covers data that is public anyway. There is no way to opt out of it.\n- >-\n  Some scopes depend on other scopes and can only be granted alongside them.\n- >-\n  The live discovery document on diaspora.social also lists the OpenID claim names (name,\n  nickname, picture, sub) in scopes_supported alongside the real scopes; those are claims granted\n  via the profile scope, not independent scopes.\n\nscopes:\n- name: openid\n  origin: openid-connect\n  required: true\n  description: >-\n    Defined by the\
  \ OpenID Connect specification. Mandatory — allows using OpenID Connect\n    authentication. If missing, API authentication will fail.\n- name: profile\n  origin: openid-connect\n  description: >-\n    Defined by the OpenID Connect specification. Allows reading the user's own claims (user\n    properties) via the UserInfo route or from the ID Token, and grants access to the \"read own\n    profile\" diaspora* API endpoint.\n  grants_claims:\n  - claim: name\n    meaning: Full name\n  - claim: nickname\n    meaning: The left part of the diaspora handle, before the @ sign\n  - claim: profile\n    meaning: The user's profile URL address\n  - claim: picture\n    meaning: The user's avatar URL address\n  - claim: sub\n    meaning: The diaspora* ID of the user\n  operations:\n  - getUser\n- name: email\n  origin: openid-connect\n  description: >-\n    Defined by the OpenID Connect specification. Allows reading the user's own email address using\n    the UserInfo route or from the ID Token.\n\
  - name: profile:read_private\n  origin: diaspora\n  description: >-\n    Gives access to additional profile fields which are part of the user's private profile.\n- name: profile:modify\n  origin: diaspora\n  description: Gives access to updating a user's own profile.\n  operations:\n  - updateUser\n- name: public:read\n  origin: diaspora\n  always_granted: true\n  description: >-\n    Read public profiles of users, perform search among publicly searchable profiles, read public\n    posts, read reshares, and read public post interactions (likes, comments). Granted to any\n    authorized entity even when not explicitly requested.\n  operations:\n  - getPhotos\n  - getPhotosByPhotoGuid\n  - getPostsByPostGuid\n  - getPostsByPostGuidReshares\n  - getSearchUsers\n  - getSearchPosts\n  - getSearchTags\n  - getUsersByPersonGuid\n  - getUsersByPersonGuidPosts\n  - getUsersByPersonGuidPhotos\n- name: public:modify\n  origin: diaspora\n  description: >-\n    Create public posts and reshares, post\
  \ photos, delete public posts, and delete public photos.\n  operations:\n  - createPosts\n  - deletePostsByPostGuid\n  - createPhotos\n  - deletePhotosByPhotoGuid\n  - createPostsByPostGuidReshares\n- name: private:read\n  origin: diaspora\n  depends_on:\n  - contacts:read\n  description: >-\n    Read private posts, read private post interactions (likes, comments), and read streams — main\n    stream, aspects stream, mention stream, activity stream, liked stream and commented stream.\n  operations:\n  - getStreamsMain\n  - getStreamsAspects\n  - getStreamsActivity\n  - getStreamsMentions\n  - getStreamsLiked\n  - getStreamsCommented\n- name: private:modify\n  origin: diaspora\n  depends_on:\n  - contacts:read\n  description: >-\n    Create private posts, post photos privately, delete private posts, and delete private photos.\n- name: contacts:read\n  origin: diaspora\n  description: >-\n    Read the aspect list, read aspect membership, read private user profiles of contacts, read\n   \
  \ contacts of contacts when allowed by the contact's aspect setting, and include contacts hidden\n    from public search in user search results.\n  operations:\n  - getAspects\n  - getAspectsByAspectId\n  - getAspectsByAspectIdContacts\n- name: contacts:modify\n  origin: diaspora\n  description: >-\n    Add new aspects, rename aspects and change aspect properties, delete aspects, and add or remove\n    a person to/from aspects. Also covers blocking and unblocking a user.\n  operations:\n  - createAspects\n  - updateAspectsByAspectId\n  - deleteAspectsByAspectId\n  - createAspectsByAspectIdContacts\n  - deleteAspectsByAspectIdContactsByPersonGuid\n  - createUsersByPersonGuidBlock\n  - deleteUsersByPersonGuidBlock\n- name: conversations\n  origin: diaspora\n  description: >-\n    Gives access to private messaging — create conversations and send private messages.\n  operations:\n  - getConversations\n  - getConversationsByConversationGuid\n  - createConversations\n  - deleteConversationsByConversationGuid\n\
  \  - updateConversationsByConversationGuid\n  - getConversationsByConversationGuidMessages\n  - createConversationsByConversationGuidMessages\n- name: interactions\n  origin: diaspora\n  description: >-\n    Create and delete comments, report posts and comments, post and remove likes, subscribe to and\n    mute posts, hide posts from streams, and vote in polls. Read access to the underlying post must\n    also be present (public:read for public posts, private:read for private posts).\n  operations:\n  - createPostsByPostGuidComments\n  - deletePostsByPostGuidCommentsByCommentGuid\n  - createPostsByPostGuidCommentsByCommentGuidReport\n  - createPostsByPostGuidLikes\n  - deletePostsByPostGuidLikes\n  - createPostsByPostGuidCommentsByCommentGuidLikes\n  - deletePostsByPostGuidCommentsByCommentGuidLikes\n  - createPostsByPostGuidReport\n  - createPostsByPostGuidSubscribe\n  - createPostsByPostGuidMute\n  - createPostsByPostGuidHide\n  - createPostsByPostGuidVote\n- name: notifications\n  origin:\
  \ diaspora\n  description: Gives access to reading notifications.\n  operations:\n  - getNotifications\n  - getNotificationsByNotificationId\n  - updateNotificationsByNotificationId\n- name: tags:read\n  origin: diaspora\n  description: Gives access to reading tag followings and reading the tags stream.\n  operations:\n  - getTagFollowings\n- name: tags:modify\n  origin: diaspora\n  description: Gives access to creation and deletion of tag followings.\n  operations:\n  - createTagFollowings\n  - deleteTagFollowingsByTagName\n\ndependencies:\n- scope: private:read\n  requires:\n  - contacts:read\n- scope: private:modify\n  requires:\n  - contacts:read\n\nenforcement:\n  insufficient_scope_status: 403\n  insufficient_scope_body: none\n  unauthenticated_status: 401\n\nrelated:\n  authentication: authentication/diaspora-authentication.yml\n  openapi: openapi/diaspora-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/scopes/diaspora-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Social
- Social Networking
- Decentralized
- Federated
- Open Source
- Privacy
- Fediverse
- Messaging
- OpenID Connect
token_urls: []
---
