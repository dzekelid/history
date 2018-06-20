---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: History
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Courses API Details for a given date in gradebook history
    for this course
  x-api-slug: instructure-canvas-courses-api
  description: Details for a given date in gradebook history for this course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/date
  tags: Courses,Course,Id,Gradebook,History,Date
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historydate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historydate-get-openapi.md
- name: Instructure Canvas Courses API Lists submissions
  x-api-slug: instructure-canvas-courses-api
  description: Lists submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/date/graders/{grader_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Gradebook,History,Date,Graders,Grader,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Courses API Days in gradebook history for this course
  x-api-slug: instructure-canvas-courses-api
  description: Days in gradebook history for this course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/days
  tags: Courses,Course,Id,Gradebook,History,Days
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historydays-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historydays-get-openapi.md
- name: Instructure Canvas Courses API List uncollated submission versions
  x-api-slug: instructure-canvas-courses-api
  description: List uncollated submission versions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/feed
  tags: Courses,Course,Id,Gradebook,History,Feed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historyfeed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/coursescourse-idgradebook-historyfeed-get-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---