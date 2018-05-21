---
swagger: "2.0"
x-collection-name: G Suite
x-complete: 0
info:
  title: G Suite Activity API Get Activity
  description: Returns a list of activities visible to the current logged in user.
    Visible activities are determined by the visiblity settings of the object that
    was acted on, e.g. Drive files a user can see. An activity is a record of past
    events. Multiple events may be merged if they are similar. A request is scoped
    to activities from a given Google service using the source parameter.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /appsactivity/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /activities:
    get:
      summary: Get Activity
      description: Returns a list of activities visible to the current logged in user.
        Visible activities are determined by the visiblity settings of the object
        that was acted on, e.g. Drive files a user can see. An activity is a record
        of past events. Multiple events may be merged if they are similar. A request
        is scoped to activities from a given Google service using the source parameter.
      operationId: appsactivity.activities.list
      x-api-path-slug: activities-get
      parameters:
      - in: query
        name: drive.ancestorId
        description: Identifies the Drive folder containing the items for which to
          return activities
      - in: query
        name: drive.fileId
        description: Identifies the Drive item to return activities for
      - in: query
        name: groupingStrategy
        description: Indicates the strategy to use when grouping singleEvents items
          in the associated combinedEvent object
      - in: query
        name: pageSize
        description: The maximum number of events to return on a page
      - in: query
        name: pageToken
        description: A token to retrieve a specific page of results
      - in: query
        name: source
        description: The Google service from which to return activities
      - in: query
        name: userId
        description: Indicates the user to return activity for
      responses:
        200:
          description: OK
      tags:
      - Activities
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---