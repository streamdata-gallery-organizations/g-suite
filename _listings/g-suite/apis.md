---
name: G Suite
x-slug: g-suite
description: The collection of Google applications as one suite. Business email, shared
  calendars, and video conferencing that brings your team closer together from anywhere.
  Create, edit, store and share documents, spreadsheets, and presentations in your
  browser and across devices. Secure, fast, and easy IT administration management
  across your organization, data, and devices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-g-suite.png
x-kinRank: "9"
x-alexaRank: ""
tags: G Suite
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/g-suite/master/_listings/g-suite/apis.md
specificationVersion: "0.14"
apis:
- name: G Suite Activity API Get Activity
  x-api-slug: g-suite-activity-api
  description: Returns a list of activities visible to the current logged in user.
    Visible activities are determined by the visiblity settings of the object that
    was acted on, e.g. Drive files a user can see. An activity is a record of past
    events. Multiple events may be merged if they are similar. A request is scoped
    to activities from a given Google service using the source parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-g-suite.png
  humanURL: https://developers.google.com/google-apps/
  baseURL: ://www.googleapis.com//appsactivity/v1//activities
  tags: Activities
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/g-suite/master/_listings/g-suite/activities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/g-suite/master/_listings/g-suite/activities-get-openapi.md
- name: G Suite Activity API
  x-api-slug: g-suite-activity-api
  description: 'The Apps Activity API lets your app retrieve information about a users
    G Suite activity. Currently, the API supports retrieving activity from theGoogle
    Driveservice about changes to a users Google Drive files. This provides additional
    functionality on top the existingDrive APIfor your app to do things like:'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-g-suite.png
  humanURL: https://developers.google.com/google-apps/
  baseURL: ://www.googleapis.com//appsactivity/v1
  tags: G Suite
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/g-suite/master/_listings/g-suite/openapi.md
x-common:
- type: x-blog
  url: https://gsuite-developers.googleblog.com/
- type: x-blog-rss
  url: http://googleappdsdeveloper.blogspot.com/atom.xml
- type: x-documentation
  url: https://developers.google.com/google-apps/activity/
- type: x-newsletter
  url: https://developers.google.com/google-apps/newsletters/
- type: x-twitter
  url: https://twitter.com/gsuitedevs
- type: x-website
  url: https://developers.google.com/google-apps/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---