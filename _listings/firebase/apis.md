---
name: Firebase
x-slug: firebase
description: Firebase is a mobile platform that gives developers the tools and infrastructure
  to build better apps and grow successful businesses.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
x-kinRank: "9"
x-alexaRank: "1"
tags: History
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/firebase/apis.md
specificationVersion: "0.14"
apis:
- name: Firebase List HIstories
  x-api-slug: firebase
  description: |-
    Lists Histories for a given Project.

    The histories are sorted by modification time in descending order. The history_id key will be used to order the history with the same modification time.

    May return any of the following canonical error codes:

    - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the History does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/firebase/projectidhistories-get-openapi.md
- name: Firebase Create History
  x-api-slug: firebase
  description: |-
    Creates a History.

    The returned History will have the id set.

    May return any of the following canonical error codes:

    - PERMISSION_DENIED - if the user is not authorized to write to project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the containing project does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/firebase/projectidhistories-post-openapi.md
- name: Firebase Get History
  x-api-slug: firebase
  description: |-
    Gets a History.

    May return any of the following canonical error codes:

    - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the History does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/firebase/projectidhistorieshistoryid-get-openapi.md
- name: Firebase Get Executions
  x-api-slug: firebase
  description: |-
    Lists Histories for a given Project.

    The executions are sorted by creation_time in descending order. The execution_id key will be used to order the executions with the same creation_time.

    May return any of the following canonical error codes:

    - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the containing History does not exist
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}////{projectId}/histories/{historyId}/executions
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/firebase/projectidhistorieshistoryidexecutions-get-openapi.md
- name: Firebase
  x-api-slug: firebase
  description: Firebase is a mobile platform that gives developers the tools and infrastructure
    to build better apps and grow successful businesses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/firebase-logo.png
  humanURL: https://Firebase.google.com
  baseURL: https://{project_id].firebaseio.co}//
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/firebase/openapi.md
x-common:
- type: x-website
  url: https://Firebase.google.com
- type: x-blog
  url: https://firebase.googleblog.com/
- type: x-blog-rss
  url: http://firebase.googleblog.com/feeds/posts/default?alt=rss
- type: x-case-studies
  url: https://firebase.google.com/customers/
- type: x-change-log
  url: https://firebase.google.com/support/releases
- type: x-code
  url: https://firebase.google.com/docs/libraries/
- type: x-crunchbase
  url: https://crunchbase.com/organization/google
- type: x-documentation
  url: https://firebase.google.com/docs/
- type: x-faq
  url: https://firebase.google.com/support/faq/
- type: x-forum
  url: https://groups.google.com/forum/#!forum/firebase-talk
- type: x-github
  url: https://github.com/firebase
- type: x-pricing
  url: https://firebase.google.com/pricing/
- type: x-pricing
  url: https://adwords.google.com/home/pricing/
- type: x-slack
  url: https://firebase.community/
- type: x-submit-bug
  url: https://firebase.google.com/support/contact/bugs-features
- type: x-support
  url: https://firebase.google.com/support/
- type: x-twitter
  url: https://twitter.com/Google
- type: x-twitter
  url: https://twitter.com/firebase
- type: x-website
  url: https://firebase.google.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---